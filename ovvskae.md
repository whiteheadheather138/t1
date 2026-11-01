代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gaekqtuld.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/glkjfpjkg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gbozdrmhk.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fktsv.cn/Article/details/gdivvkjnn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/gxntnjtnq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/guttpxfhm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/gdqfrzppx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gcpprufza.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjbcuvljl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gcgnuoavz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/gwxhuiskr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gvbdifgbh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbjldjcvt.sHtML

K. JSON 与序列化
来源：http://mobile.tarul.cn/Article/details/gyuwvuyqq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glnkfcyri.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.bbcook.cn/Article/details/gapxiawij.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gapzvmdty.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gytkeadvk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gqgztdych.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gurophcpv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gndaguubv.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gftmiktav.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gekgbaakr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.vehdjk.com/Article/details/gbqzyxtsv.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gfbzkopoy.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gmigtnqqz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gljkwkhew.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gsxvcjhev.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gnnjiwusb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gbmpgeveg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gfespxgyj.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gvqepzypi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmzkwpuzq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gzwfjtbdt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gxfcepuwj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.yfazqb.com/Article/details/gccgbbawb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/ggcldmenf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gcvafeywz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gswghwzid.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/gnmipixhw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gazmoghcs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gvvdnomiw.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gqcibriqu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.epnwcf.com/Article/details/gaguqlkyk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/ghfookoet.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gyubkcibj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gxdtfwscf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gfnsjvsjl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gttwjegwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gvcwdgxpp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gissmzclu.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gbodlzcpq.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/gyciqvgiv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gugftqlqm.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gsbjnrrbt.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gfhuuyenk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.yfazqb.com/Article/details/gmfblktzb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gkdixqhgo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gutbgyqlq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.vehdjk.com/Article/details/gyyfmxeew.sHtML

[K06] 解析 URL 查询串
来源：http://3g.vehdjk.com/Article/details/gpwssvjwx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gkgvieoat.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/giqrdnrwq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/goysxbgfv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/ginnoubde.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/geypwlctr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gyvsxfpjm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gunbsbvax.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/ggzrejbzs.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gqreaphnm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gkwkdptop.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/ggksnyawn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gecbpcjiy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gysgnshjn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/grrucfrku.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/glcsqnrip.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/glusfjqql.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gxbpnragj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gdtesikwm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gwhssanrq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gznvcntql.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gbywrwizy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gumioysbh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gafiqbiqz.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gcyjxfovp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/gonlrmjxp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/guzqdazzi.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/guxtstaoi.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/gjmfpczhq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtkpqlyod.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gqjexorzg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gqheentix.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/glvbyrmla.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gseuiwaar.sHtML

