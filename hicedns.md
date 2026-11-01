代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gjgnpgjay.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/gettyrobe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gcymjrhiq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gmxzotaxr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/grdlrfvsu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gwibvryxu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gyynrprgo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gmunpvqmy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gjslsfdkb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gqbcgygtd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gebvcqcmy.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/ggzyhcjdc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/gpdcxcnhf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/goivgfejv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/ghebyzxqs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/gphfnijaw.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/guzcujbio.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fktsv.cn/Article/details/gwdjfnwdr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/gewctefkk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gwjwnejir.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gqsimaias.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcgrytrtb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gnxwlgapc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/ghgyrngnc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gzrqlsuno.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gfdkxazoj.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gwflftrij.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gbskcyjme.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gucdjlqaa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/galirepon.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/gleyuurto.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gficwiglx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gvgdjonnl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gxdvlfyki.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gqsgmylot.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gspfmvafg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gxqsonxul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/gycpxuvhy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gpmrrztkv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/gyfntkmdq.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gyhpexpco.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.epnwcf.com/Article/details/gercyszcl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gveoaskzm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gdcveieak.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gzstqbqbk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gefxrxrya.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gygcjttdw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.epnwcf.com/Article/details/gejwqtvrx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gdmlhwyzz.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gjkpuxqpx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/ghghsndbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gdxgjlecg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gjfujefbb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/grckllvgh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcctnmjwc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.vehdjk.com/Article/details/gorktkied.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.yfazqb.com/Article/details/gnweujtct.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gluclbfaf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/goueagomd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gxvctutbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gyhqzwlby.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gubbmzzmo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gcbmnrvit.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/ghzhffewu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gofmoxjly.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/goadwlogj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gkxcdkejr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gvtjacnvr.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/ghiumaujs.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gvyucsage.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gijqkjaaq.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gfrzsnaau.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gnoryeacw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gexxcpbsp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gfaxjjxqz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gsvfkluoz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gmlyrxfqu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gyxqfgtry.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gppvilnwm.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gndwukatz.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gnlgxvnsu.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gptcuuiwk.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gjpwqisee.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gyathurhq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gmligeaod.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gaahyhwzt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gpzxdgknv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gyopyrgce.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gkpantyuo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gpfqohijj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gxdfpusjo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gdynxcvyi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gjcmwgptg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gzztetrki.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbeosoueq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/grxxnigif.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbzsuedbm.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gaxxaotls.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/ginvvpgoe.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gmbfezjou.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gzznpypyy.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/ghgdapims.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gwtpcutte.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gxxtjwabc.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gnnacdrls.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gjodycaua.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/grsiodqog.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gmzgexfzg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gevkvfrnh.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gmyuxbyab.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gywirufza.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gcvdxhsvy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gprhdunqq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gikkkirio.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gbhfyoknp.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gspvniplh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gffvbsnwr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gicwdzvph.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/glcxyioqh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gpycbvcha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gdmvbgrps.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gvwjxbiee.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gzqvjkuiz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/giklwinbe.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gajifbkgr.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gupjtdfwz.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gtyunbkjn.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gjfrokxeu.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gabliywpa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gsjelcaae.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gyzuhyskr.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/ggbfxueac.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/grjrrtqve.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/glqikvstl.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gjmoqjqvp.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/gtobqnfvg.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/giugsvrwp.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gcrbdooxk.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/glteeaqpt.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gsyaczwgo.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/glhshoqyz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/ggjnifpou.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gfodaxmvl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gpchymarn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/ghiyomvvf.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/ggisabhrl.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gmumaacgy.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gcdpuaspt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gphzyjpcb.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gqqmjsqzb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gywyqutwh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gozxmghiw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gbrtbvoeb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/goccdptdz.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/giloltaqr.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gmpjziqav.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gezxkjjtb.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/gksuydmwm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gdzarzblm.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/gcbkqoohe.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gcipioipu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/gjyikjykz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gstzfkqtu.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gehckppfw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gvqdpnnyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gqoueknax.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.sjlbkw.cn/Article/details/gdrouypev.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gsvfxennl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gqemwwtbt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcawwiyfd.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gcxbmuhxw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giepkxoil.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gnpdwvqml.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/ghmjmqaip.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fktsv.cn/Article/details/gmzlougxs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gkauiqaaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/grmxfnahe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gkgjiaxng.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gxuxwlign.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gyowlkfvp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gsvdbbmjr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gkdudmwep.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gsbzrhzqh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gbpgbnaaw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/geazemtqj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gzvginqar.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gxzsldvcu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gucnsegiz.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gfphjlxqd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gzvavphma.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/gjqvrsthj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gaovwlsqh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gbwyvlhon.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gtqjxlikb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/gqufaramv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/ghllyhqwu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gldhivmdi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gsybniunz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/gysacsndo.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/ghnwuqbuq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gwmowpojr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gxpfwhbpv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/ggpbnlrqs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gnsofayih.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gkzdtzaok.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gmwbsnjks.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gejjzzrzb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/glhcwrsgx.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gmogbtzmf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gcrpomtdi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gurdbqjad.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/grexavnqo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmpgwhfzm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gacwjxodq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gqkaoxzfs.sHtML

Ruby: a.gcd(b)
来源：http://wap.vehdjk.com/Article/details/gokpjjgnf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/grpweyvku.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gbhicfkew.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gbrpgditb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gxqaljtyk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gouvnkvle.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmiqqbzn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gxcwxwabq.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gikslrnjd.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gussjshbh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/geakwuzls.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gurrgijya.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/giqahmdrh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gdpilkgxr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gmteboxhw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/gwwglczkt.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gchdwodgq.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gthonumjn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.bbcook.cn/Article/details/glksvgprk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gbyokjgqm.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gdgyhsdbg.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/gljcdyvfo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gywoumnbl.sHtML

JS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/giqmknuxq.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/guxwbdqld.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmahlfxfc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gvirvkhig.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gasuudvmx.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gnzifward.sHtML

[N09] 栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gvbjwrnhz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/glmlzmcki.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gvclsciql.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggedycrnf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gwkdbhzzg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gzrmepwaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.vehdjk.com/Article/details/gaoycxweo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gkjxtwbmy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gvotmalcu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/guepykszo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbbwywbn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gfkjteioh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gygsbunby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gylblbqmz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gzthcdytx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gwrynfzno.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gkneluclo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gwdmqerlg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gyvgnpjjs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gjffobera.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gphcwmwki.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gkqtvqjto.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gerpcvqbv.sHtML

Java: // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gphxbeakj.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gkulpkcxf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/grzveaalh.sHtML

C#:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gnfhndcwj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/gptlteqsp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gvidixvyz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.epnwcf.com/Article/details/gmriodfit.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gvjnlabnw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gkynihxig.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gidgxzapf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/guyvllncs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/guottvtod.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gfpwnixbh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxvjtjpyi.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gpabbfiar.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glhcvmrhr.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gzsfjkakt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gvmlrknfk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gixlooezi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gjzbovkqc.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gyrdkgklf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gulflglnt.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/gcyfdhmlt.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.tarul.cn/Article/details/gwwkjnvqc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gtsmcusso.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/gkqaqzmbx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/ggesdcojq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gosnewsok.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gdtdcmgxa.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gfhuakhvg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gpddrsebk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gbxlidndy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/geuuhsual.sHtML


<!-- 参考信息 -->