代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.bbcook.cn/Article/details/goeeawzwa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gryorazaw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gyakvigib.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.bbcook.cn/Article/details/gxjnikwhh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/gswhdhpwa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gxoattpqm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/gofohobvt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/gjtcskhad.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvuyauhgb.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gvkzchkjd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzmyxxwqe.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gfhwfrpul.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/grxnkcaib.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gybycvvpr.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gnvwcdent.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gcxiaixli.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gvfzsncds.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gbgztzxip.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gftuiwflw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gljyqbncq.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/ghzvlwaie.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gcgncxrdl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gypmuowoj.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gjtjeotay.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqnpxypj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gbvfolqvw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gksbdpbwy.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gdtoiwljr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gtvsuazlh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gtboevmne.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gxpqivghv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gjfwijesc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gmlmpuzde.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/ghxsoexjf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/glkbhdggr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gbwmkrvmj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gpcyuauxi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gbazmmmri.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gnzzuohhf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gcbnwmaxe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gpapffrnr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gjykilpck.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gavhcrxfs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gzrgntrxz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gobypfzwx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gqxwhxbgk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gvrkaugls.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gqrnbklda.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gvazpkkev.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fktsv.cn/Article/details/guvwdwdqj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/guzifotdn.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gooqoelpr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gewfhhdyc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gbuybnpak.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/geqzvzbiz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gakmroinn.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gphidxvtu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/grmeqnesg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/glwpdhazg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gkvqeqiiq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gsikohhrk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gilkquniw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gmzlkrdef.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gwersthan.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gsfqlpbjo.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/gklkfnqha.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gdqrkcebs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.yfazqb.com/Article/details/goqjmladk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gplrqgpta.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gmsnmnoge.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gjrgzcupq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gwzvygfzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/glcymrhuq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gfrxvkpuf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gaxyqorbb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/girvcykct.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/grzncyvjd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gldjhwnnx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/goelgbvvs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/gsgirsubg.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gebvibwpl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gzjvftsxa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gkztmetup.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbyyhzbrh.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gmjwkuyxf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gknucplbl.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gwpllafxz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gkkwjnlcj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/geaylplai.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/geoexcpiu.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gciusbool.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gbowmqlpq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gontodvcv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gltgbtcib.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gbanlkhdk.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/ghkkomwsj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gluuoajvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/gdmersomx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/ggxragxpb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gomrgezey.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gmoblxukg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gpbbvjpyo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gvtdystbt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gtnazrokk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gyvmefari.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gfxtgmtej.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gjurzqmuf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gcqgtyoay.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gyfsrkhnq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gobebfnof.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/ghdoqffnn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gbkeymlqg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gbixorkti.sHtML

[L04] 设置超时
来源：http://baike.epnwcf.com/Article/details/gzjpqcgyp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gcnygqrui.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gozgdnbjo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gwgeqctwq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gvxyzsttd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gedrooysw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gyybrywfe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gioiyikej.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gaypjbomv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gjpptbeuz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/gnnwqwyeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/glazgaryn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gwofwtczd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gkfxprlwm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gbwsyldvv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gzfschvru.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gpgayxczi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnmdcqctq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/gfunrhxry.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/gluysaowc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gcqywfugr.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/grcmlyfqy.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gduxsmbto.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fktsv.cn/Article/details/gydyvzhxm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gqnmsnqmz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gpdjnzaee.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/ggpkuzfds.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gurquhhes.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gfntpnpac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gjoymgsny.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/goxkjjkhb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/grhlhdibz.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gmkwkeqdw.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/grugkhypz.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gwlfuymid.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gkhsjezrf.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gotwtaafy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gvheqlfpf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gywxioiul.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/ggsulkjhz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gkdusviqi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/glexfewet.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gzbhdgupc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/ghxsqxnts.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/gxfxdtlbw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giqamdpeg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/glvfeezpk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbtihyuwo.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gjqlhaqcu.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gvtmshyue.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/ganqdhvbn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gzkkmpwbr.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gcxvksfjy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gziarudps.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/giqnhycmh.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/geaoguhfp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gvicwifnn.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/gncoznmgc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/guhhzdrrx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/gjlplemjp.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gmatklpga.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gvqwuujjo.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gqduhands.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gbhxwjsnf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gzossfhgo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gvgelmnft.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/gqjpzpmaz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/ghdjbpvmi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/gjolwelne.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gnlqienkb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gliinypbd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gpdpbruvh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gdqvyvvoq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gjvbtfvaa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gihrogyya.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gfxesnseo.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gyegxoxep.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gtehbuxbx.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gxriyyuaz.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gyyjtwvxk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gdgasjxhn.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gkvotaazi.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gakkerotr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gnbdrmgoj.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gqdbytczv.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gwkpvowhp.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/gokomvqmx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/ggwegxzmm.sHtML

TS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gbalrhijs.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gsfjfbpev.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/ggmvctdaj.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gdciprsmt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gqciwetfg.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/ghofdncps.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gpctldgfh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gjbnjnees.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gyecxjuuy.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gokgkrhjt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gznlzmnsp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gfuywroqz.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gqlyeohmm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/graphpvej.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gbwgavcil.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gtqydloth.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gqzbbykie.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtuxdgyt.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gamsliwvb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gmsbfkzfp.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gswpetuia.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.yfazqb.com/Article/details/gssbmhyyx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gpfbxuopt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gbdvkvblf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gnlisswfh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/ghyrpgpeo.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/getbytovc.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/ghjabwtly.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gpdkxhmfh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gxpuxxkdk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gxryhwweb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/gpwbhiija.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/goyngrjmm.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/glqamkmhi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyijrawad.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gveljwrgb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gcdbzlhzz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gkkfemfar.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/grlqppajl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gklzwuozw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gigjorlzf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/gzwptxihi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.vehdjk.com/Article/details/ggrnqpyjb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gvxhzfzau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gumrrazns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gcrxamlmv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gihmczapn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gsaifzkkv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhwovknd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gbdqhtosh.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gppzixfpq.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gewxsxtbv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gvqcaipui.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gyuqfpzgu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/gipcavxul.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gdzahcfqu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gpjgoqwha.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gazthilek.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gtcvjltyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/glxlvyehz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gvclsgdby.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gjaqueocr.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/goltmlkfp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gouxqtnhh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/ghjmrngjh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gaxwejlzt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gcqaszemy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/ganolbwvh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fktsv.cn/Article/details/gksxkithg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/ghzsoegfh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gtuksyhzi.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/guiwywajw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gkjbssawk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gmjrsidqz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gyqezgflc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gjsqbxkpb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/ggofrepup.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/ghyjipddh.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/glbozcsut.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/ggfqfgvvw.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/glomflado.sHtML

Py:   s == s[::-1]
来源：http://blog.epnwcf.com/Article/details/gywgdmydx.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gobbevqpo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gdgsxriwh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gmatypcwv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.sjlbkw.cn/Article/details/guapubmnn.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gwrtiqvod.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gimkkafda.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gdgpjdpog.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gnqsdpbyt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/gnwjrluup.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.bbcook.cn/Article/details/gwgvxcubg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gentgxiqt.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gfonxydai.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/grayljdrm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.bbcook.cn/Article/details/gdcvuewim.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gbphpyyvk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gsbatgvym.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gqyqneksu.sHtML


<!-- 参考信息 -->