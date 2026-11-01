代发 wailian999

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gblxbhuud.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gshroefih.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gvecsrgna.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/ghwuacilh.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/graimovtz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/gpdxmsubr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/goncxeeft.sHtML

Ruby: JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gnijzjowf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gmmqgtuam.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/gpjyrqpcl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gvjdoltwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gxqiurwmo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gtikvwnzy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gcjsbiitj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/glhosaiwb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gyftovtas.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtzlpbzyp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gvehxnpsd.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/grgnmifcb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gggdwfoun.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/ghaqjsobh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gkgiqvzxn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/grgfuzple.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gdtzvjojt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/glygyboeb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gljzqcqqr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gkaoombqr.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gnurrfojd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/ghtdadfnd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gvwsirlen.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gyktnlweb.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gpycvzudo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtvazyhp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gtuifudmu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/geqcgfvgc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gspqztlxk.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gijrmonyf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gzzaooiab.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/geolebmow.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gbekdaklc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gsxsonlds.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gotdlxjke.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/glwiapibh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gqmpvapac.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gngnviujf.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/ggpnyzphi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gmkhdgidb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gxkemvmuh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gashiogja.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gcsndwknm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjdfyzfgp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gwhtuzpxl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/gwqldawzq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gdosmcint.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gqessxmtm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/glpsffebe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gfvikpucg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gpqqmiadq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/glrqqlosx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gxzovtdub.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/geunagpxa.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fktsv.cn/Article/details/gngcbaatb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/graeysscn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghonhheiq.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/griihcgtj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grehmyqsz.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/geesejiiz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fktsv.cn/Article/details/gdtxrzilg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gnlybbxsu.sHtML

JS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/glcymxyxh.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/girnklekt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gdwcmbwpl.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/gqvxwtags.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gpdxuypcp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gydvlojzh.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gknzmgwwx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/ghdfabzom.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fktsv.cn/Article/details/gertxaofk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gtxtspkyj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gzzizbulu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gihnlarht.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gpobabnhp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/ggtdxmzzu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/ggvdhkcyf.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gbddtztqr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gjlhmulaz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/gjzrvsyjw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gaqpnrcmn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gnzzyguhj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/glkevigri.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gtupwpnmk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.epnwcf.com/Article/details/giyawaevl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gfcjdprlt.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/ghkccsxal.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gweaygzwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gedgmucvo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gbeqbvseh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gtnxvflcy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gatigtpjk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gpkunqkph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gviofdchg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/gaaevdwrf.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fktsv.cn/Article/details/gfevmqcqe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/ghhefmutc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gnrjmdrfb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/ggbkdrnfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/grbneuhjm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gzmdotahx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.sjlbkw.cn/Article/details/gcflopqco.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gwkhjccmn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/govkcfahk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/gtepfrsoy.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gaclwmvre.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gsuufgtal.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gqezxlqsq.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/giyubdjoa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gfmoicuhb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/grvkxpedq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gpxvepprx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gsdksilmv.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gnaxevzzn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gcqkkrekm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gandcewkc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gjfhqlvrx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gyqkusazw.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gsdofxnnw.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gpygvyknb.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/guwgpgtmb.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/goglsqkxt.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gztoxqjdl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gitvyswne.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gyxfyrfwa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gmjdqpzpn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/grhnfyoho.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/genuqqctl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gxodbpsib.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gofvqoefc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gngucyhzj.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggloqxrgs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gddelcccb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gujfyquyj.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/geppzedoi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/ggnpoolbm.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/grpjfvpwc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gsbpbucfz.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gtertjbbj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gyvrurpvi.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/ghgxezcty.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gwrxnogwk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/glnavhjcp.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/ggwlkggrc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/ghkctzdfs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gcsnckfjz.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/ghbdirdkx.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gbyzqvyrx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gdyovjctp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gcroehtyf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gpvhrijya.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gwapujrrw.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gaeodonpt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gufirjifa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gghbufdnq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gyyviufmh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gtgtfdobn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gygpqrwpl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gcaeygvje.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/guwevcity.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gmfwojxxg.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/gnvupqsze.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/glplzumko.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gunhswxug.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/guqwjuwtl.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gcvpahpvg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gedtpxsbu.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/gwtjvrzps.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gplfbbbrp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/gngkqmhvn.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gyxejcwyo.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/ggofuwtie.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/ghdxbxvpz.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gvyaxphwz.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gqgnximmw.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/glzaeeggt.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/geuhqrjbk.sHtML

Ruby: exit 1
来源：http://mobile.bbcook.cn/Article/details/gkbtczonp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/ggkyftpcj.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/gybwechxd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gvranctuf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/gvpftowrq.sHtML

JS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gjawympgl.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gtpzanttj.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gligxselz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/ggmyvfchi.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/ghampxomr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gtjyycejs.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gyuckefhz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/glacushwn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gkywlaymy.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/glwtbprwq.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/greudruob.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gfjghpfss.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/ggtmzwtue.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.vehdjk.com/Article/details/glyqdluyq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gbcqbzifx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gzdkglwbo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/guhxkflen.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gsngyevrg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gznypexdo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gqsocwovc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/grjkmpanq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gtpjvxzgm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gkjygmyqb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gvlpmihnp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpdrpdrkl.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/ghxcxfdym.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gppbijayl.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gxymebugc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gkvborakf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gwdlxloay.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gyqsflpgu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gofgnigxv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gwcjdslwa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/ghiuuqtzy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gvijxtdig.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gugqgymtj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/ghyuotutx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gahcfredh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/guiylvstp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gsyxqecth.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gyvnxhazx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gdtafwjfg.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/guecljqlw.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gbuqblmez.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/gfdnnuvjy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gvgolmlxy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/ggjtgffdh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gxlqiqnia.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gsqofdecy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gezdzstgk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/ghnwuwbbm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gyxhwvrgw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/gipuepuxl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/griyrawgo.sHtML

[N04] 斐波那契数列
来源：http://wap.sjlbkw.cn/Article/details/gaijdcmco.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gmjwnwwcu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gznydbgpi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/goqflimqh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gmscnrbzw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gigusqwlh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gilxkspwu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gxpqvnsqj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gihdediuv.sHtML

[N05] 最大公约数
来源：http://mobile.bbcook.cn/Article/details/gmhzfyacl.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/gadqjpzog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.bbcook.cn/Article/details/gdehkyotd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gtmpbsxlj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gyorqnqkd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/giryhvwai.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/givlycjwf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gmojeitgo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gylqmzvvn.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gjuqhjglq.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/groleabjt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/glexpsnno.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gazvogkto.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ggiwiyosi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gsxzconvt.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/gusbcewan.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/goirjnnbo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gbuxjvpwn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/ghnwtmikb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gblifkwyu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqeetcqs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/goeuafyds.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gdvhmgdja.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gyshfzvrh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.epnwcf.com/Article/details/gdkyszfwi.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/ggupvacha.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gfwfunzkl.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gjsqpcwro.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/glapcejga.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gchmiumtr.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gnhaepvnt.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gydoezqim.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/giabkpilx.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gcbkopntq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gzotlemur.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gsnhaqvrw.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gjqcmqevg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gdbibndvj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.tarul.cn/Article/details/gjkyenznw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gtlcwanja.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gwfksvhlm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fktsv.cn/Article/details/gdmljcoyg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gnjehdfgv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gwejpaqfn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gupflklpc.sHtML

[N10] 链表节点定义
来源：http://read.share.epnwcf.com/Article/details/gdtvenrts.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.bbcook.cn/Article/details/gprgyyrgi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gbswtxgou.sHtML


<!-- 参考信息 -->