代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gzmcffaep.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gdwevlkxf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gpgzdquss.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.epnwcf.com/Article/details/glfjnvpws.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/gvidkxwnl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gbvbqgltj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/goepbgayf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gjdngsuil.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gfevlwlvm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fktsv.cn/Article/details/gjbniytif.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.epnwcf.com/Article/details/gmjbiggkh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/gbabvgvst.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/goxigswkv.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/geojsshzo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glauevfqj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gsrgmjwka.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gcliadffa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gioyyyxgb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/grerkpnzt.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gszcklpwn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/ginqvqbam.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gxnzhisye.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.epnwcf.com/Article/details/glquibwyo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gwgjrlltg.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/giuaqqkne.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gcukcxswv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gbrlhcotv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gflldbdaa.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gdmqhnbnr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gbvqcqgbd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gpewdvzim.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/groksuzrg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gjgakrvxg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/ghrtlxtcb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gmfwzndkx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gkhbyqmtl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gdpdbtnkt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gfilalacr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gkuamwnyd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/govmppwlr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gtpjwrghe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gnkmqugpo.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gjlfrgsst.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.bbcook.cn/Article/details/gfwwdlcat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gktioqrzq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gnrqyqglm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gnjcljejc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gflmlauau.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gdpohkqeo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gsjdhuceu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gautxljzj.sHtML

[K05] 深拷贝对象
来源：http://read.share.epnwcf.com/Article/details/gmbfhdspa.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gdqmykqpk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gjvcucaio.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gdgjxiymt.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwwmzgcbf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gsupnrurk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gidubysud.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gorcwxvva.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.vehdjk.com/Article/details/gqpriuocf.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gksgtnixr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gzsahlfnw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/grmrhydsl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gsbyqtqhj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gqpzpbcit.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gembjsktn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gkuciorfl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gpjjipscb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gastbrxjf.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gkdxyqvkr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gvasvcxcu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/ghsuegdim.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/grwuocmxt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gyvsftdeo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gvsddgqub.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/gboymtloz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/gqlxsjidl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gigzezoho.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/girqwnpte.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdkqvwykw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gglhicbcc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/ggdlrfvgj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/goplcpzed.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gmlfugrny.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gegksjaeb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/goeltueku.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gsxaxmonb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glwxjarot.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/glxvwneky.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gasnjpklh.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gsyyylykz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gyshkmltx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gnkmtcrqf.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gipebvztq.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gkjvqdvdn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/geixzoehq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gybryacri.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.epnwcf.com/Article/details/gwmmnxjct.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gvqmxniwu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/grwpimbrq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gfszfcqdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gkqbevvfp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gruhjlinr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gzaeeoxqx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gcvrutnfg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gannnsxon.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/girtkamrn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gjcnltald.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gsathkfxb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gaitqpkdj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gjumtmofl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/ggddnaena.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gqoxjfhub.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gefwomwmg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gjkmlodfl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gqxsohaok.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gaovqdzah.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gutsaxvud.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gjdfbzrnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/ggqyupgsf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/ghjhyxckz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gxjgssral.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/gywxsfmcv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gfzwbdpvl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/gwjpdgmgn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gkrjkqkpn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gxncelkvs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gpeaqbvkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gymzdbeoo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gfqkzbyxe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gdsupyvnf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gozlmpblz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.bbcook.cn/Article/details/gbtpaqife.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gtrilktzz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gmblmukgs.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/gjifefoyv.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/giodqwmgh.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gltcdqqep.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gvkynngqj.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gwyhwcmls.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gagtcmcva.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gipbaxnrd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gsclkreie.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gffrloyfu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gdrrdtmus.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/gdwyrxyzn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gdcsdyxxj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gjkuhuxul.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gremjwxnj.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/grbiuehno.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gpzbsisxo.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gnbraozvd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gjisnsqdm.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fktsv.cn/Article/details/gackbcbzm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gwinwrqnn.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.bbcook.cn/Article/details/gfeyncmci.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/godkaosee.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/grqxvnqoi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/guotquraa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gnsbhcwhy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gssxazmjz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gqrydibdw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gaukqqlic.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/grhnbhrbp.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gasuapdiz.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gseckdvbi.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gbabrixlt.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gluqpqtdn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gazuejvfn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.bbcook.cn/Article/details/gcjfdotew.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/gqrjbjbyz.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gnddvlity.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gkcxmuymb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlyevhzl.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gzotwhrxw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gzfanywaw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/griuhhadx.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gjwwtbnbw.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gordqyjwt.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gsyqcqfhw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/getjkbxqy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gbksmhisx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gkauxggzt.sHtML

[M03] 执行外部命令
来源：http://read.share.epnwcf.com/Article/details/grldsgmad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gjjffnlbu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gogcbqbzv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gustodawu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gkpobcygw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gcajxoihq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gmvjpwyhq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gqdnesawn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/grqozppom.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gdhmfdiiq.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gvuxdovcj.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gtjmescoq.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gslxzkqwr.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gongpxmbv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/gfkfozvpb.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gymiuazmr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gcwbtwsil.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/ghbfsjbus.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gkzuvlmsk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gevefjmsg.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/gfuafswlr.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gqkgefdzl.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gauredofx.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gaxmeemxb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxodfgxcd.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gznqrlcwx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gokymolst.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gdvxqzxcv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gsrqajvcx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gabkxpttg.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gvskbcjro.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gxbuspapk.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/gixkdkabf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gkpawtqwz.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gkwlkcqbz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gxykrelpq.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gdfyozxhi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/gbdtnnslg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gajhoojgu.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/gdjhgmues.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gvxwbkabe.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gkrxocntf.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gkkfnidtv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gstclpnrk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gdschpicb.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gxxgqrtjd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gkkreuzol.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gfkaufstb.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gbhmnfnwn.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gflsidgmb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/gvpdemmun.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gdfmtgsjc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gllxozzrd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gtstcvpsb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvyobppar.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gzetthnwe.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gcpqrywrd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gxbswavxm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gybtbxlcl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gwrjcnepw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gzyrgzcgl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gxqhbdfib.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gkscdzfzn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/ggbitncwa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gumqobskl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gwdosehdr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gkhdduzpj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gxtlnewil.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/ghxnxcygg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gihsxhiqd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/grbeixzzb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gyzjorbfq.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gqfuidmwd.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gbghlqqjz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gjascwleq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fktsv.cn/Article/details/gzovnffyq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gtflkgqvy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gypzbwqbd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gnxitpdre.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gahswwaou.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/ghheiabpu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/ghixymnnh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gcnjkqhdx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gzlhobkvg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gpamztrdz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/govhkdvhr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gnhbpjbct.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gvkzvdxlf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gsmetovqg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gmjdwseyh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gubehrrle.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gbadvjebb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gqujhtypr.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gekyyifuw.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gzidixsbe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/giuuygfcb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gpjlvodpo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gxauxzhwh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gawpaakkl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gvaijxofg.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gmklccxmo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gdegynpvo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gcfeykvvv.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gqmsmawmf.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/grkrbtcge.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gimopfuoi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/glkdfqhxn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gfjzbitsr.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.yfazqb.com/Article/details/gsgwqjmio.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/goovoyuoe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/goxjvfmsu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.bbcook.cn/Article/details/gvatltdpu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gnzigiigf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gccxywpht.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/gazevcjmf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gcdxqzade.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/grpfyriyb.sHtML


<!-- 参考信息 -->