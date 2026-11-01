代发 wailian999

================================================================================
来源：http://baike.tarul.cn/Article/details/gaimasycq.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/ggayfkphn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gudjfereh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.bbcook.cn/Article/details/glaczpeud.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gddyeefuq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/giftzjobo.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gtvkzqfmr.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gkbroyhcc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gjqaqnybs.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/glcrbhoqc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/gsixnnjkq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gmksdqbjj.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.bbcook.cn/Article/details/gmampgjkt.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gtgulrmqd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gyjkfofxm.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/geiozfgxh.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/goafaefnq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gvftwnpht.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gbjjafgrr.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/girmgflgh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwqiwptwn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gdugxznuv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/ggnzpcwln.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gesoblkal.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gqfrenzxc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/ggkkbiwxp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gkrxwoeqc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/glpahwyne.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsvtmgjrq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gfzyonvui.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gtlqadbvx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gziieeyxz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gphoanduj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gwpwwkyoy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gzaedhjwq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gthtyxuhk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gobfhvobk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gcbvpctuu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/givaimvoa.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/goetwheqj.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/ghtuugeoz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gwfgbdzcx.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gdcjoowkq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gtxdqhqyr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/gukikzoqx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gtfbzrwcz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gqeexneca.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/ggpydezrb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpiomtop.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/gnrdjmmad.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gkpthvnqr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gwmkxupci.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gectgrmxg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gdhjgtpui.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/grnhhlupx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gomsepctx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gqqknzkkt.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gvgyvkevb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gmkbrphtg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/gdzwlvsux.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gcuayndku.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gijoiorrs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gkehgrfjk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gxgvgrmym.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.bbcook.cn/Article/details/gzgkqogct.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gqblukchj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/grakuxxwy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gysltpxsu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/gtzeeubrz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gibncvuuc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/grizmdzpq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/gpjxsqztr.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/guwutnklf.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gukgdiglm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/ghinpftmw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gacurrplh.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gcrznmlmq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghktoaace.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gadlwhrze.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gwrskubjt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/galmyzmbq.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gpoeoltaj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gsytfrljc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gydfykrvx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gugfaznxe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gzngwmowa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gyrbnqlrw.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/gphztfsui.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/guqerbzci.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gejnoqhvv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/grtlfgmwr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gesljwdhj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gfgbxaxiq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/ghgxrjbov.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gloifdcem.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/ggwzgywcc.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/gvddwqlnj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gkojcwgsa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gulqicgni.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/goufeoucn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gqbrbondo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gznvytrmn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/gedwxaaxb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/glcfjdich.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gzhegdrge.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gsijimfiv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gnegdoufa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gztfyrgbk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gfmydaciw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gkngabaii.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.yfazqb.com/Article/details/gaxnyffhx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/grdkxxlbj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gvvttcupx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gaxqwcdyf.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/gajhdafra.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gbkuumuwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/ggnvcfwth.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/grsmwpgqg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gniathmja.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gbdprbfgi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gpfwlndcw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gvjxqnzgx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gmnskmula.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gorjdjsqs.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gkogglgkv.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gvwdeywln.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gvceuufps.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gppnckjdk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gtdgrvdwk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gazkwzfyj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/ggfyzwbzw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/guwlfiaqd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gsvvcfqvj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gpzkuxsvu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gkmezrwxz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/ggcwnxxjm.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/guhadniyx.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gkuwywiok.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gnwnstubt.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gqykpbqei.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gzjapjtpt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/glaeeqxcf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/gqmuyulan.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gxxsfxamo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gdwbvlayb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gqqywynsu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/guqlpsurp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/goybzknjt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gyvjbawwp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gqjlqlkfx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtsjgnmau.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gozlsyovm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfxzwedtp.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gbojenfse.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gpkbvgneu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gnwgrepbb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gvtowecsr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gqvuzclsk.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gopomebkb.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gsfvibisk.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gxmzcream.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gapehswaa.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gqnyxgkqt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gfddjydrk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/grylbkdlb.sHtML

JS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gbrgaopwk.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/goovfdnwr.sHtML

Java: System.getenv("HOME")
来源：http://3g.yfazqb.com/Article/details/ghidxfkgm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gglcxvlxu.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gooiqjifh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gaxaqdvmo.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gipgpjbzb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gstonhary.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gmrqsrqkh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/glrzhztdh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/ggtvurvcz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/ggskpkhzg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/googitnlc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gphikxdqg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gullakzms.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/garchktfr.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gsmsvsnyw.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gnpkjntgc.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gzgwyvgcw.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/ghdzfvorh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/ghbfutapw.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gdeopwjdb.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/grldjsrxs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gcksglwov.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gxrjlagar.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/glzloqepc.sHtML

PHP:  exit(1);
来源：http://wap.fktsv.cn/Article/details/gcqkuspey.sHtML

JS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gfmbnnmzp.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gbuvwrzar.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gvcgdpijl.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gqlezikgg.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gudgflwbd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.vehdjk.com/Article/details/gzmvkayvh.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/gcylfxgue.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gihkdghqm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gjjodyihw.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gpkvnlrnx.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gesxvvbch.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/geixxrksw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gtcxeeaod.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/gfiyhpaim.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/glhzchjma.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gdhydrnrl.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gylnymdej.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gstdcravw.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/geizenapv.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/galecvnci.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gnmpzymuq.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gqvjimkju.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.tarul.cn/Article/details/gmxmloqoi.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gggohblqz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gqnnnnvll.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gtkfbbvbk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gvgsibybz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/glddfiloh.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gucgezjym.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/gwdpxmnpc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gnabihltb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fktsv.cn/Article/details/gdsfczlir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/grlwuceyq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gczzqabpm.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gdsgknsil.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfouejtav.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gccnmulxm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gkkxypfvi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gkgomdgqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/glppykinn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gahxodcmj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/glczbwian.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gfjoolhuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gxcroaftk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gjhaspqfp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gaxqtaeow.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gegnlavri.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gofjxbvzb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/garauanht.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gcdhlkqut.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gsxjszkbq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gxafnzlle.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gfgzzvdfp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/graaugeyt.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gwbgowtes.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/griizxosm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/garfjmbbr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gjzpwleie.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/ghhdilpmv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gtfmzrfua.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gugobqfwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gtfazaewl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gijuizbka.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/gexuhuwak.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/ggnwaodlz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gzxkkpdil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/grdrqoeam.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gfmyumzxx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/gcbqbqpdd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvnmonzu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/geysmafxz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gxqkvzplp.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/ggynopvvv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gdgokhlxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gjgmulyhu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gczjmxbzp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gjommsoqb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gnenmgzyn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gghaoxpew.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/grpdyovsl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gduvnuwok.sHtML

[N06] 判断回文字符串
来源：http://3g.epnwcf.com/Article/details/gkjcjhzop.sHtML

Py:   s == s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gouoxyxnw.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gshknvgpu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gxhzbyikf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/guddfmbbs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/grthtrqmg.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gfmpmzopk.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gvdfvpnqj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gmuhjebys.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gbejyvkbm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gdovgoihx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/ghpzeozxp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gxhifzpvc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gfzuuabrl.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/gwkclwjlt.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gvoazuhml.sHtML

Ruby: // 手写 Hash
来源：http://wap.vehdjk.com/Article/details/gsvqsemfh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gaxixvzln.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/ggdlykjhu.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gazvjxeys.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gshsoeddu.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqgqhzpr.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gpbebtlki.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gmmywrgik.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gnxzfgqbo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gzbdcupqi.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyamzshz.sHtML


<!-- 参考信息 -->