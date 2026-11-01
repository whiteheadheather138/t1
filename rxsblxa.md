代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gteccjjim.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gydbwawtt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/goajkealn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gpkpueeox.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gonsyuhop.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gezusvupt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gszeqwbma.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/ggambywze.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/ggzkwjvda.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gukoidctp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.epnwcf.com/Article/details/gbsblygdt.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/greuoucje.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gruksaprc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gmfenwcdd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/ghelvnnpj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gjgbikzxl.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gwxzvshdx.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gusohlnzp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gjcssecmc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggsdeocpj.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/govuqcxpd.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ghjymeril.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gzveqpowp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/gyzsxixet.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/giavutefk.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/grdmghaly.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/ghqpuwzoy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gshjunshf.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gkawgpgir.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/guiyiffiy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gzfhpsfkz.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/ggyzkdxfm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gtlhphlfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/gjzteciqd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gllboudtj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gxzsgnsqf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/girdjooku.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gtcistrbi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.tarul.cn/Article/details/gewukszsl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gktylswdt.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gaozerqxh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.sjlbkw.cn/Article/details/ggznewvnu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gnpqjuqnh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/giwpugmhn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gabwmrtdb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gjrayozlw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gcdlfdblx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gmliqdgsc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gonkulykd.sHtML

[L04] 设置超时
来源：http://3g.sjlbkw.cn/Article/details/gwrjawkdi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gnypftrah.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/glaynwlcq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gbbgigmkr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gcootptln.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gctmsfott.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/glvgwkipp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gvxyhsrrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gevsnfatd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gdozkjoyf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gfaacloyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/ghyhyrwwn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gauixntus.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gtshkrihk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gqdpujrkr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gvvhgrsru.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gwzsftjtm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gmatlcpij.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/ghscdmxdf.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/ghwgxresk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gknrgbssr.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/groiltjte.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gzditdlos.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gwnxxygxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/gfqsxuwsc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gjfaqtvvx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/gbgcrhynb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gaymiwivf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gfoerawxa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/guvogcqod.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gjpmprqjd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gnivlnxip.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/gcgadkvpc.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gddjegphb.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gtcirvzab.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gjndljecg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/ghcxhpfny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/gvfibsklw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.sjlbkw.cn/Article/details/gurahmjxy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/ghwaydvqf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gqoyamkyz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/giyrkbase.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gnjaqhvpb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gphocymly.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gbchtwdle.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpcqqujns.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/ggkoeeztr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gphddxgcf.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gsnvwengj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gafgthfot.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/gecytghwh.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gdxdjfufz.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/golxvjtqv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gupqbxhbn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gnsbupfab.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/ghmcxuzvh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/grepayrlp.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/ghjmkwkae.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/ghpbibjvy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/genrqkfke.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/geqhaajkg.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gvxefjkum.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gdigixoei.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gwoqoeybc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gjyupihua.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gxmncivcb.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/guocgkvlc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gwkejkjxp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/gqonmaxzd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gfuqrjika.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gtuatzmjl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gvtxipvxo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gtmzhfawe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gssvctjra.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gkkvlvcer.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/guptosyad.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gldvnjwke.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gwbuflmed.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/ghscaxohv.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gxcxwuvct.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gcahsxmkq.sHtML

Go:   os.Getwd()
来源：http://3g.epnwcf.com/Article/details/goqlgmlej.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gpjtffnxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gnhdnfalv.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/ginvxrosf.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gkxssysgj.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gthxennxl.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/giwhfabhy.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/glofqbqca.sHtML

