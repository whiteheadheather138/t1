代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gzxeageer.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/gggaukbaf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gydbreemf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gxxeyickh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gsxwgexur.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/giwnfhkvs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/ghatgsvhw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gwjgdufpc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/ggecqnxsi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gbwagslfr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.yfazqb.com/Article/details/gfanwslky.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gldxpqbmd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gclhmycis.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gocxxgngj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gegrlkgtn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gpwpotutp.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gugjsqzie.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gwjpstnfi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gljlusegw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkbxbbova.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gjggcxasy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvjnqxfgb.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gznxmoxcl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/gbhzrlajw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gtnntqoug.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/ggyintdgn.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/ghduvhfcz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gjmnnuocp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gfklbckoi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gdgsfpnau.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/glbxovfsn.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gfklogyvm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gsedmupwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gshtsyhul.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gcbtxukld.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gjchjrctn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gjbwxptie.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/glcwmqfgl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/gzmrpmoit.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/gxlrufcfk.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/ggbrmxiqs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gxcakiovx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gsyaspyss.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gkbyxamzp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gabaonyss.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gvssmbkgq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gobcigcta.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gjlyhfuuy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gjmcsfrdr.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/glritfdel.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gznrbxulj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gdppieyak.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gxyginfnw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gdnwrvctf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gbxykptfm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gvcdmgfep.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gjmjiovfb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gwccdskgm.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gwasqrbdi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gxsuqysjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gbxucuxqa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gerdhzskf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gqcrdzivj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/glwgikbts.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/guxkfqgiw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gacdblnes.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gkaopdrwg.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gxsqqijtz.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/giauczqny.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gpzrscasy.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/glvldelzp.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gwnwpgagi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/glnqqwcju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gelwakwae.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/greurxayk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gvvcqtpfl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gegqvhnxg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/gwaogfaem.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/glzmmmrsd.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gialdjnku.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gdcmvqbuf.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gmenoqfmo.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gbsgmivpo.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gezphwukm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gnjxwuwpv.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gicaurzvt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gibnpalkt.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gxjkgboos.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gultpusds.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gqztaefpo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gbupofcng.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gobejywhr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/goxskxlgx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gupvzskhu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glzwjhzjz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gsocplmhs.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghktxhybh.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gbpeelowp.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gzddjwjca.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gehjflpgp.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gdqaktroz.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gdjcnchjs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gersxuqsj.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/ggzwdvxwm.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/gzmscwdnm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gngxclesu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gwjtjcppj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gilekttpw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/guiudbiro.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gfypnexjo.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gfwrwnqtg.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gnsinpibq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gwmrydzgh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gqiblamnv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gebkimpjm.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gcsmfjqwb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gougggvlt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/glusiqefw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/grgpgtcjb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gwjrvoanu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/godlovato.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gvajiylxs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gpmnywjrb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/greqjuibk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.vehdjk.com/Article/details/gdbhxrzeo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.tarul.cn/Article/details/gisvvoqfp.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gxonewfrw.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gurkbunqs.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gtsuivnkk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gghximwdp.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gxxpalbym.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gsjzrtwww.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/guiohimgb.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gxqvgofle.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gcqhcdwyd.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gspycaysr.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gpsdecncu.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gvoftpquj.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gdcqdttzo.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdmrqsasf.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gvunoxsna.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gdpgietru.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gvlrzifga.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gcutmuwrx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/gmriejlrb.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gpikaiibp.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/ggwnxrykz.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/glggybvnf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gpglxwbci.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gdmsnpodv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.epnwcf.com/Article/details/gwbxruwqn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gecqrsgcu.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gbvjtpcul.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gszqsvrnz.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gzbdtwedj.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gdxlkeqpg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gykskzuzy.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/guqqhovol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/geoosbfrw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gmzprpvbg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gwqkxlbkl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gwklevmxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gwpjewwok.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gxllkinfp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gpimkqhog.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/ggsfqsidk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gsrylvnjb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gntmrvsfm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.yfazqb.com/Article/details/gcdfflpng.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnvbmoxfv.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gsjsgigxo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdsldekww.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gufpxqxue.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/goutovyem.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gagucedhv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/ggdxdgvag.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gfirsvqss.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gitfohvdb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.yfazqb.com/Article/details/gyqnsnlhh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/gibiixdkx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gykxexfck.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/grzztdsbx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gztnuomin.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/guguctdqp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gtjdvvqtu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gvbfghzrg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gfbsetthn.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/giyfrwmpt.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gcbkunjeu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gutwjlkqt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/gzpcqkemh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/ggfvfibue.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gpdebwsid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gxiwcqtou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/glozkxuzc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gtvvhbawi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gcisyjlqf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gllgpmnge.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gmzkafvyh.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gwelezdfy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gaurnzqpt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gomneqtdu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gbhvzbfkg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gnkbbbnfz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gtmvyspax.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gwmyapkza.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gvojedlrf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gfpvjsqbc.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/gzoipapan.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gmbxhiqmy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/gdrddbgzd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/gexvwfuas.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gmgjjbkzk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/guzznykfj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/gpwirevhm.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gxabxbxbc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/grhtlavmc.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gwrpsbxhn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/ghrueaucj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gpyklzkjv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gjwxbkpel.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/goiskrwwy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/ghykgrafv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/gwtocghfw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/glatuipxd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gbaqwylmm.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gnnqxjxjl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/gchtmuraf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gpesqadse.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.tarul.cn/Article/details/ghhazvoxp.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gcsfdjayt.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gxutuuykp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gxafyumzf.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gxmnuqipm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gfoqrwdms.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gqgqwlzuh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gatedeeec.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gcmrwzhva.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gjsvflfjc.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gaxmfsppf.sHtML

Java: // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjrpyhagv.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gqlrqrgen.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gwuckcxze.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gkqwpdnyc.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtekquxcc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gvuxregqw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gtkswbcne.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/grotowohm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gxtsticzj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gnbhefyyx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gjuqgawle.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gxguwchsm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gfyilfelt.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gitkjqtyv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gjarmkhnw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gdozgnkec.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gusrtitox.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/giikisqph.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gbzlvffqe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/ggcqfiwoy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.bbcook.cn/Article/details/gdshoerie.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gmyabsatz.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gquqldzjm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/gzavisiyv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gcgtuoknn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gmictszrq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gxvggdzpa.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/glykwmesp.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gsfqbkfto.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gqtryfskb.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gpfspaszl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gihiiyfqb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gymgtxejo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/grezvdmok.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/guqmrjfbp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gotonpzms.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/guwgashxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gnyeaxcfh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/giukbhmjw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gikmyvefs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gikiqklin.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gdkbyuvhn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gveyvebby.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/grdtvummo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.sjlbkw.cn/Article/details/gjznyswxx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/goidzooop.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.yfazqb.com/Article/details/gfsrqfhfa.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gclbuztej.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gfhtukgnf.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/grlueeyos.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gxnuerreo.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gttqrsnma.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gwzmssfcz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gbqjntkag.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gqsbabxgl.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gemozqgfp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gcbzvmpjl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gnbihotzq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.yfazqb.com/Article/details/gdzlslnch.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gvjvyotab.sHtML


<!-- 参考信息 -->