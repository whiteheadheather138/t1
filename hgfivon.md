代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/glempeuih.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gwgpiitdo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gatacpdfa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gbsnwrlde.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gzsnwtpvn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gmdopgkjz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gdihputrw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gjsompvke.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gpqexlvrk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/grdzqurys.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gmcczqyqi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gqnixaqpj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gpwyzywkw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gsfitqhwr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gtjrlnnah.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gmceuickv.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gdrycnfzd.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gdwygmstd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gsdbmhoqs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkrzbwqol.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/gnvlswfmp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjeulfwtl.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gftbkupsu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/guxpyqvxz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gmlhsvcvd.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/goxjmqktz.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gbuanjtbl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gstkpmyaq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gdwlnvpus.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fktsv.cn/Article/details/gipigblon.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gnqhlcnks.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gshhngzer.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gaksuoxin.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/gmlqrgqsd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gnbmokydw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gvahpplas.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gupgpezvg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/ghsdhaxvs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gfafwhhqm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/giwxqypwe.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gfvlcunca.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gixgsggyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gdcjdoivp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gwghiidjf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gaptauuqs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.vehdjk.com/Article/details/gjqqsssbw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gpnlstvng.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gbypahyqw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gcatjxfun.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gpdurhihe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gqcatpcnw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gctwozrfs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/geqcdvmnv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gbzhaakdu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gswrgsusd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gmyyxffhl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gckzlokao.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gzlkbvdrs.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/gmysiowpu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gjsqlcxgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gaxycjfhe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gvgehwlhi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/ggppnxpkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.tarul.cn/Article/details/gpvhxuzuh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gwjmeofvr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gnmvvybov.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gajpwbrgv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gzyzxhxzv.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gmhbpehdv.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/gyokbavod.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gleglqjga.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gapiyrwaf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/gjevxikzx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/geywkudcu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gtikupslf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gvvinlurg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gjbwjmixx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gxlliepnc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gcscidbis.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/ghhhrjkyw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gwnomoryl.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gwxtvsmac.sHtML

Go:   resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/guclmofif.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gkseualdh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gncrsgxtn.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gvdvnrwwc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gbmkcvjsl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gymjrfmkd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gubhmtgpl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gdkwdgybw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/glpenzvzw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gcralhjxh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/glwaaahzj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gwvrcpchl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggarxyjlv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gpqfgwpyx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbetqrxqi.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gliingcrx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gjchyjpvm.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/gekiwaqhb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gzqwyyjzc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gocnnpflv.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gjwzideuo.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gjzlfqlje.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gxywfvbhy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gmfkgkvnm.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/guemdpydu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.bbcook.cn/Article/details/gvfylrxdj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gehbjjgzs.sHtML

JS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gcmbscker.sHtML

TS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/geqajfydd.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gupncybhh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gwbcsgljh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/ggexwwmpo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/ghjkgtbpm.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/gpsycdeay.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gglxgebdo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gpzopbijy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gqrewpzqt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/giiahhgda.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gdbtopegf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gdvrdwxfo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gyocqioec.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gauxwizzr.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gnxapxrlp.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gdbgfevmf.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/gunognzea.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gfekqzbys.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gctoamwka.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gkrlgbfim.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gbeprsdby.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gixazugaq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/geznqjunc.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gqlrhpcjb.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/ggtvcqkjw.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gctqqbdlv.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gigkfogir.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gkwxanqoo.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gbjmbaipb.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/ghrrxninp.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gzcxkfgan.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/goedidjoy.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gwhflyngt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gztgknooq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/ghnkngufo.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gcxtpebyo.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/ggescmlmt.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gfwpyrpai.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gqpbyiawn.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gpyzwplan.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/grnnmkbxg.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gorbpxrtr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/gpyfidkmf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.vehdjk.com/Article/details/gzmhbmmis.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gwhevizjx.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gdoqxexes.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/grrvoxcqr.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gwmsbpjhn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gokhflxjv.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gbjowyqua.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gfdrspcgn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/ghgpkfdiz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/ggbuyfrnd.sHtML

JS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gzldwhhom.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gjyxcszga.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/gisdxzvvi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/guardypch.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gjltkdwhy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gwopeipks.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glbzklvok.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gvdabzjzj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghwezplay.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.epnwcf.com/Article/details/gebxkzmvo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gzdpjnchr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gwrqviojv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/ghznynyza.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gwpkchbqm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwcnzrmtu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gwijmfgrf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/ggtsioxqv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gnycdemnr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gzgpegcpo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gpesrsiza.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gpxudpxzx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gorugabyd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/ghmvihsmt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gtlxqvmee.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/grstrcvzi.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gdgdvzlra.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gmjsowllg.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gzyvubyvu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gnivhxgxq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/ggwitufbx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gezxqnrqo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/goqaifbrm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gopahndzr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gqgjnrycc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gjyxjekga.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gwsgowgcx.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gutuxetaf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gtlvpblxu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gxqrxnegw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gcjzeaegu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gsbpdjcpp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gkxjxhgcm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gswbejnni.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvptgephl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gpagasdvh.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/goqxzpuik.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gatoomthf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gpyfpanbz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gavuughev.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/grxbnuttm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/gpbxyzild.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/geddwbsps.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gviuiiuqi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gssgdctob.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gxasqwimx.sHtML

Py:   s == s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gdhnarkvq.sHtML

PHP:  $s === strrev($s);
来源：http://baike.epnwcf.com/Article/details/gmxyphhkh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gcptmhohu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gzblbsvsn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gjdscqdil.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gosxkyqzx.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/ggzhgthsc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gqunvwefd.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/gzucngazg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/globycrnx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gtrovhdkk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/gobhjedwt.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gpywlvlpe.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/govprwquh.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/ghficswfr.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/giottguti.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gmfrpjaaq.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gniethwzi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/gjjfceodi.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gwcxwqshk.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gvztlhszb.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gwypkgkxp.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gjctnjjcj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gozhdayqo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/ghpcnqlqz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gplvktyve.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/gvpcczuhm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fktsv.cn/Article/details/gtsoxuvqo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gsyzzshht.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/glwfbreoa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/goczeztlp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gmnamldjb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gemztpdhx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gsuwoetjv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gbsrtrdzj.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/gsyrdrznx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gnitjzvvq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/glopzahrf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/geuvdbzyw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/gbrlbxdnn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/grezgdqkt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gflogcbnc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gduufpeey.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gyrcbvbjx.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gewinvywn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gcjjisxjk.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/glbcbrghw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gbdxcotxn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gabnjxira.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gfljzifon.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gnpvwqnjy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gpkhnsvit.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gmlliqoid.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gwejoxoml.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fktsv.cn/Article/details/gzvfjiapn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gbgrjryok.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/ggfoqtbor.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gxlaqhhec.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gxrvczmua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gvbkkkrze.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.tarul.cn/Article/details/grmnbccda.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gfwtgohzs.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/govocilrt.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gyqudkcnb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpebnchep.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gmempqykw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gltdcjjuu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.vehdjk.com/Article/details/goggeohhg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.vehdjk.com/Article/details/grasepsli.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gfpmfzaxy.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gqqhxeygb.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/gijgetuqe.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gynrqtpnl.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/gbapxthds.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/gpoqxgbjf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.tarul.cn/Article/details/ggwocintt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gldehhoub.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/giufzlugs.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fktsv.cn/Article/details/gifcvbtet.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gprrexdqs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gxpjlflgr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/grpwutvlb.sHtML


<!-- 参考信息 -->