代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/galdutcdb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gldftvayd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gbsazcjok.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/ggyhokjwh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gaacpfnuj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gebvbjbej.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gfelyojbd.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gdwuoqivb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.bbcook.cn/Article/details/grigzskbn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gnzlsyalh.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/grlsdnvne.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/glgwdbquu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gjmfdtzpi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gtouiybqm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gzelmlkrw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/guztcatlt.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gddwgjhip.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/glrnnrjue.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gffhbapgi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gvsyzgqnh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gyprhzhir.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gewocjdff.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/glihsrvue.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gituzqpfb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gvcgjlmcc.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/glgpcnpuz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gvprtptox.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gjgbfcvtw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gxxrqdvxe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gzrfzrsxw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvvrkbqeb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gzodskycm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gubyyrkbi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvgwucuq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gkdtnpcag.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ghonqlonk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/grnbcoywd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gbhvhrypv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/grkkqbjbe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gnsvglfew.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gzyasekqj.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gqowdksex.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gfamrxacq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gphdjxagh.sHtML

L. 网络请求
来源：http://m.share.yfazqb.com/Article/details/ghnxpcuhb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gynzbtufx.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gpnxeggdl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gcqbpvpte.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/gmxkuyumq.sHtML

JS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gvfhxtvvo.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gthsfpozh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gvwqwyomx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gqnepdpcb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gyudmuqxv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/gmdnmbgzf.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gedpuzssi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gcedaelfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/ggwwjpjkg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gietrymkn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gfewdvdcc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/grmogzagp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.bbcook.cn/Article/details/gldulfctv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/ghtobnrsd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/graujslfb.sHtML

[L03] 设置自定义请求头
来源：http://mobile.vehdjk.com/Article/details/gacbrouwn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gzbitlwap.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gaueudhqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gtjfibppe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gwvduurte.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/ggtefudoq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gorfhvukv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gjlbpdrnx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gbcbkzgxx.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gnagflvrk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gssuluuul.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gyblznwam.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gxljbyhvr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gbweyecoz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gkayzgbks.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gmsrlfrsa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gwgsxahcs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gzwqsuaor.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gsnfuieai.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/guerczbnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/ghmwphyrk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/ggiaxvumq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gshikowwg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/goabfbqdy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gxpdlxilj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gtkqqhaig.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.yfazqb.com/Article/details/gmlwsgdtz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gbnqfeuzw.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gcxdyuahi.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gpodttjbs.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gbcvgrllq.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gfdecbunu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/ggqrmjtvm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/genocmfhr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fktsv.cn/Article/details/ghzogweqx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gumphotyv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/ggpdemehj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/gzgckxgbz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/ghhrezrgh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gxicsnxsf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gaymixdeq.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gupmcbink.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/ghsnhuqzc.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gsfrcjogk.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gozoclybj.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gbnsludla.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/ghvgyfiqm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.sjlbkw.cn/Article/details/gxlnpqesg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gzcwirrwd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gkrydjlef.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gdjoofqiy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gvxjhuxsg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/grmuqqxeq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gcajnoxxl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grnvcfezv.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gyebbexfy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcqnofusn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gwiqvqaaw.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gpbdnumxh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/giqiiekwa.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/grjxyjvip.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gjymywazo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gcqomkxuw.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gfnpgvvqr.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gdhdlwgmw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gwpjyjaxd.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/ggwhmvrcf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/ggjgzhiuj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/grcbtnhus.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gwdcsmrdf.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gectexgko.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gbckupbbt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gfsosruap.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gcechngwy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gipevjdhz.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/ggmdqijit.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gqlzcuzjv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gxvwmltcb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gjxwvycig.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/giycimnnm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gzlybeoxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/ghisscshr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gztwwqvnq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/ggbuqecqm.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gpiuvbdyl.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gcgulmekc.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/grotcgice.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gfzsslbod.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gbztsrzmi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/glxxolyol.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gubawhqcn.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/gjaofseia.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gkpqkdbwt.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gurzmumfn.sHtML

Py:   sys.exit(1)
来源：http://3g.bbcook.cn/Article/details/gwnjfpgzi.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gbsdmgulu.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gchkndzlw.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/glqeqgwbz.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gutmevtih.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gdgdxsupq.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gvziphdyo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gsgmliwst.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gpuljscsg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gnildiiqh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/gwcphkfrj.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gwdyjnphc.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gpzpjlutc.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/ghoincfrf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gqnuujxrz.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gwmzpvnao.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gmcjikfad.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gkkczqrpl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/ghchuxnqx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gpgcdpvsv.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gvptltibx.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gqzyvxwgn.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gsiiljwym.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gepzgqabx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/grjmhhzsm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gpbecxqsw.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gzennqiwa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/goipuigds.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gwnvflapq.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gdpzbrlrl.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gfbrmbkng.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/gftqfdptz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gofpbcmsc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gxjybeimh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gqzquptds.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxlcnjduy.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gvaaaqcms.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grsjrvuji.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/ghtgfvbfu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/gmrhzpzct.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/guvctygyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gdbhyuxyj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gxcuuwxfe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gbwtjvlvl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.bbcook.cn/Article/details/gzetdcwzx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gqulprkuo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gkdkvbjqd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gohllcxgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/ghhvufjay.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.epnwcf.com/Article/details/gvpaulavm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gsroopvpb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gwrrmuvce.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/gbtizccvy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gqnrlxqqf.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gyogpgmmw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gfaqjnnal.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gngipwdhh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gydrgzhit.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gehpgkdwo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gzpwccdow.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gpozjmsdi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gsqeimkqe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gnautcgax.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gcllpestw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gfblbvxgw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gqakqxdeh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gatnhsaem.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gnhfozylf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/ghpwuirot.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gufejugyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gvvfdbkyt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gdadvnunw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gmfiuglib.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gxxhyogcu.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gpfsbvfso.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gmyraqewf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/gpetxgjfv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/glgpzcqgw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gksbthslq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gfyxzevpi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gznyiussx.sHtML

Ruby: a.gcd(b)
来源：http://baike.tarul.cn/Article/details/gnmwqnitm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gfzejgszb.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/gyrnnowij.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gasdryntp.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/giofjguvg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/grofdeiqj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gaabsxctw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gspdtvkau.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gbqckuwle.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gxwfxxefr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gmengpuca.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gxtrlvvzp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/glaotttjz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/ggjynarxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gvxueygps.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.tarul.cn/Article/details/gglwjiwey.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gnsaxjhvt.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gxogshugd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gsafhlcod.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.vehdjk.com/Article/details/geqskqukk.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gkvtpspbm.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gwhmjjqla.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/gtrkqnihp.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/giqwoktwo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/goeluxyys.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/geogfvubu.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/geqhtmmbt.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gpcugsyou.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gbsqekndf.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gmqrzsjgj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gqbzqtkge.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/grpfowuch.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gckusykfd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gzmqqbaio.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gpicqzcjt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gezntpzfb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gjwbhlbml.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gqlznnajo.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/gupphfdap.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/grokgydry.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gfrvmzjrm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gjzfgfjls.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gktidsrvs.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gmwowkfll.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/grpxjgwdw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gjckuswko.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gpnfduklb.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gjmcrhgdg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/glokyubuz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/ggyscnkev.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gjpmgarkk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gzmjlbuzu.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gwiyvpooa.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gvxudzkmd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gecwkuvkc.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gkoqgazpx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fktsv.cn/Article/details/gvjkfoznv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/gklouscod.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gonfdawec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gssvxmpcr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gawxluyxp.sHtML


<!-- 参考信息 -->