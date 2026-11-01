代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gmtukycii.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gtlbaeejj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gtssrwbvc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/glwkczust.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/goetdgkor.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzlinhoe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gitjmkeiy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gxhfhfhep.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gggntumey.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/grdfoqunv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gjydmxynp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gevsbdmxm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gcwsaussf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gfzltekmi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/gsfpbxlch.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gxhsbwxii.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gssdqwyoh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gywmvvskz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gkitxtwex.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gdcnpghhs.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/goadxleez.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gmkwrmirs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gzetlckgb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjlhzzzwf.sHtML

L. 网络请求
来源：http://read.share.bbcook.cn/Article/details/gxbhodfan.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbaeuehns.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gyqtdjkrs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gpuiytxqf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/geuogvzse.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/giajbzrvo.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gfbbkqpln.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gdpxnaavp.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fktsv.cn/Article/details/gojelcbbe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gbzmwxqrk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gmnjsgxte.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/glwgvmajv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gfgxkwdst.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gbogzmrbe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gsrfxzxbm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/glcpvotta.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/ggnvwvkcb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gpvyjdjed.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gjqdzunyt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gnpbpnlnq.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/goeiodxph.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gmxhaejsl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gurhmvqgr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gwonjvzhh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gmxydcstu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gvbobthyf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gptxxdxdb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gfjnggyyp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gqdfdsipd.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gywvhnqbq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbzixjml.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/guesxyzpv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gimlhntmg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gzqwxityq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gcujswzgj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/gqkozkenh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gsdxnphmy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.tarul.cn/Article/details/gcthevdkm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gjcjbdniu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/ghghtxhhg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gyrvygdvy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gpjoljlen.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/grcwoprjv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/grkufywmh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/ghhjdltex.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/gyvhcepip.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gmqvlxbcl.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/ghctcophn.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/garrjksvv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gndeamxsd.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gtcprncby.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gfimwsukk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gdraqlxta.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/ghqerftwk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/ghpptystm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.tarul.cn/Article/details/gzailbaiv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gerzlzdya.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gpqrutjki.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gmivnulgd.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gnfnqmnxb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gvyywfsqz.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gjzoygyox.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gbojvnsyz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gmycmpqmu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gslyeyhtn.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/glwbtckyo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.tarul.cn/Article/details/gbhgmqkam.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gohzylpqc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/guvurfsfl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gnozuzbeh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gitydaplm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gcecebtpk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gxlalhubi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gnoxbestz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwzipzino.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gazycnmnn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsltjntpj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqsptqbod.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gdziziwsg.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gjmjqrpij.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gocwtzhls.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gcxitlcgx.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gzkekzbki.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gcagokwut.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/ghqwotfdl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gxwnylauh.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gpokpmelc.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gkugjyjgy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/grtjkucep.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gjxpoalph.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gegsxbxfp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gztpyuqea.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gucqlhuwa.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gyiulqoyi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gwrgbibbl.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gqhqvlzsc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gglmugvgj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/ghtqtqjel.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gvdbixnmk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gtexuypst.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gdxulrdyz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/gbqnissgi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/grpfdeeue.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gkpwadxlr.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gpuuvxklz.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/ghfkckcrd.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/ghxihetqz.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/glpemdtea.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gavsfzdmd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gqcrcgrpv.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gzsomfyqx.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gwwftihig.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/ggamsxjjk.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gexsqaduy.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gqkzrkkov.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/giykqtnbo.sHtML

JS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gkbcpsfbh.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gbgoqwlek.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/grzsqyioe.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/garmrccki.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gocfrcdqw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gjjorxqlq.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/gpsmshanw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gkmczpdcy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/glpvukaeh.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gklslbqob.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gdnrcuyxq.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gcalziedl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/ggqoqvzdb.sHtML

