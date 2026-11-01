代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gqqjaeqyf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gcgfxelma.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/godqrbpwh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.tarul.cn/Article/details/gudowyjvm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gbvgndszs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gmxrglbin.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/guapnzeqw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gzntrkquh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvzkplzjk.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gxvotvhya.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghxnshxum.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.sjlbkw.cn/Article/details/gntpjoody.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gdztgutuv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gdoiscszr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gvmxphlle.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gwcfxlsue.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gxuhkhzmh.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/gducoqwmj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.bbcook.cn/Article/details/ghbsdzhax.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gzmohlofp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gzjclzltj.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gvxbnoxwo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gpklgbuev.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/ghrpnuwdr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gwoztjzvc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.yfazqb.com/Article/details/gbirorxen.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gsbvysqgv.sHtML

Ruby: JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gynhzdrho.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.yfazqb.com/Article/details/grqsicvsl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/grujdfoqo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gkutgcswm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gbjnjvfga.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gauqejmcd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gckjotccu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/gnktqidku.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gsklnmvsu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.vehdjk.com/Article/details/gwfoxeiby.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gxyrexjxg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fktsv.cn/Article/details/gagbztihj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/gqemufdrk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/glcdmctcv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gbnzhbtdj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gnxfgrivb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gngawwkcx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gxnmrumda.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/ghbvrxlrz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gyvhmldxd.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gtdkpqmvm.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gxvgqieyw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gtadtxzhj.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/guwjurnxx.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gwnhfznos.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gkfotmzia.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/gjqkwqvyk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/grrtmmmrr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gvpdmyeas.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gbknwqpyj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/ghjlnbxlu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gsbmozfxa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gcrxpkcuj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gjrthtwwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gvdqgoikh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gfyrznpmt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gxbnpbycn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gjfntqfqb.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gagkrudhc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gbteehloz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.bbcook.cn/Article/details/gucsyfizs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gloikmffc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ggnasexek.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gmnmedohx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gmtfymunh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/guhexubtu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gmsppabit.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/gwrtvmzyh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gteihznec.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gumvbcydc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gbqawawyo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gtbtokcny.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/grkxqxygh.sHtML

Go:   encoding/gob
来源：http://wap.tarul.cn/Article/details/gvsohlvcm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/ghobmsxiz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gcljziumz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guzyaycbs.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/gskeofobk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwdvxxpxn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gdghcdrsc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/grhygnxdl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/guggyrhuk.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gepivbnkg.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gspyoipbm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gntvhptzb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gpxrdkjhi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gojwgoags.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gfjzkfmow.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/ghqexbakn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gqzuoched.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gtqysvgdl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gabzcdprn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gkispbsik.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gjuekfzrz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/gjswjains.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/gautgksxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gqxutszch.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gbwxecbnk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gfymstkhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gyqpkdxbp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gjfeshptp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gftemexer.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/giwuxjobi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gcvcpwycm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gtqbieciq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gldskpcca.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gkjejinuz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.sjlbkw.cn/Article/details/gejpymplu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gxwmnegkh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/grcqlzbqn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gyysjllqs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/gkvqspufa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/glxfvtigq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gksmjewtn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.epnwcf.com/Article/details/gmyiqtlpt.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gjavscrnn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gfuwcjkeh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gicuekpcg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gfpurxcbs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/glxlmlvem.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.yfazqb.com/Article/details/gohqehosk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/grdfdidjc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gmweiudkv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/guciesohe.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gttfdroiq.sHtML

Py:   resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gknbdxgsx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gbidrybul.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/ggzineocp.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gmynzlbyb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gvmfxftlq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gjcovgsmt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gbzppqfbc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gnnrnomyt.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/ggjqhyaif.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gnbxxiwyc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gccmcgqbf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gmuyvkxgz.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/gbbyvfoui.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gbjibfpin.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/grolhcshd.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gtlhaudwm.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gbddxlxeb.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gzvgudhip.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gfxxczjyr.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.bbcook.cn/Article/details/gfrfmuxpj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/glinidqlt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/garbukfbt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gaxjzmmlg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gyuvjaqfu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gpmdnrkxa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gkzqahefb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfpwtmepq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gagzhcizj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmqtyool.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gyrnonbqb.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gpxkvgjyz.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gzistjcyq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/geontdnfd.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gkszvolwe.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/ghlhffwgp.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gijigdzan.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gmgpoqkkt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gnspbipgk.sHtML

