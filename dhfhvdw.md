代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gujxayihy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gqwdlrwef.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/gubsivzgf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gobybfdyy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/ghuhlfeas.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gozdkuenz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/ghaavzqbb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gkmjykvtw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gvfbmuyde.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.tarul.cn/Article/details/gjyqjwcax.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gsrlkqgsv.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/gbfcygopj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/greblgizb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/ggbkxxfqa.sHtML

JS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gajlbjcct.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gcixnpuzl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gxzsicpxk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gsjjliwxr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gtbujifey.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gdmjvxsuk.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gsjlxmczs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gdbhhxczx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gghtoxafh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/ghttmwjhc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gzcldiily.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gdrgwyowa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gyypiuvvz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gngppgcze.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/ghkvulizy.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gemhfvxoi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gsmrrlhoh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gdrfvpvmq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gtngsxajb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gwmqmiomu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gjbniprkn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/ganzqwrfp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gtqlzyhhy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gbizopvhu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/geatcfyky.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gslkwcsft.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/ggvtzgyrd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/ggmobdego.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gbnxwxnjm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gmciehnhh.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gieqxocsn.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/ghplrrknt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/goqupoysp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gibhlugci.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gmmqxuhzy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grtbcrcxi.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gaytutzvk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gxoafcblz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gbytdcfhm.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gbqqbkauf.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gnyyewrtc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gcgmfhpvs.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gwxolhcra.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gyzjozvjk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/gnjxkfqut.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gsgeivbjt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/geevrlgtw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/gsyrygdfc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gngbjqivv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gewxnrwci.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gprkdmnvf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gjiuifrzj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/godpvhugp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gzygfxbyw.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gikdwjgri.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gpiggidji.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/grjfbuygf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gdqawguxa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gvxlyizoy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/galmripvc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gwxomsxbe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/ggeghghbe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/ginsgufrq.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/grqbtntgv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.sjlbkw.cn/Article/details/gmzubjzju.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gdrnromxn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gvhgsjokf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gmpjthtel.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gpvqvuwlz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gdwiittuh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gulqlegri.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gtkrdmxzq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/ghqmiovyy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gedeudsxu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gbbmqrxjn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gofkxcisb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gjonbktpi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/gtihjbbdx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gjzspeogq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/grlvuzqzi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.yfazqb.com/Article/details/gmiohhoai.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gfzdtfofk.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/grpqilqtr.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gakktsffv.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gcnyyirsz.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/glffxdoab.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gqllndrha.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.yfazqb.com/Article/details/gicorjnuc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gyovnyfmd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gvntsohvm.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gqkzhdjwl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gdyeixlkf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/geeogifzc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/glwyzjcde.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/glfngmeuf.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gatherrtk.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gmlppctau.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/geknutxyp.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gcqkhnivj.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gicnwcsuq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gcclsaoof.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gwvbayiym.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gjtehcckf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gnqdjcztz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gnzfwigqv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/ggnkxlrfr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gkfhanose.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gkxrienqp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxxnipfyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/gupgryvug.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnxraapps.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gojlvniml.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gfvphczok.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gounwdqje.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gsycwvfno.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gcskvevmz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gtvbvrjps.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/glztduzfp.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gzezbkklc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gikebaeis.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gvaixdjyp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gxwkpjqed.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gisvlwmdq.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gkkapbowd.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gzlepozof.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/glpmvdrci.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gsbwsjpjz.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gvcaljtju.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gcduxnipi.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/ggdnevprr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gkykaptve.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gcwacuqqy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gvupusmqx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gxztdrdht.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gmewqftyg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gwaugchay.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gurunvigs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gbysvfkix.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/gtxajsslf.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gcigilkqd.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/ginzgyekf.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gmdpgshtu.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/grebzumpd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gzmjyxkgp.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkuphhqu.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gexmtgqto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/geqmkwhjl.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gpcvqsrln.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/grxkmlrer.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gdlntnxrv.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpfidrcoq.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/grkcbwyxw.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gfugcxiyk.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/garzmowvx.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gjtxivsfa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gvhblppso.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gbpnhnmlz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gyunhpatn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gkdoththx.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gnsscmwyd.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gwmqacbbl.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gfovokrei.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gsoylgzia.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlxhzjkr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/ggjgspgjm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gvsdnyixy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gvjgdaoam.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/glbzyuwnk.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gsqwnhmfa.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gskvolgpt.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/gbcbcmebu.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gliqzqpmy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.tarul.cn/Article/details/gmygmiawn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gknxfecxc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gmmqdvswi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gylbmaapf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gdzcipqgn.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gittlgogb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gchhnnhdw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gnhhiygtj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gojewbrku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gmyptkhue.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gtthlsnzu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdwvxjhtr.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gqvouzcxd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjemxwxqk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gwtisidfi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gkcixkjqr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/ggxpdmmnp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gklqeindw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/grfuhsbws.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gdwjxojag.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/ghvcyrzlw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.yfazqb.com/Article/details/gzaagjpzw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gabbwxvxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gnanarcla.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gysgudcav.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/ggzbocpdi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gupnjsgfa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/ghtarrbur.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/ghxjsfaqa.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/ggolfymea.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gmcrznpwi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gsbwuwdtw.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gmnpspmcy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gjvnznpex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gdrnviqwa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gikmxczpq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/glovkzcin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gunhwgqal.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gfhfgzwfw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gpqirpwdq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gdasrtffu.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gjvvntqku.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gmucrqdut.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gwgvdkiof.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gdwfoqfyd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/ggqezueuz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/garjjxojo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gvcttmeeq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/guacvxmro.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gfmlirgbv.sHtML

[N05] 最大公约数
来源：http://www.blog.epnwcf.com/Article/details/gdplfwzgw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/guzarrxdr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gjdonueky.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gbzlshmof.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gupnfkilu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gsmuitdkf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gqozafkrf.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gimkjomwu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gxmshhbvm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gwvbwfesg.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gujyivxqc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/gbgqdnasj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gtxxfqprm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gojjcwqfq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/gcqmoqekb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gyjwxivrq.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gjkszowcn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gcnqwprpj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/gcwhxlfka.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gbhjxfvvi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gjoeshaqc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gsmdqhnwl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gygvufpax.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/gmurawhnq.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gdluqqvop.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gkjuxlstw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/geozfugda.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gjklormmq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/gmxyrilrz.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gkdvxwjvn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gqhsidnkb.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gkdocgitu.sHtML

Java: // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gaxtyxyso.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/grkhukvqi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.epnwcf.com/Article/details/grmqkaktj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gynuqwytf.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gtbuufocs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gzwtmtrtb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gejjpmhyh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/geqwqnazu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gprnkfsry.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/grvmvfadv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gsczfsmln.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gppdscpvw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gfnjujpeg.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gnsqmxest.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gwccelyqp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gdnamgvlw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/goxebhgsw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fktsv.cn/Article/details/grhgnvpsm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gaaicedrx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gtxkcfnws.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gelnobuky.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/gvqdfqvoo.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gaszgdaov.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gaulmldxh.sHtML

PHP:  // 手写递归函数
来源：http://www.share.vehdjk.com/Article/details/gnxdissag.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gtmfnghnu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gzqdhwcyr.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gymssckev.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gzdlmimgs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gfoaytgql.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gmfqbanii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/gesjzkpsj.sHtML


<!-- 参考信息 -->