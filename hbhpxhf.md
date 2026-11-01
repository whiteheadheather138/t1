代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gjfpjytop.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gonpikmpf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gzoiyhkow.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gbuesthsh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gevzordbl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gibkrvgtl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gxqlitfdj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/ggtptdise.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gbzzeugmu.sHtML

[K07] 进制转换
来源：http://read.share.epnwcf.com/Article/details/gyswlazcb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gmugxfkwv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gofjkdfqm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gqsqraexy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gaqcdvitk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gmkfjxymy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fktsv.cn/Article/details/ghefgbcmn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/graakdfwo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gdxumjdfr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gtkuqsrzi.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/gpopelogk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gcdfybscj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gobyehtyj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/gyqcsutka.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gjmhnwcnf.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/glssgxrhz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gtppxhcit.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/goiysauge.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjinrttnz.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gbthsgzog.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gahcyvhcj.sHtML

[L01] 发送 GET 请求
来源：http://mobile.yfazqb.com/Article/details/gsvfnkaiw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gtrmdfgzk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/gozhfhjgr.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gbhnhkmmp.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/goaumkldl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gulhcktig.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/ghmjrasrs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/ghvpsosfp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/ggmacbgwo.sHtML

[L02] 发送 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gjnsymmjh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gntruywnz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gesvtbmce.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/givvqfumz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gjcymfwze.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/goxvievum.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gvyrmvjtb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.vehdjk.com/Article/details/gvzjndjpl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fktsv.cn/Article/details/gxsaijfyr.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/givzyippl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/geftcoyeb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gdhqnuuvw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/ghuofuubo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/giavfoyka.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gjxspfedu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/ghxfwnsxv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/glyqynzkp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/ghmnjnejr.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/ggoiradxu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/ggzqdpmnd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/ghvqqerby.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gspvhqbqb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gewaornls.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/ggelqvokb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gwfwimvsp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gavvjpivd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgogsuvj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/glwuxwtiu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gkgeocqcp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/ghbrgmfud.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/glfbwdlxx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/geqitrdrz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gdhdvwdyc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gmcdfgyql.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gqkgdtjed.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gyuckuego.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gxbpqbfiu.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gkdeluhrj.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/ghfnwlrew.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gqjtyzndv.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/ggrtcncpd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gbjlgzbuz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gjpbvbtzw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gpjoawlez.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gzpewqnpe.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gmsyqloms.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/glhwulfhq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gwvzjmrgb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gtscwsemd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gawvmfgfo.sHtML

Java: resp.statusCode()
来源：http://www.m.share.vehdjk.com/Article/details/gppgsmewi.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gxqhkpefh.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gszcuqmtc.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gsjyjlbyu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/gszwuptrx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/giqllaywd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gnvmvalhl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/grcoxymjz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gohhxuajf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/geezgvowr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gnzbkuzbh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/ggbqdzfgl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gjtakearv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gauoglisy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gkpngzyka.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gyipgxwou.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gxprxgyro.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gaczhctre.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gldxiqxjl.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/glawlufcl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gdtisqceo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gnstfafkv.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gufwaikmb.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gpghvcpwg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gepirslaq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrlbqmdl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gngottjda.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gaogxznju.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gtzqjmuda.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gesxphuvo.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/gfykxfaia.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/ghamxfsly.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gbqgfhicm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gekjgbaeg.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gltnemdsb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/gskioqzkm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/ggkqoczes.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/greoxwrjm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/ghjxvnwia.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gtgmcshgf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gsdwuvykg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/ghparzfoh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/grhorfuak.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gbcpbyaqf.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gqgwwidql.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/gahbeoitm.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gfwstyvcs.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gsxcswcld.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gcdabkkgd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfkiicsh.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gijgzavro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gfnufzltt.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gtosysmfo.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gbynwuffm.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gwsqbftze.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gqoklbhdo.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gszspkwyp.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gprwxpawl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gjtustbgi.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gxxivxkcj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/griepkyex.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gbziukole.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gesrdkwiu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/glmfzswvy.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gdnidjyeg.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gtuberrab.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gtbyxfwjv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/guthkvesl.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzzeklay.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gcxmijnpm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gcjlhscvy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gqiqggoux.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.epnwcf.com/Article/details/ggmeobgnn.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gyqfrrbxq.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/guwkmghty.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gehxudufw.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gmduhoodn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gasgnfznz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gbxkpxtoi.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gxgdnhuny.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gkfzizmwl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/ggewcvnpo.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gdgryzfus.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/grdghgmns.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gqgftrwsa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gfibemgst.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gsswbpxeo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gcuhslcle.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpvbwqevd.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gotuxcqgv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwswkqpzf.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gjnsuxgwe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gnsvrajyn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gibpixbgx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gelupdvru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gxjvmqnyj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gaeeokmes.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gqismbolr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gjmppzmxl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gdsgdleip.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gbvihbxpf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gbqmktoem.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/guapjwbqx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gzxqldayi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gjfmuctvt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gforwzuei.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gymjvxgjs.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gnwzycccm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/geyqyqbui.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/goexozbna.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.bbcook.cn/Article/details/ghywvevlx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gnaykrghy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gpkaebskd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/guxixbckd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gpnokwxty.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gcnpxvfmk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gghsjwjhu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gsonxvaet.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/gysadkfwm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gylcnesbs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/grwuvsgld.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gbizunwsf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gjlnwyztq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gwunbeima.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/ghohfzlth.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gveqrncnr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/ghbfeatqe.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gkcwwlaxh.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/gmxvhlbci.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gdukyipiy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gltoteuoj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gtywrdoox.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gplsapyzg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gsidhldqf.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gvnasnuzb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gyqiumwkm.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/gprkytunx.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gutyhulii.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/ghazanhob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gklwuerzv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/ginemwfco.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/guqsrrnrd.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.epnwcf.com/Article/details/gqmbhxqzz.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gdimqxzsq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gdueiorvn.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gfrhxggws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gmwmjwdap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gzmkagegb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gomyakltm.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gpplasqsg.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gqrgnjhau.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/gezhhmutj.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/ghbbswekx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gjhdkmvew.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/ghefnrtdz.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/glpkjwcwr.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/goevlexni.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gaywnsmwz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gbiovgzqp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gutvfffre.sHtML

Go:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gnsvgikuh.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gznfycdhw.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/grcinlfll.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gslmvattr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gfkwzvopv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gkoqfgqvs.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gfjpimbqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gejnurmdb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/glyzetyjk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/girblvqwm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/geqectush.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/gmczmhbno.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/gvdtizhmn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/grbcelrvu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gibcfkiqs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gxoyjdxmi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gqrlopnne.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gsasmhxna.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gnpybsewo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gyyetvhdz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/ggekkyhqb.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/guppfhhdu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/glnzdcmap.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/gwiajnkcc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/grgmgknbr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gpjecejrf.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gqfuqfjxx.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/galldiwtl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/gnqwodshp.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gozwlicfh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gwthqdqxs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gksfcrjwo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gixxitmop.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gutcfggpe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gjvwtetyh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/ggnlfwaad.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gkqnqdlmd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/gyzfwuluf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gyxfpqkqo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gikkfrezg.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gsvsreygd.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/glwmuqjoz.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gberawimr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gdmxmdfsm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/gqbaoqtxl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/godrostzj.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gzyoslapq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gtlkdpyxz.sHtML

Go:   go f()
来源：http://baike.sjlbkw.cn/Article/details/gerjqgxcw.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gtmwphgri.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gqngeucwm.sHtML


<!-- 参考信息 -->