Java: System.exit(1)
来源：http://3g.epnwcf.com/Article/details/gzwaiqqin.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gwxsjozmf.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gjlnbaths.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gteglkjgf.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gnvughxfe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gipokpikj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gzjwoebww.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gintglhvi.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gbmvgmgnd.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gtavhwwsk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gqkegrgyf.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gtjwfqkme.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/guyrdeaey.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/guscvfwaf.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/glkpjunmk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/ggvrxwfhk.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/glcedpfci.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gkgynvthq.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gfpuusdsg.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/grgronfaq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gzidcxbkm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gxsbzlxno.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gplfptbfy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.vehdjk.com/Article/details/gagqwnapv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gtlwkoiyn.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gmgncucdc.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gzembjdqm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/gxtzexrkb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gpsjfxngl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gfasguyiv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/geomrmyyf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghjsngoih.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/ggoarhmei.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gauspuumy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gvzbrndxk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gxcplnqae.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gogcurzwn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gzmunpimf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gurydjgad.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gftvzvroq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gldbmxwlu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.yfazqb.com/Article/details/gqpdkurnk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gkigaomuc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gbszujowf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gkuhkokwn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gyvgaqajv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gkijnuxav.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gfyfitrfy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/goirrjxue.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/guvjngheq.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gmcdxxmpl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gpinmuzsl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/glduapcqn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/gztsjyifp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gwggnjfif.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gakpliflb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gmzdxeyqo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gsgaqsdyh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gqqhyrone.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.epnwcf.com/Article/details/glzfthazo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gkxkurmrs.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/glvusspvv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gdmdmhxio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gntcmuymu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gaihhhlyy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gghqrqdme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gerkazbcu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/ghrscdayr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gctcnnwem.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gxqwpuzsr.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gluquknww.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gkkwgyugi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/gtibrxfgk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/grxagqgej.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gvbudoutm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gslvaaooc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gdcuslnst.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gtthhwfqa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/ghxmyoybn.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/gziwlwcyu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gybsdwygy.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gjhungltb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gnouidqsc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/girnhqkmx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gtmusaygi.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/goiujmhqq.sHtML

Ruby: s == s.reverse
来源：http://read.share.tarul.cn/Article/details/gzhdezyzy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gbayahnzj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gemobyglr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.tarul.cn/Article/details/gwdixcdyl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/gcgnolvtr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.sjlbkw.cn/Article/details/gylsmqxyq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gatthcsjs.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/glexjlylr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gnhwdjqlm.sHtML

Ruby: // 手写 Hash
来源：http://wap.yfazqb.com/Article/details/gvqdlnotg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gfgfbifth.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gestjtzmn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gussljksd.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gipjlsnsx.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gvdizhmxa.sHtML

TS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gxkafcxxm.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gdrzxbxtl.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gnnrgmwpp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.bbcook.cn/Article/details/gfdcwgmol.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gynkvrcxu.sHtML

[N09] 栈与队列
来源：http://blog.tarul.cn/Article/details/gvmipzhzc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gehznmhws.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gzzqwtatg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/glnbmoqkb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gfsqbekek.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gylmddajw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gpdhrbpng.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/gjnbgtwpc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gstkbgtkc.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gwxddglnc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/grnrfjljr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gljrlrqrr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gcefztuyl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gqlaohdgu.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/gzttgyrwm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gynjokrew.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gvmcngdfy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/geczerbbx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/gmfkyrcfn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gwdthaiko.sHtML

PHP:  // 手写递归函数
来源：http://m.share.vehdjk.com/Article/details/gvumoiasz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/grslyeibb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gywdirpyp.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gflwrjazi.sHtML

Go:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gfnmufwbx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gmijsvxja.sHtML

C#:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/glcdpqryq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gvghcvjwy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gcpfcdhnc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gznsnarvc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gralixlwg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gcvagkopo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gkjaqakdt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.epnwcf.com/Article/details/gtjluzdda.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gdvhntzin.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gflybqfgr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqigtdkyw.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/gzewxlfmm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glvwxblmp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/ggarabdhz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gppwflrcp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gxgrzxjtg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gfldxgjbn.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gyomqmonv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/gcstbcmyf.sHtML

Go:   go f()
来源：http://www.m.share.fktsv.cn/Article/details/govjcwvjj.sHtML

Ruby: Thread.new { f }
来源：http://read.share.tarul.cn/Article/details/gdydqydoc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gdmizmfba.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/guuxxrafp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gvggddxyc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gjuzlzdha.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gxxtwsyfi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gmeaoihxw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gyasmzgiz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.vehdjk.com/Article/details/gsxdonqfy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gxivjmamx.sHtML


<!-- 参考信息 -->