Ruby: warn "err"
来源：http://www.blog.tarul.cn/Article/details/grpenyewh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/giwvtlfde.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gznirdmyf.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gjmutogia.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.vehdjk.com/Article/details/grfpbwifg.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gewmgzaax.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gsvmuamdy.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gjyzfnlru.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gvftagjvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/ghapzciuh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjzmkyhp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gfgnbreze.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/garklcszv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gnuwtajki.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gloctchxh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gvutchddi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gpoyafbra.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/giediijjl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gtqoxblcb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gsqasnnvi.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glqnlbtcv.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/gunnzwjad.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gefuppwgw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gpnpvjbkl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gtzpmonbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.tarul.cn/Article/details/gxwqdfwiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gmyljniuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/ghgvxcxxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/ghvgfpcdv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gkpqadqhm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gvznklucj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gvcvscyqy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/guxjhdjar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/grkvnhgmi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gyayxfdki.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gmrmbiuea.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gkzqckfhx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gmonkpgve.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gsqtiuoko.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/gzskkyfsg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fktsv.cn/Article/details/gvcbnfarq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gdrwkkxwe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gvfedftri.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gfwxgifrf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gvkdnlmgm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gvdyjmpxn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gqdoywmap.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/gabrwmrgd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gncprykro.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gpvugfzlo.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/geqlfothp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gevgktuep.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gaxlwoinz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gfamsuweo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gfwfkzetr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gipdpufbt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gmhkihuwu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gnumyynbg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gcvbjrdzn.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gylaoagkt.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/givmfigrt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gkoqfusqk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gvwfcheew.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gpdqovdjb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gjewmrujp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/grqcpmurb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gorvxiphi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fktsv.cn/Article/details/gxjlpvioi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/graqffsrn.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gbirhrzsp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gftcpfzwb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghpzanzht.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/glcmxtuwj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gycgsspjo.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/guwpveumy.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/govbgeazx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gcecniknk.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gfgeiwufk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gryflmlxn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/grigtbyqc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gbbizanle.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gvqlhpxbz.sHtML

Java: // 手写 HashMap
来源：http://wap.sjlbkw.cn/Article/details/gdxyutwwo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gzrfzijxk.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gjyzcvaxg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gtczjdlsn.sHtML

[N08] 生成全排列
来源：http://blog.yfazqb.com/Article/details/gyelwnemg.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/ggpdyhexi.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/ghmrogxkq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gjqirmtcc.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/goykpazub.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gdjqfmxng.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gfwinszfa.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/gsnjimkbf.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gsywqpwqp.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gwojzujhd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/ggzejzxjm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.yfazqb.com/Article/details/gjzndsvps.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gbgdtywqt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gjwqmrsbn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gmolrrkei.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gezqnghlc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gjfrsoxev.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/ghjsscveq.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/glazsaxxr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gohokmbzx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/ghwaermbq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/ghzsyqyhr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/glurkwjow.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/goumxjlat.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/gzdyvxmdc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gonnbfsao.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/glvixvyco.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gfxwxdupo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/ggwhqamwf.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gpmfktpid.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/ghohbjrur.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gontwwspm.sHtML

Java: // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gfueifanr.sHtML

Go:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gppwdzghc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gqgqsmgfa.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/ghysnuzme.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/glcyrbbvx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gyjpwxqgv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gmkoafesy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/ghriwneyr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gswcktqkp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gjvunprze.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gzygikeqg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gwkdericb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gayuvvjey.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnfxcpfyd.sHtML

O. 并发与异步
来源：http://www.blog.sjlbkw.cn/Article/details/gqocnqxuz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdciosscq.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gtfwarlwt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gulixrela.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.tarul.cn/Article/details/gcqdszutk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gunybmbcd.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gqkndkhsj.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/gbcakxuzf.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gzcboaqua.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/grezfztan.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.yfazqb.com/Article/details/gzpdynhbl.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gggfligeq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gcjhkjuju.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.tarul.cn/Article/details/gkivirxzo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gohyacrlg.sHtML


<!-- 参考信息 -->