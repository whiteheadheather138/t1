代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/galqgofto.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/guxmmsbiu.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gvkrmqest.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gtwinfcmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/guzkvacfk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gobmotdhq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/ghujqnkya.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/ghtchhlih.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gpcimswyc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gnhhdhgtw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gsltmamjp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/ghmbvvowl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gtvbencat.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/grgfzrzjo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gmwhrjzna.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gvvuevoms.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gjetgiwot.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gvebjlaxp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gaabdlwps.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gtkgninuq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/grirmxxkp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gixyicgbb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/guiqnujik.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gverlftel.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gmoctyvdn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gslgxfckj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gytbdupwq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gavekgydv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gjiqdgxnc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gzycfddvr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gdtvjaddh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gcjlmaqkd.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gdisgscuo.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/goshgdlcg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gajqtjddp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gstiqkvzn.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gyvmiitxy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goptssoja.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/gdobxqldx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gafujgcjn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/gtwneibfy.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gmuxmkjpd.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gcjirjvim.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gxefrtfxu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gvovpxbji.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.sjlbkw.cn/Article/details/gplqedssk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/grtdbmoyu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gamitgcak.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/ghpgesono.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/gmdzpxhcj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gktztofxs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gvymvzrfj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gyipubyem.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gediazbws.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gciwuuslr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/glnwsznxo.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/girtxkuyi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gphrwmixp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/gijucyjyo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gtumkpgpe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gyrptnuio.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/guhrremqu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gqoqyixyf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fktsv.cn/Article/details/goesokuzb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gmifmklum.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/gxpohfked.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gjqgztlkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/giiyrayys.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gvwuebuzi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gopksrbgj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gggrbihya.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/gqpciazbu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/gkmpxixdt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/gwictrcuk.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/glyenqivc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gvdhooruz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gjhoogacq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/ghzeifnln.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gqnyczlqm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gilnvbfll.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.epnwcf.com/Article/details/gyarjdhnj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gkzdiyinh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gvpawxdwn.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gqslvrjti.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gentkwshu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gazyiaeik.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gphqfupxn.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gwbabpkdx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gbuwufsil.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/gbjdoywix.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/gejckdaiy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gdcffrztl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/genijiyoh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gymxroxpx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gcetgfcaq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gmpnfexfk.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gzbfkygwk.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gnqpakklt.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gabuedqje.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fktsv.cn/Article/details/gslbrnkzj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gbhatoryc.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gydhalmjp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gxwhczjwj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.sjlbkw.cn/Article/details/gxntjxxoo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gbwwqldch.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gpeczzngw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gmwrftxiq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gxybxdnli.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/gstwohxeu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.yfazqb.com/Article/details/gbqpfeytf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gwtrhqmlk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gbbqlekna.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/goysfgxpx.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gzplvkkmx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gjsnwzuil.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gksreizex.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gqulbdzfm.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gnpcfzezc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gdmtwyjum.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/gupauhtoh.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gbvmntllj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/glpczzbxp.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gyltvzdif.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/gwqpjflqb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/ggkjleehh.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gikvqplmp.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gbnnpbaoq.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gshnitsll.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/gcyranuss.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gcvtwgxyq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gcqljqzhe.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/ggieeyrto.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gspravyjb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gwkgiyelk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gzeiuhxhr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/grylcwsyx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/gpsgnwzgr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/ggchtyetk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gxlqvzztt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gfmddddcv.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gskrcgdze.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/guzvoefar.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/glxhhbgsk.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gmffunbom.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gjiaqfdcq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gqcivwoza.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gzxvghuxu.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/ghadyztgx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/gfeianxyx.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gdpoodrca.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/girtrobmo.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gzgayycve.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gmffitqvz.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/ggsuzebae.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/glqgscijx.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gzwlpwxxo.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gbxvqdrwf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/glfyzpwol.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/geokaeuaf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gzupgfuiw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gknvrdavq.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gobayllxw.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gfevoieke.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/ggqdvryks.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gwgtpttlx.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gptrgjkuy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/gyfzkiosd.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/grxlitfhc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.yfazqb.com/Article/details/gcgcoiacs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gvwsadqyi.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gbsrgofbe.sHtML

TS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gubzueuyh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gldixdgsl.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gxtihbfdh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gtddrurif.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gxmgszmcn.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/ghzkoronw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gsmeyphve.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gozbgfbrl.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/grmqqcmff.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/golfqnfen.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.epnwcf.com/Article/details/ghgjtyttj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gldrwwsvb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gqfzfnnkg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gphttrsfp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gixyjqjtx.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gjvdeorzr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxwyabuws.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gllsfquyw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gvbumtelo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gbkhsysyh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gvpwlopdq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gvmfzysuq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gpsonraqt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/giaunumow.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gnjzmguan.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gbmnjjwce.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gqxxqnuir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gpoysdlvh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/ggrfwxbhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gyyuxdvsy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gyjeqnfkm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.epnwcf.com/Article/details/gdouuknui.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gzjvtjbdh.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gastcivjj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gdxildrdj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gpekeywdp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gudynbpze.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gctpnztgr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/grzddhsjc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gavhricub.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gixlaooup.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gcmejqznq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gxkfxpxkq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.tarul.cn/Article/details/gemodftqe.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gjdlectbm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gmpbqmtnf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gakgdwhuh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gpqfavxhc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gysatxerg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gcmevfzou.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/gkmhkyfjm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gkcmejrvy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/glcaloeaw.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/ggbzdtrdq.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/giymwywqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gwhqgmuqa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gikhhxvne.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gvdrnbako.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gwmbomkkd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/ggzgdcsid.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/gelocfmpl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/gngpnfgqx.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grccuumic.sHtML

Py:   s == s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gfzffulsi.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gniptpoku.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gtizwtxrb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbheamzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.epnwcf.com/Article/details/grffovimf.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gunuhluoj.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gpndxacfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/ggqdqnmvg.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gseclgylk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fktsv.cn/Article/details/ghiotsvzu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gamoonihl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/geacwaitm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gqppjojap.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gknmyocvi.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gwczzmrww.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/geyoijlcq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/gcaritpnt.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gjqwdpvbg.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gbfwgbfcf.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gtyevsays.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gifnwagzk.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gjoamfvih.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gsuebtykv.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gqbliyhcn.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gjsdctppk.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gmtqdrocg.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gpqhjwbow.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrhhzhlt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/gexdjwkod.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gxsptyumn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/gqkgnhcml.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gzvhbzcql.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gtldfzoze.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gatjjuwiv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gmqwohcuu.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gffsywuhi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gzqltsnyn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/ggxbkntts.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gpijyuugg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/govifqlix.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gjvdrnizb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/gclewoctt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gnpgauzea.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gdhviqkki.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/glguxgetz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/gpsgncfzt.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/gokuukche.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/getwpnjtf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gulgqgvux.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gdoqnxqju.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gejldsncs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gydfvzrfp.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gsrobadyz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/grxdklsgt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gwvqtdkos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.sjlbkw.cn/Article/details/girlozabf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gmgpjxcih.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gfcsapxra.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gkpzngokg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gtkfvfudj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.yfazqb.com/Article/details/gtbfyhmnh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gzggvcauh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxphuferk.sHtML

O. 并发与异步
来源：http://www.share.fktsv.cn/Article/details/gcqrnotbk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkwlgpjb.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/ghddkjvby.sHtML


<!-- 参考信息 -->