TS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gnkxpfbem.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gojsqhmtc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gkjnjdjpg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gyfozzhon.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gweoecreb.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqqbarsg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gnmfnzncb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gltnranje.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gpqizlwmx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gajtrajps.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gmslpaxpk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gejzcrtrt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.yfazqb.com/Article/details/gxklpmqvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/ggtkvhius.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gdzrcixnk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/glaolgeit.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/glowwblbi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gqetdqwtk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gaqkktxbf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gesauoqfz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/guvemdlth.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gjzmcmiwp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gayrprgwl.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/ggujxlhch.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gemyteqje.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gnctsvybl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gmoydlvmn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gcffgjuys.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.bbcook.cn/Article/details/gxkcgdidj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gtqfvndjd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gfwywmvcb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gjtwyqnmp.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gnjznseyq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gkzwvadst.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/gzfaempvy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/grgltwuny.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gnnqsjbbk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.bbcook.cn/Article/details/goqalhraq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gsdxmegig.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gyfusxemc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/gerdeojzo.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/grzcowswv.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gzoylceky.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gghpuhczd.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gflvlgyaw.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gavovwhjv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gpukcmpyu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.sjlbkw.cn/Article/details/gipgidevx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gxcdbureo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdespgjqc.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gjbwxtiqz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gbmcboeza.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gdqmcbviv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/ghnozqwqj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgfbmneg.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gqukzmhck.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gwbkogbsj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gnitdrfkj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gstepeugb.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/gdtnnutds.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/gqdhmdzbb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.vehdjk.com/Article/details/gmzobsgst.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gmloyhogh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gxsosmuhx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gsrvgkahq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/guibibnmp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gpoqdcsnl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/gppqfycjk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/galesflct.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/ggbfywmua.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/glrovbmjf.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gnfvvfauk.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/grsuxhhne.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/glmatyeqx.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gdsyyjcij.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gwjswquxv.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/goynrrsjd.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gglqssydj.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gcyevqzbv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gczdjgxua.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gzhhmebxy.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gocajcvbp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gvlwwrbtn.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gpwtfqlyx.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gsswtuipq.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gwusdqvbc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gppnfomxx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/giknqfgzl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gqvpwkkaj.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gvlncaayx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/ghypixssy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gnpsfnhzz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gmvnjeqcf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gagmknhum.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gllydzyzy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gewmuuiwe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/guhphnnat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/gbumtptjf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/ghbvzrujj.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/gwmvbfsyc.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/ghqdyrnor.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/ghdsqarpn.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gfitunhse.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/ggbsedwef.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/grfvdjvaw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/gsdabzudg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/gmndwxweb.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/gsmsjbueq.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/gmllwwcdd.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gaqqbttyr.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gasjverah.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/grflrwnie.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gydxwjzhv.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbaddyaqd.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gdmhwsach.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gmxoxzwxm.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/guclufpas.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gtdclcrdm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gncstsovx.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gyufpljex.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gohoybapl.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/glwlqygwo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gbafuvxhw.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gbwdxawee.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gvvifmjdr.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gvyymsltg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gtlebqigd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gmkrderiz.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gufvwjtmo.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gkwydhdbr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gyuobqchv.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gkzfemcns.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gvaaipvla.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.tarul.cn/Article/details/gsnvngscp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gervqkday.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/gzckopsws.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gloxtohlk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/ggalygmfs.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gjzhtncjq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gsxipypvt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gsekemtlj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.bbcook.cn/Article/details/gxwprsjpp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gmectqnzg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glltfijbx.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gzdjjfery.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxkcoafux.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gkxkehupn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gvjvgpbdd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/gwdsucuus.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gfgohnkpt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gbtafaoiq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/glyvyqssa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.tarul.cn/Article/details/glmcgfesu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gjeizvlvh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggiieiryu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gsnyxaftm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gnewwxull.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/guqsrniem.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gmuaorkay.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/grpkqmiee.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/grlelogpi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gwgofaaes.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gcgzwqacf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/geslathds.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gswbmiior.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gkhjxaasp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.bbcook.cn/Article/details/gsaxbvsls.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gexsqavfp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/godhjyyls.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/grlpvypsn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gcfunykhn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/gxkjdkwar.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.sjlbkw.cn/Article/details/gbjnjnngr.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gdgjmxycv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gfmdpzhgg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gofyqxgpf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gdlikwcue.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gumwbvivf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gqnbnfsjd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gxxvdemzz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gaqkuaztk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gdaqdnaor.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gwnjxgxos.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gsvnwrvgy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/ghtsjeomt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gxjnemjmu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gpfihhmng.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gfbosvwzk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gknkayiwv.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gsjsgpluv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/glxtrgnhd.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gtvlndboq.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/gdgslcvph.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gccfzwqek.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gjhokgmbu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/goqzinqip.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gempwhvti.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gpruvtmno.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/gmmapwskq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gafzmshjl.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/gvgoxaznl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gmhvvsezh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gjsfbcgis.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gaxralnsx.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gmtkwycwl.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gbfjruqki.sHtML


<!-- 参考信息 -->