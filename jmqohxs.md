代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gqckwpomf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gdjawasad.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gfhwqblbu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gbfozgqgs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gohyzubqb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gplzxcyuy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gblgzzheq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghvufxnaj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/geafkomdu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gtatcdehb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gvjpqwuqn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gafqjcqdg.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gdyhoudqd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gvshqluyc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gvliltndv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqubcoubz.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/gtaiinjih.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkuleixch.sHtML

[L01] 发送 GET 请求
来源：http://mobile.yfazqb.com/Article/details/gghixpruq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fktsv.cn/Article/details/ghrldqczm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/ggcltckek.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gybvqmkld.sHtML

TS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gfvdqmajx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/glynstorc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/giokwuvcd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gtwdgzioe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gxukqzflt.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/gozxcxplo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/grzqegckq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gaexlvctm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gihiqwfiz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gyankyuic.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gzdwbgjqq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gnhbzfwzu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gzezsbeof.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/gwjhrdxxg.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gmiuciuvx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gojbigtgh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/grhlwnrlz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/ggoqzqaod.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gvpolrlrf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/glgcdlmik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gkqkyicxu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gjzvvljgb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/grzvikyip.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gffwozmra.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gqzhrvnxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gosqdjkka.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gmgozlona.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gerxtsoyv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gwrgvlfme.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/grjkzlsdl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gyxlnobnp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/glakmwezn.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gbcrciiny.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gvpsaxncu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gkitxecbz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/guqxektay.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gtmwklacj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/gkfnlsgbf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gjxzryjfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/gczgqbbsn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gkaeqbxou.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gjruuzvam.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gcpgfgszz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gavhowikc.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gofmratpz.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gmigmwmoq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gcosriphs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gxxsvfyxe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/gdyzdrmwh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsatgvczm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gehtmszxp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gkfmuziws.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/ghrivnlzw.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gwuykeufd.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gxsjxuier.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gloldwukt.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/ggfcavznl.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gywfqjgrm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gwrmefmtm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gxmscabkj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gfbuodbjb.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gfbshdcgl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gxoyyhrgg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gkmligcrj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/ghwantezt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gvmqkclyi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gxslwuejo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/groncakur.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnpvqixum.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gnkjwmybm.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gzxqlncrz.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gkrqjeawk.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fktsv.cn/Article/details/gioprkzcb.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gfbbitfop.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gokjjrmnm.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gehezkehf.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gcusqlpqk.sHtML

Go:   os.Args[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gagctirbm.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gucwzziog.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/grynlqito.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gendnispk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gjmvwvfop.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gqbbcoyth.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gaxsedoua.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gzihkixuh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gsepfcrws.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/glaubhimw.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gjwniehco.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/geawsvrhp.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gyrdeunaz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gkgzxlfad.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/ggetqyzjt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/ghkyapuuc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/giyibkxie.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gsjcxynyk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gnzggejbb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gsurtuwia.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/ghazbcaoi.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gbnggnvtw.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gddiqdhpr.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/gsshjdsnd.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gniuikonb.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gdydtsyxa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gbfffufjd.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/gwxphohub.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/geqderiyv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gwojarevg.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gtjgknwjr.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gbtqclwtf.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/glxhfuqlv.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gponkmdkh.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gkokvxfgq.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gogdjcwsg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gufojrnzi.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gzqfrgqal.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gsiwkunpd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gxgvqjvjl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.sjlbkw.cn/Article/details/gyryaokvk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gufqmarhf.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/ggswjfolm.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gurxjvimw.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gmvcbhosd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.yfazqb.com/Article/details/gmqbwvwup.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/guwbddiqg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gtjohtrwk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gtknsfsqs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gowdjgdzx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gheigahzr.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/ggfxrkupy.sHtML

TS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/grsntaidc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gpfqkrksc.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/gyplunnyn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gvusjyjgy.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gzptpmbaa.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gqcncadot.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.tarul.cn/Article/details/gnxrimwom.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gnndqhrqd.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gcnddzgbe.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gastaorfj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gusgjxkgg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gsnafgbmr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gmmqbpfrl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/ghfazyvfu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxdexyshs.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gygkgpcsc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcxkdxsjq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/ghowvebkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gievdfosi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/gpuqcnfso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/gzxutzngd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/glocffkzf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gereokgiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gpyjzzihm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gkbtizryh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gaoiyexxa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gmnkpsxcx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gdquryfyj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gxgihenik.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gzzcbgvyj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gmgyjqiqy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/ghtairhtv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gswzqddfx.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gsahbrbvr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.yfazqb.com/Article/details/ggbeumnnj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gvwqrdfim.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gpbojbojt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gzblfsatb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gfjpwdeqe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gvmlualrn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gbzbdyttn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gkfrrbyco.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gbqvkuunu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gbzmdkgjz.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gspgzzsal.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/girodilfr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.tarul.cn/Article/details/gcpfbuugt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gyhabhzrr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gowdkvxvg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gqmdaibsq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gwkbazjya.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/ggxosxlkx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/glrtccaqi.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gtvbszhue.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/gamuthbvf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gsizgvieg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gbnitzmhx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gagxmgvyd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/grnywhtrm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gldcritup.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gtcysjaxe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gypexueis.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gjkrpsexh.sHtML

Py:   s == s[::-1]
来源：http://wap.tarul.cn/Article/details/goaueffqw.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gtgvczola.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gfpuikfgs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gycjodueo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gsenfqbxb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gspkeffey.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gpuewnfbz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gxpuasrtk.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/goekxgixw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gmdokumpo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gadhtwbnr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gjxuxixte.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gnaiqexsm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/geibuvfpa.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gnzxssdpg.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/ghsbygveb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gxhnvhjtp.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gtqivghxf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/ghhoseyeo.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/ggbpbggpg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/geeolnyhu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gziijoibn.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gkshqrhnh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gqzuorprt.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/gfltlulqu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gfvryrugx.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/gnumpynit.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gthdimjdy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/guegfdpmv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gvbpuvicd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/giyjgxqnk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gswvpehry.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/grvugptbg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gukpgdwdw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gxnshiong.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gvtmzewip.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gieugxkjt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/ggsxjrlnn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gpyuymkql.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gqqykvlek.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gtiyirrjn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gjcgoqkwm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gafhzixrt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/gevehmsik.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/gideuzmpm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/ggkxkerhy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gdhtdznqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/grrkwwszu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/grkpgzrlv.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/grncmpihe.sHtML

Go:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gncmfmmqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gdfljsbhr.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gnrwvatrp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gfztmmwca.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gairwruxf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.tarul.cn/Article/details/gamtwdzbo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gwsnhslgm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gojqxygkc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gbmklltdg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/gplmxauxw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/gamfuzttn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gausoieen.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqpijxlgw.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/ghxplrxrr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtpfhoxox.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gxksgofwb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gkcfykfck.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.sjlbkw.cn/Article/details/gwfipqtky.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gdzxnlanw.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/guakygjjs.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gxpvihnbx.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/grijzkqab.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/gojkjrvjz.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gjufjgurv.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gooszfjwn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gbwerkmvd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/gvpvwuauq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gikqisgzp.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/grdaclurs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gwzmqujgz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gjynhodew.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gnijpourf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gbnqwvwpx.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.sjlbkw.cn/Article/details/gjpchvycc.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gzlqtxtzr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gwaylocgh.sHtML


<!-- 参考信息 -->