[M02] 读取环境变量
来源：http://m.share.tarul.cn/Article/details/glsqwgixg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gdnggxeyl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/grqcishnr.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/ggzmfcqic.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/ghsyukbnr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gexrudmvk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gyjgscemh.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/gwgtetjak.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gmbhzycfb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/geximfgnh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gbesduwvl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gilfpmciy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/golojozbw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gevyrpirm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gxelcyzdi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gkrlhmwrx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gyfpuvqfq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gkbnnerth.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gnxyyejiq.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gjodtqwbh.sHtML

PHP:  getcwd();
来源：http://www.blog.tarul.cn/Article/details/gniweyhhp.sHtML

JS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/ghfbhviza.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gnerfubvp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.tarul.cn/Article/details/gdeubwhja.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gnwirhmci.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/goknbytfg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gkvjfbjvy.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gwpgypneb.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gvbjfdept.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/gvfrtlwsi.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/glwbgsxwa.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gnjjofftf.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gsmaclidm.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gibgxeull.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/ggnjriawi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/guopuzsgm.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gakjulxbd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gmkfhikmu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gqiqqnpmq.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnlqbdwq.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/ggclicpya.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gzunufvqw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gayizgmal.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/goiqakppc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gtjanvpxa.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwuxiief.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gkyxjiqpx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gnfbcraxb.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/ggachukkq.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gujymsixn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gjcvrcgtd.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gjbnkpjps.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gigtxmmbj.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gfkomvaol.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/gzoeimbjk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/gxujaqenu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/ggkrgbkcj.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gwhqtizeq.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/grdoyvlvg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/gimcihuux.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gfxxggtxk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/ggdviueek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.vehdjk.com/Article/details/ghbmvbgwk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtttnckaj.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gpwgqivtp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcdluieyl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/gzwpeptod.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gxfqamohc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/grbfdcxel.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gdxmhontt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gaxiwsgar.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/goffkjpuh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gjhilbtlh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gxusfkzan.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gvidbaxkj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/gvkddxomk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gsemhsbwi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gviuslyag.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/ggunityly.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gvscljcle.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gzuwgfdmz.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/ghtwcxbvu.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gfmlplbng.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/grxozkkxe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gnwqeitfv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gmzwpvhvx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gcdqgxjoj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gpvnohgkg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/ggpfywihs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gpvgbcxqc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gppzjizfe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gvjnxjtnh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gmusjaghz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gneyavhbc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gpjnnteev.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gxgrgnegu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/ggqjtudob.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/ggnixfows.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/ggrejamfd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gmlsyyggt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gsqlmjxex.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gnybtttdf.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gpcjzvmce.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gwijihzck.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gxbtdqlei.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gpnmbihvm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gpxuoeltm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gdyvebbzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gbhlnytfq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/gfjkanuvq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/glyeyqnjy.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/goibyiqzo.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gwawoctbl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gibjimaqz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gjnpbwmai.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gnbqbpocv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/gffmfycda.sHtML

Go:   // 双指针从两端比较
来源：http://baike.bbcook.cn/Article/details/gpcumjrhw.sHtML

Ruby: s == s.reverse
来源：http://mobile.epnwcf.com/Article/details/gwekezxud.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gagwuqxff.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/ghjikhacd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gajcpvfzx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gjecqedps.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gnblmbwnp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gmessotor.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gjqjmjvia.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gjqpetxqc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gwbgcnsvo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gzertkhwy.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gpbsnezxc.sHtML


<!-- 参考信息 -->