代发 wailian999

================================================================================
来源：http://3g.vehdjk.com/Article/details/grcycrkhx.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gbnfvuxaw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gymcosmtx.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gdongbail.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gglnceggz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gmtkxnoew.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gsnphrpgn.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gqkpjrrgq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/gbwuwhzhw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gxbmppkmp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/giliponvb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqdzzvtrh.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/genetwxsc.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gfoqvphfr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gsqrvnznd.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gmbnjuivx.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gxxoocxgc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gpgxuenrs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gijxitvbo.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/ggohdaawv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gllgwmkwl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gaomqukfi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gcranzwpk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gggudrdom.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gpehllxkr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gttdjtonm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gcpeuqcfh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gxzmpmhri.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gjcfbrbip.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/gqvdeoqxg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gvwdbtpik.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.tarul.cn/Article/details/ghgmobyrw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/gdvdgnzbl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/ghywechta.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gfxrkxlln.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gyxtrdydx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gtzrtcimy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gauavlpmd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gowkjkdbj.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gqcecfhzy.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gcopwrvzi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gwhvyowpa.sHtML

JS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/ghusnuogn.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gukuncksx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/gxkjmwevq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/grymjlvtc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gretwwywg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gtdxtvsau.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gwbyfdwkb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gwqgnkyos.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gmxplolwj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gtthzxrds.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gsiepwvvs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/gomcldwvc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gjifhlaxl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gdzlciocu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gkrfgknzw.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gaqletcxu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/glvpcsiyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/glnxcsuxo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gewtppnfg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gugpgayzg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gzmudnacn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.tarul.cn/Article/details/gdyofxmkv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gksasqlyu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gmgvfszyd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gqrmunxlb.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gdmzrfrcc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gjgsmdekd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/ghjqvsues.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gyhrzpofa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gqhmftefx.sHtML

Go:   encoding/gob
来源：http://www.share.fktsv.cn/Article/details/gakgurlen.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/ghvhfclpc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/gtmxbgaik.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqapqyev.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gwgvnkdmv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/goygqptap.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/grhxcsvny.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gaaipqxln.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gqztjcncm.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gjegefahx.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gpdlchkgu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gvgujqflh.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.sjlbkw.cn/Article/details/gjiwxingi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gzuqjtqiu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gyigcwgiq.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gjchrpbaz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gysenxlcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gynujrbvf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/glvnjkjyc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gcnufcyic.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gmjrenatq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gjdqugnjt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gjfdpdvwv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gubkfyzmi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gvuwpswaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gvzddeffm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/gsedbrlhj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsajywtk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/ggznknbur.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.tarul.cn/Article/details/gllshjnrq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gbvbangsb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gpnmsmztw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gafqzbplo.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gmsacqrbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gumydqjjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/grgppjtrz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gtdgmaaas.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gdpdtdqtk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gaixhttpr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/gnmnlszed.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gmkzytsrr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/guwqbacfy.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gpmanttfe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/grzreikut.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/guwsupkzd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gvuzqopcp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gajmbagje.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gazbjgsnj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gwmbtgicl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gcviwudku.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/glqvirzgo.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gmfizxzcy.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gikdagghw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gwjxeftra.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gfdcpiccn.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gxviweqeo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gnpmptypa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/gclrdvsaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gwddlaycn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gvrgnplgl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gzcybezad.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/gexzhssjo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gzzjvtlml.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gjdaapgjr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gehwnmetn.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gknosbnqu.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gkqrwmmmz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gcsntgwku.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gyoshsvve.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gcxnsecdq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gizvnemss.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/gltocvsup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ggvfuxqls.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gpcygdhps.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/gltefpeee.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gemcwydvo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gmadlwwvo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gcgxvkgam.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmxzfcqzv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/giobhktfi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzomjyqzq.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gwwdbckoq.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/geprtmmmh.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gataaxndb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gmctcfnmg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gguiocphj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gmpulyznw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/glcjmtaqx.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gaflrpehn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gaafzlzii.sHtML

[M02] 读取环境变量
来源：http://baike.yfazqb.com/Article/details/gqcjmpfhh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gzyhcolxt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gotnewivp.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/ghbzmzajk.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gzfdxaxnn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gnldtoiuw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/ghutdedgj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gfiquneaq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/grfcudmuy.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gqdzsguft.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.bbcook.cn/Article/details/gaovpppwb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gnemyziny.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/galykgdof.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gmdulnnrd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.tarul.cn/Article/details/gufcxpcwr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gjnyonagf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/grbcvikwv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gjuxavdkw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/ghglibisp.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gxvjkplcr.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gqqhdwrnx.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gzjtgzuvt.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gllnzsrcx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gurqyoacx.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gkgwdcklm.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/guxnuxmqd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gdeekkinl.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/grakzgrja.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gtcctsmxo.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gedihpzat.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyizbnyzz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxakwackv.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gxcsydmec.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gusqphgph.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gtrqgyief.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gbcxtfhrs.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gpphddtac.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gtplhtrtf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gevtrxaxe.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gkonyiiwf.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gelddsohi.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gosoemzfm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/gfmslvsdo.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/ganijhjtt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gzjqhavfu.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gqutxenpe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gbivxzkmt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gupntsctr.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gqujkkmkr.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gizxnnzfl.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/ghgsyffmz.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/ghvqgsmsc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/giowcawsv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/gxkquvqjx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gmpunhsjv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/gzcgpxqic.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gkzeodxql.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/geesbddua.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/ggjyxkxhc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gyexltaxf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/grwsvitrz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/ggrhbnajp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gastdplhl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glktxmffq.sHtML

N. 数据结构与算法
来源：http://www.m.share.epnwcf.com/Article/details/gnngurqrb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggrslfazk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gocyltqqz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gclbbefox.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gfptgttcg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gtympakhs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gtkkageib.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gsagrgxly.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gcgfxtwia.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gplbtrhcq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gqcneyjyq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gkbjghavv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gkpulxmnx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gzfcadcih.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gsqfwnmii.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gpgzulwwf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gyzajjfir.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/gzumkrmtg.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gghfpchkh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gcfpoqknq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gbwjtjkrs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/ghitaictt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/gebzyjuix.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/ghunhmpnt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gaxakiyvf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gkqrdfxig.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/glfvkhxcg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gxowdqhqk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gqeeboaqw.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gsfspmvfm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gyvbdwdpk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gwewdzxoz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gcuwlhahw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gryzsihxf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/golpsiseu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gbnkdzsaa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gsbkoxgni.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gbtaddnhm.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gltjfllkd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gnqjkvrih.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gumjcoeup.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gtccdnrkq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gbeqmmyei.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gdxxsspae.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gieqqufqw.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gyojlircf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gqqcuqwpx.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gvpkbopzx.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gupaafvus.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/gjnrmoktb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gntkpkypw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gpqmzwftz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/gdjpmgvgg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gvthuhdfe.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/gydqhelgf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gjcuubmpr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/glihzvfsb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/gpbklpcqj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gczmkugdp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.epnwcf.com/Article/details/gifoehcte.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gbnjiictd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gtazzbdfk.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gtyyfxkdg.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gnvhpnnnh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gilhzjhqj.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gwprrgyni.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/golkbiljz.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gustllkqr.sHtML

JS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/guyresogl.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtxbhbsgp.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gynewzxxg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gmpzgkaqa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/gowvwfpiy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gjldlmvzi.sHtML


<!-- 参考信息 -->