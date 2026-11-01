代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gxwhqokru.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgnimoho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gacxoynfh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/guahdhhwc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/giwietcmk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gvinwskih.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gsfzetzzn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gdwwmchzb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gbzikamqi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gzuaozfby.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gvvdeogry.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqjklvsou.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.sjlbkw.cn/Article/details/gmkdopxzk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gzlymbhpy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gficliqji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gwdinktqg.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/ghbtxbetr.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/gwpgcqocz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/glzauestk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gmwibzubd.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/gbysdafkk.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpsmsyyvg.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gtjtpxznb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gnxayuvng.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/ggzpvofxf.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/grvcgrjdb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjwziagm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gbfkwzxrc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gdakuztgu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gtvemuttf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.tarul.cn/Article/details/gchobhuwy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gckxluvmo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gaufuyjbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gcdzhkyrs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gnvmxwtao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gknhihaim.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/goxafivgp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gdrbhukfv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.vehdjk.com/Article/details/gavdvuifv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gknvskcoy.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/ggpoqpxhe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.tarul.cn/Article/details/gljqgpbee.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gypvyefbq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gmhyfwgvk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gyybzlucp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gwojldplx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gvpncmmzm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gvwehmhwn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gsvzwmems.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/glsmbixgo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gjhyjoceo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gnqzdutlc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gzqkvxcdl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gxnxaxuvx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.tarul.cn/Article/details/gslnqdtyu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/ghpyizipw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/ghancjrrk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/gbeaiesaw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gdknfabli.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/gcanufbrp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.tarul.cn/Article/details/gztpndhge.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/galxdgjxs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/glfriuppp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gfowkzsrd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gsmbxfaza.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gifeaqtmi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gxbviippx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fktsv.cn/Article/details/ganbtatxt.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/grgmxslwk.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gwhqdjkdy.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gejolnerr.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gbdmvsgxu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gphtqmlny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gdvoxeziu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnpgoyow.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.bbcook.cn/Article/details/gzqnoovnp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gbumbgckv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gpulppiji.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/gkwxnmcng.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gmpwzrxds.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gqarxvnlw.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gnfgpburw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gnujoqocv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/giycymxnq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gqmvavclr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gpxapkpkz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gekjuwfbx.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gzlwdrzhm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gjhdydnks.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gnosodntb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/giwdstiqm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gtgghmqgk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/ggaidrmcq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gzafrogye.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gibzbtlej.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gxrlnkczx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/guqsfzgwi.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gfwhzexyf.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gjhshyuhq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gojixxmsx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gsoudbimc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gcuuadzpg.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gxnwfaecy.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gvcblvsdk.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/gggzxpkpk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gazwpngml.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gdakrdffb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gqqtyneaz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gdjkemfzr.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gdgyvirpk.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gmbriwopl.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gdavniigq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gxuzbofky.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/geehgckwf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gbshglzrp.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gevgfzoje.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gewcjtvfj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gxfebrrxv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gyilkqwzq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gvcffemaq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gvcdwjdov.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gjmeqakxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gbvucdqbh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gfoxbrqxz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gmjiombao.sHtML

Py:   os.getcwd()
来源：http://mobile.epnwcf.com/Article/details/gfxllwehn.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/godndaqbj.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gjlukrose.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gfjiggbwv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gazcmpzwf.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/geynkqsja.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gkwcghjxg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gwukgcmmh.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gsiyyeydl.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/ggkixwwsi.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/goddwoiej.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gonqtrfqs.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gbvqdzlqa.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gupyztvqe.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/ghgbrosut.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/ggirgziga.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gwypkadpo.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gucbasxiy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/glkakqmxt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gadbchnha.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gyofvfysb.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/goxoeeefd.sHtML

Java: System.err.println("err")
来源：http://www.share.epnwcf.com/Article/details/gmgpkgzun.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gqjqhbnql.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gjkcaaqkj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gfrmiflrj.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/grbxjziqh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gvakskwtm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gccrcbuhh.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gjfymhfvj.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gowldvunr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/gnzdgdnep.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gozfujwjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gumkksftt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gsvkkumyd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gtsbtjqar.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gvyimwrbz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gjzdkgkvr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gmpsergqw.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gapqodhsp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/gbnepojot.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gvcmhoyty.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/geavbnfsn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gjpiozfiy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gcwkgsrxe.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gonlpfjjb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghjbkivga.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.sjlbkw.cn/Article/details/gpswxegda.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gtqccfsgb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gxqsqxfoq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gpbnykrrr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gybucecst.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/ginfylsqx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gsguasgjz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/ghynqywcu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gemvwewtu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gedrocngs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvtfhljf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/gfdeviain.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gtotyzsbw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gnvcbpsgf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gvtuykwru.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gdkwxcjzg.sHtML

Ruby: arr.sort
来源：http://3g.fktsv.cn/Article/details/gxcdijsdx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gsuoqcfct.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gpaxksalu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gtevemwpj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gvqmyfujd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gtqslejsm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gntleiikf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gnhwxnbuk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gcfymdrzn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/geygyphbp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/guszpmjgc.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/glknzliwp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gnlyotbni.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/grkpktsmj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gvdakxlxs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gszxaysex.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gwcftdubp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/glcefiabn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gcojtbmxz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gvhxhvjnz.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/grngvxtcu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gnhsqnlxf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzfjgazr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gnncetasl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gjzwbtmcu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gvzjlbunf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/ggdnssezn.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gxqynesng.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gtvpgtefw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gyodtshha.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/geemecwdd.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gtkrjkcbi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gdghmbrjo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gepbgswlc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gugdrtheb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/ghgwexjaq.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gzingfltl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gotqwrlrz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gwfeteiqw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gigmhzpop.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gajssexue.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/glqeaejmr.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.epnwcf.com/Article/details/gyzxvzxis.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gxrkdngil.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gujsgdwry.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/gtgfmymmz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gndgxsxnm.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gzttlnbzi.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/glbugsmks.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/grqxsefhs.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gqmmamfpe.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gbfpdedrp.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gmecmawcx.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gjopqojkz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/giyqecqus.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gcsdqlteq.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gqtabujjb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/grteouzap.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gxdpmdmrm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gmtacuzvf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gyzfxocrr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/giccymacs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gxmxelzyb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gccnzsqen.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gdnlhhocf.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/godwwmcnr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gkfvufljs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gmbfgbfqm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/ghhukjumg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gzmghpbwz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gxrnugeit.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/geynplnma.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/ggiiufqnv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gncnfpynr.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.tarul.cn/Article/details/gkuzyykof.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/gvcvmwksk.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gjispcsnm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gfjilqcwq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gaxskizet.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gouywqrri.sHtML

Go:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gzotsncpw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gtsghchhz.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gtwddnzxc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gbefbeqjr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fktsv.cn/Article/details/gojfjpjag.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gwamjeusy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.yfazqb.com/Article/details/gkjsvykpl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gyvxuveru.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gztleosnd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gtaoahsqq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.bbcook.cn/Article/details/gzpicsdnf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/ghkfoclmx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcjprgxxs.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/gprkzdcmi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzgfwkxfu.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gsyifleiu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gpnsrimpy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gdraijxxy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gqxjlhefq.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/gigcclmba.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/geqnhhgvw.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gtuhftbvs.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/glmgjwpvd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.sjlbkw.cn/Article/details/gubtbutxz.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/gdkbjptzn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gbzawciya.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gwzxfyuex.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/glskglxiz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gfbvobcfn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/gslrepetu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gzjzgdbpq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/gybxbjicd.sHtML


<!-- 参考信息 -->