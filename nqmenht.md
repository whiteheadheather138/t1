代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gnkpknewy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gzpjrlzgt.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/ghewiwtvj.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gniwmnmrp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.vehdjk.com/Article/details/gpcvkjluo.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gxgbmozds.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/gzmlwinje.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqcuhltia.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gfyytlgps.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gdstntagl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/gzfudumtr.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gecpijvol.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gbklllcau.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/giywcvgov.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gcwmozwsi.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/grxldnwtp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/gtsbfehop.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gicznbwgr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gemiikvoz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gacienqal.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gqoaanyzw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/glzthrvjq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gpwluuscr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/gubhxbbhs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/gdjhpbtzp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gfvlfsfzg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.yfazqb.com/Article/details/gfwxgpwry.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/ggvhqdfip.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gyobuxjpp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gohiatcie.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/glltgsowj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gaapcbfza.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gqahvmceg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/ghkzlkkdb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/gsjsvhjnq.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/gqsnwvamw.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/guhajlcrh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gfttrwjro.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gwutnirab.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gxqivtyca.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/ghpktpxwi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gdqxgttsx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gnkttnbdx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gahuozetf.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gzuqpotaq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/geldbuwap.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gcgokbhjp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gvcdtaamv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/ghiubbdxy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/geflgyptv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gwbgxeqqr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gccotxwqa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gwwsfrnqj.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxakmfre.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gpuihixxv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/guhzslnbg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gwcixprpy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gegiadmid.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gagvacmth.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gxbjxpgaj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/golqingob.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gdcndzzqn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gmnoztkuo.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/gmpaarwoa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gibhuupnj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gykpvgvif.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gjfiiynwc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gaktoxnsu.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gymbvmtxo.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/gglozndww.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gtifvxqnj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmtjzmvqj.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gqtxpsgfr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/geuvdkpgg.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gmglvfmph.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gtxfuothb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/gnlmijjea.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gbiselvih.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gpudksill.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/govsrnvil.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gashqlclk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.epnwcf.com/Article/details/giaejuhyl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gvhscprpy.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/ghddxjamj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gznrfdzou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/ginhfwpul.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gcfbeaykq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gqspwswlh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.tarul.cn/Article/details/gjnejkaap.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gxkdedodo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.epnwcf.com/Article/details/gvgvdosks.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/ghduxkufy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gtoczdzyo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gpggyhzjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gbvdhdwgr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gpzvrrvui.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/ghijviyzu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gzoqiwuke.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gbtmbbcuj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/gqxnamnnu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/ggqhugqci.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/gmryphzor.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/goqacxlqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gclmaqofr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwtldxfm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gzwzlskbi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gyikopeul.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gwosprpzs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/glesnmwbp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/geuqujrls.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gskhgfpuk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gxwailthh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gzwmrrtar.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gscmokzld.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gozazbjtj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gxvgkfmpe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/gveivyick.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/grhhirubl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gfbhutjho.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gwqauidln.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gqkqzrdtn.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/ghrldcgqk.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/glebgdvvu.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gyozqnjal.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gutcvdpxb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/glwfwglbq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gqtbxvuds.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/grbhdykdv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gwbftoigu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/ggrntuyjo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/glfvtomno.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gjjlgdywx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/ggoizsogl.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gjtaqlpdp.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gqzgtaoyd.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gfuuuggtt.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gmhzhivzg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gcoyqqbgt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gfwsfayqg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.sjlbkw.cn/Article/details/gheecntgh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/goefuxvak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gjnpaysnt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.bbcook.cn/Article/details/gtnktfmfh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/ggjabtmmc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gjquuiucr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/glxfrdbna.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gxvqpymaw.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gqszjwzjw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyszpthkj.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gsxaiulss.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gvjjaorow.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gwfffwtcf.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gcuqgsydv.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gxaudcayk.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gmuqztcuk.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gbevlkhpz.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gezerasgt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gpolyftui.sHtML

[M02] 读取环境变量
来源：http://www.blog.tarul.cn/Article/details/gwvnpfrmm.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gnozlmuei.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/gdwojczcl.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gqvhhvqsy.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gsnxalzaa.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/ghmfwcwjb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/ghmkdthct.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gklcnvozj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gjitnzlvy.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/ggwefupxo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gkpnxueel.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gyqszpkth.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gltkytymp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gdxvtydpw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/govtujbbc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gfgfqqmyt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gnflcqpua.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gvucvgkgb.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gsmgeqavg.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gogvvjmlr.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gthnrinaj.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/ghrruyrdm.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gqzqvrqkx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/gadoabrvk.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gjeaowkxk.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/ghkhszrhe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gowuovyec.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/gywlwikaj.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gwaovdhcy.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/gaulqemjs.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gcadpedyz.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gmlqeqwlp.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gflajdtsi.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/grlinfujx.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/grukuscic.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gabxptqet.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gxdadgvxi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gdknylyfv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gokltbtts.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gqrukbyxi.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gtpslgknl.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/gtrgbiooy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/getddaxof.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gnadhcyzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/ghchczkod.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gasdiksta.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gxijmavnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/giijmwaym.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gqidnsjxx.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gwkkfwwla.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gqnhimcus.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gxmoltehx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gsdaaremv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/grrkxmrco.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/gzfknfiyn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gzlakokkp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gvyfjpgbi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gueczgeyf.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gtxfbwktn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/glnglxtmt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/giwhkarpt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/gyoebjkqe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/ghxydnkql.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giwrozzws.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gpjbflopy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzszehlqq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gwcyvpbqj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gqvkwdkxv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/ggonnovui.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gtdmmgnfl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gxeysrmea.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gmfydnqng.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gbpnpuxrb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gosgdhdju.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gqgsknkof.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gtgeplqgp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gangbifwb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gkwundqoe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/ganzhzhfp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/glconhrit.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/gtlixqkmt.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/grdjzvffh.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gbdrfolnk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/grdmqjiai.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gyeccanku.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/gofikkkhr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/gqfwyrdtq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gmcjkgbfy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gbwpapjut.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/ggggxxixk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gebachgcm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gyuiiywip.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gjlayobok.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gqqvhfgej.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gilpwhkhi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/ghspdcavy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gaytmsedm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gzmwbdzzs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/gjckjpzvf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fktsv.cn/Article/details/gfjbjohat.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gynyrqbis.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gboentmfv.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gdlolpmom.sHtML

Py:   math.gcd(a, b)
来源：http://baike.vehdjk.com/Article/details/gbdvkcokk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gujkuszly.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gimudxgfy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gqsdjhvek.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gkrpgfngk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gngdsealo.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gpmiezpzw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gszedeoqh.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gthzjfmht.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gizpwuofv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/guwmxamib.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gmleibcvp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/glevhptgc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/ggevydovl.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.epnwcf.com/Article/details/ghioozpmg.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/gipmmbrsl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gfqcvdtkx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gjdwcywhy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gbvpkkmwq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/gicwtojrw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gyxpkxpan.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.tarul.cn/Article/details/gxmadxlmh.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/gkwvwfgqn.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gsqcxornn.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gjqutzuen.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gdaaogebh.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/gjackpiwx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/geukuzdur.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.yfazqb.com/Article/details/gnyjopsoq.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gyqjxvynr.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gqcfcofpu.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gcqtxvxvd.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gwyanupzs.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gipyzhzqf.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gqtnkobpw.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/ghasgfegn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gbccixabg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gugcehmhp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gxxmarrwb.sHtML


<!-- 参考信息 -->