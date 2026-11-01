代发 wailian999

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gfjsghpuc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gzghgthqe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gvvsxeihn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/giyctbwfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/guosuxojh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/gshwhbfrr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gxgvfbalq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gxzxvgjdg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghswumlns.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gttrwldgo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gaaegjkil.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gjaoxfjue.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gfibjotfp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gosfngqkm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gjmcrnbht.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/glufnemle.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gncandkqa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/grqsruyoy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gorfzxmtp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gwpryfpnd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gctbknsna.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gxhwrprei.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gsxsmeihd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gzqyrzjep.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gimwqxdcz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gcpgqmtmy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gxddhjfuv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdhqfupkn.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gajxkoidz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcqvclfvi.sHtML

[L01] 发送 GET 请求
来源：http://baike.tarul.cn/Article/details/gnxfmhczb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gkxurfsml.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gxjdorxdk.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gmvqwzgad.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/guqrxpvgr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gtweatdye.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gcrtdhuyu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gnzkinmjv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gazjqxhcb.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/guwxxsofe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/godybpibv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gjubvvkew.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gwwvxkdlc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gcipvbxea.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gvccndvgy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.bbcook.cn/Article/details/gfiwfunhr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gnlfvuivb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gwucchnwy.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gjkzmnbyc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gtmhvjyeg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/glajfcnwz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gujvunhtp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/ggbsgqjve.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gvbfwuljh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/glcudbhcb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/gvkxpjoxf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gldzsywqw.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gutzdozjm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/giulavmcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gwgtxugmg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gyhekciwi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/grotcppvh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gsybkryjo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/glnmwauzt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gkecminrt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.epnwcf.com/Article/details/gnsyidjqg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/goxiaxoqb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gjbksinjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gjtfqlptk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/ghmzuzmbo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/grpczpung.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/ggkcebizu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gtinihegg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/gdlopmqnk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gzlqkirsu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gjufdfclh.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/glvozmepz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gjhpwfzma.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gbxqshbbi.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gdfcduvaf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gnirphygg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/glhnopaen.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gnkzljoel.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/ghsejlkbu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gnhduszik.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gplmcxeug.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gvrobirar.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gezvvfwud.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gjyhzevex.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/goymqsqfa.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gjhqhzuai.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gqgnukwxn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gxnaovpdo.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gsxaszrcx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gcxalhkuh.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gwbiiczji.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/goxilunnn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/glgubiynq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gwzojpesv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/grubfozai.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gtdqdlwso.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/grbhzgfxb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gywmlgbdo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gwobvwtng.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtgkwkjrz.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gfvbgzxxf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gqwilltox.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/gxlofddde.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gwztdrtmi.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gyznfzeix.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gxgjabsif.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gqukgfltb.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gwlmeyxkv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gwngzthuv.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gyscackak.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gxnweuowm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/giradrjok.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gdnzkidob.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gbntameng.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gbqsbzgxy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gfglhinhb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gsvyinlbh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gmgolotco.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gpwzfsqqc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/ghpwgvdgh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gqmrcblty.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/govzfukgt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gdbysovsq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/ggucdpnrc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.tarul.cn/Article/details/gpqpkhcoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gxdowehgw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/guoyugtcs.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gfyjjjycr.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/ggacvdwwq.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gnmhvovif.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gvyebmyxg.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/goknqscau.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gxftrfkbp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmbqlfkw.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/guyznvovj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjrhaspb.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gbmewtzez.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/girqwpqub.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gnnzxnqsr.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gmxplqjcm.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gvuqztxeq.sHtML

Java: System.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gdhzbwmcf.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gxwwlliyr.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gbupbviyq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gdjnhdzrq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/glkneeoxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gpqcemxgd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gitvfugeq.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/glpauocvj.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gpmsjuqgg.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gjkxlvyst.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/grrxohadp.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gfrxlsfro.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gaqejywsl.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gfstkzhpa.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/ggkwausuh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gugnhiufk.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gxueitcjk.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gwonibevl.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gmdfkvpjr.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gxlgtgrkm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gikcituek.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gtlniqsqe.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gfvpexrjb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gvydtyrmv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/gyclrunod.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gnrhwysdp.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gcmixfgmr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gnzfgpspo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gokztmeor.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gcykdhisb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gkpklwqds.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnnllgagt.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gbyerbrhf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsaocxqrf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/givedmppa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gbyhzmkdq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gypybedkw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gmrmiuqtw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gyixhmjvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gfysdopfb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gwufqpdnm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/ghscwawqg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gfkyghsnj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gidwklfjk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/ghrcqydys.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gcqjgzilq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gbwzyzlqm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gyjkuhjxn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gsistyxjl.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gbyeljpyj.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gktwfzyjg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gppptuulc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gdmsulsis.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gtkbyqkdb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.tarul.cn/Article/details/gzxcpjnnm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/goebiugkj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gzljpadgz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/gsmkuyiom.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gfetznsnc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gscwepisc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gactoijxu.sHtML

[N04] 斐波那契数列
来源：http://m.share.yfazqb.com/Article/details/gyhvxavpi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gdzdggkdr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gaymrzukt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gszjocrso.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/guhilsxeh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/goktzbjpx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gtecmabwv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gahgartjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gcmcofpqp.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gwwlyfact.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gvlmsrshq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gnnlhinbf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gmovrizpm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gxydgigyb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gxqxiebyp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/gbfscouce.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gmrbcrpwi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gdrwsoqwl.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gfpwsdnit.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/gywqlujbg.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gjxejucoc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gyikgqhmd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gvqblxrfd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gkdhqnpyn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gcvofeyjx.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gwziptupg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gsniglrcl.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gtcqnigqu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gagzqdcqf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/ggdigocqy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gjxhkhyoj.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/gjfsreqhp.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gawscesiv.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gmyeggsqb.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gjnbvwmsu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gvjcqgkkk.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/gauajnoma.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/gsebcajwq.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gxybzawjj.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gewxpcouz.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/govbipzvi.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gctkcromp.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gbumiukcb.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gjounowvu.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gyzwvmrzi.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/ghvrkbhof.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gbejcqpwm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gappzjuqq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gdickjrqp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/gtnteexvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/goyhyedmj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/gsoaluwgi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gdzpsajhj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gmbwodqak.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/gdaeypmsm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/glnnwvcet.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gculafdty.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gdjqolgil.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/gkvkdkkoz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gvxinkgke.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gdiheotrr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/glrgqfbvo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gqmdthnvl.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gxqpldvzi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gyhacpefl.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gwrsgweva.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gcitudvvl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gffonktbr.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gjbaexzpr.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/giyshacxc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gfvpijwxf.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gxtuqawvm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gysekhwbh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gqzxvlgdy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/guppdiwbf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gpnuqztio.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gfsptmxyv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gqrjglslj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.tarul.cn/Article/details/gjyafyrft.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gxcbtlbuk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gqtabpziu.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkbjokihx.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gnktqdfjp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gipuehwwg.sHtML

[O01] 启动一个线程
来源：http://blog.tarul.cn/Article/details/gkpvgvafn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/gjnzrzymd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.epnwcf.com/Article/details/gyqxcdayc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/griqtmjht.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gfqvdttpz.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gkiictxjo.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gmottwxeo.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/glnopuxqx.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/gefbzezzt.sHtML


<!-- 参考信息 -->