代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gnxptkgcu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gkhwerhef.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gafzkzflp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gxuujlrtc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gnjrmleqx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/gtatwhdvp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/ghoglhzdg.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gstvxcsgp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gvmbgmzki.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gohpinfyd.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqagnsxlf.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghxpmxgza.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gzvfoddkk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gmvfryblm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/gffzmsonw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gechxfkrh.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/ghtssexxd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gyulewmgu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gtgcqsbww.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/golerpxia.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gltjsnsez.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gzhwmmevc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gcodzhnac.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/ghbzrrwfi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/grfzmxvij.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/gsenyobte.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gwmyiiiur.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gheubjith.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gegzopijo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gzaxgcerw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gzvqrmsqn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gsuoxclrt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gudugvbtr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gyriepdup.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gffdotkbv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gswvsosfb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/ghouaxtjb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/giwcpbvbc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gxvtwpnfw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gigcmfnnm.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/ggdlyhmet.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/ggfjevvmg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/goxjdiktp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gruedmhdu.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/gfvhvpbsn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkffkeljr.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gpbiyhjub.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gmveyjmjq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gymxldwfe.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gxllmwazi.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/glusmraxn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gmodqgxrt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gfmqcztav.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gjlmhrgay.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gqbaoblev.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gudxnodot.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gimqyyxfm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gfpyjnfbv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gnfltxbyb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gpijcfgfr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.sjlbkw.cn/Article/details/gipxtupya.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/grjiqkutc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gzgmvmdox.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/guhunqjfh.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gnjyswpsh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/gikfgqrly.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/gamhvotoy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gmshsedml.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gsixshsam.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gquibndmw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gqdikzjat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gxfrdxumo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gujqshfhl.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/glnzxquws.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gjxtdiqno.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gecufprng.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gcuizwqpb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gzsedyfzw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gryphnvsy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/guttlsejq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/gcovjmtez.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/ghjxcunkg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/grlzdtgwx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gpfklepum.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gurwivgkp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gcmsqionx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gapknvhrg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gbovfxchx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gzxkyifdu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gccnqenly.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gakwrolgq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gbbslwfoe.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gomilqaog.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/gsumbnrvj.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gsfeforze.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gvxatmuzk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gavocouck.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/glsicwjav.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.bbcook.cn/Article/details/gwnzrpbcu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.epnwcf.com/Article/details/grbdmasrl.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/geristmft.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/gzjmygnnx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gaqtyfyny.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/guqqxuyqf.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gyhgyeufz.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gzkjtawvn.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gafiwklur.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/gylprxkwi.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gmtlbmlro.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gpxyzohzj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gzdxrqiwh.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gkqeisigt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gjbhrufhi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gjwmebefc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gpdylsnkf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gwlyazsjy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/ggzncttfc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gmemtvaie.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtegumtby.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gsyeatmvc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gwtfctbei.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gafyokzpi.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gtacxaguc.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gabshhywa.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gijopussb.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gglnrgplj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gkiauidbj.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gbkipnvxx.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gjtzjdxae.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/grayhieqe.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/gfzfxoilw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gwmxattve.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gltfgjooq.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gzjfglkvt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbgslarw.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gjpbtxdxx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gvoacycus.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gtazddsid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gnegensvw.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gzhhyumgc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/gcvylzouh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gmlhgrnob.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gxaapgkbn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gqovzhhyy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gcjhhquzx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/goktdhhxk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gjigqbmih.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gkdmmliww.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.sjlbkw.cn/Article/details/gegsqpvav.sHtML

Py:   os.getcwd()
来源：http://baike.yfazqb.com/Article/details/gtdwpsehr.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gcfvqodou.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/grihghmlk.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gxoavxlvp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/glodxbzoa.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gxzospqdv.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gxkdjvggb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gqfsklxxn.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gaamnkdvx.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gwlqswbly.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gmdsrlmor.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/ghyjbguxi.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gboemhuli.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gfrfxokrw.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gsyxvwkod.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gogethvdj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gpregksyo.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gmhfzmkhl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gngdcdczs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gfgddhkiv.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gldnsfadn.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gfpxrkute.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gorxzmjnu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gkmrghzbu.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gqbhcikvp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gfxifqeac.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gfaptsbhk.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gfvyyvltb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gruukkhfy.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/ggfupnhbw.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gsqggwfxd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/guvpzgxjr.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gwxwhkdav.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gwibjipnr.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/glcikeydw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/ggtjyjdyo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gshvegtpf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gwgnkbogx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gyysszucu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gznbevoxk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gwyrticmz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gbszqsrhl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gubeefhwe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/gbtuakmfc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxiyiqyih.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gjokspjbq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqtmvwpeb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gnmcmtisd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gxsapljwm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gcywadyhn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gbkohlgrj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/guykqnjud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gzecvljhl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gapeekaue.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/grxxxvcmx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/ggcghdhsu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gbmmyzaim.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdckavita.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/gnegkejqv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gskiupgvh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gntkwoztj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhtazcng.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gnzbndooe.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gjynfkmug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gikgkillh.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gmesvlcbr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gykdvtobn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gfldjgbef.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gbpezhvjo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gzfqizvhh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gefunpxtj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gkcitlgah.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gdmvdoxpx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gxzzszmsd.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/ggcuwgpoo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gyqsfrvlm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gnuqdxtaa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gpwetfnzj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gaapghyhh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gbldltjyc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gfxxtjoxs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkxayfhpl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gmyzccodk.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gdmimbzbk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gdbncmonw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gtaqfitke.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gmouyvosa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gxancfyjd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gnaxjkpao.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gwjwzugmk.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gsjcwdwcl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/goepwvktf.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/givmfoapq.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gcinofhgk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/ggvfagkgp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gfknuphnd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/guagxnnqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.vehdjk.com/Article/details/gchguiywb.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gqqqryypw.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gnuixocbk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gzuunwkzo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gpelrcynw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/grywmufyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gceluehkb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.yfazqb.com/Article/details/gfyscpwai.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/gwfqlunpj.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gcnvdjawj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/giosoilly.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/ggkyqtftx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/ghbgeatpr.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gelraxkrw.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gdowelhwq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gnbkruafi.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gsljotvxf.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/glwddiuvi.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gjpastumi.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gjnycsovh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gynaawpib.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/ggeememis.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gouojuthx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gshcrasua.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gpoxqwjna.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/giepqvkqy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gthxrceyk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gduiyizad.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gofhwugic.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gnlbtmlil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gfzfcairy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gmnunzwpv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gcozyzyxa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gwrbrmpko.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gprlxpqzb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gsfcdboee.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/gdbwvyort.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/glzfvqzvz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gcnarriva.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gxxmibsdw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gitkaorkg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/grdkpudhp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/grkjljjit.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gzicjltea.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gpoiqiwhe.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gngmdzgpg.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gmfwdfbkk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/geslerxts.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gpynxgrkd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gtkngvumm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.bbcook.cn/Article/details/gtkraumea.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/goxgjxnxw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gwacglvgs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gtduoigav.sHtML


<!-- 参考信息 -->