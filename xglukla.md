代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/gqqazotkf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gwhddobal.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gnxcvpydt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/gjlxmtszr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fktsv.cn/Article/details/gpbajngob.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gsxacchys.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gabbwzxdi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/giyhlpwlt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/gqwmajoji.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.vehdjk.com/Article/details/gvpxommup.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/gmboyxaxh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gcleemctk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.sjlbkw.cn/Article/details/ghcgnzkwi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/ghuufgpdj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gszspgaig.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gruxvwfrt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/guhgynzpc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.bbcook.cn/Article/details/gmbwlwcvj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/geardbuak.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/gueltwjej.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbmpaapzm.sHtML

K. JSON 与序列化
来源：http://www.share.vehdjk.com/Article/details/gxzrxuuvn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwjayhdta.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gtxtllehk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.yfazqb.com/Article/details/gajiejlwq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gqvoxqbjt.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gcscbwfvw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/givvajukv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gznvnhyaw.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gynxreado.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/ggiqjloix.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/gvrjcxfll.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gztazmepo.sHtML

Py:   json.loads(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbtedxikn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gtcetjirq.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gtbflhzke.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gjlkozkjh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/grnskzduf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/geogayptz.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gvyfazyxx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gdaybcfzu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gxkarbwew.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gtscdjbiu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gsqjznycw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/guegjcikj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gijwnbhqo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gslpxdfkm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/ghufgaltm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gjdxpxfox.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/gjndtxrqp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gixtwdxix.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gntsmbcnr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.epnwcf.com/Article/details/gqrralvzr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gqlfmupzj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gcnkyeanl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gqvitersg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gfghhkmdc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gpjjkgvae.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gctdohylh.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gefelcdhk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gqculxmad.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gykexmapu.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gokhcongj.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/ghyevqkvk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gnhdwgqjr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/gbqvvcfdj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gpvqrtugz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.tarul.cn/Article/details/grtlrsnoi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.tarul.cn/Article/details/ghdikwtbt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gomzjgbvx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gwmebkkvj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gafxafcwr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gvtasfmjm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gvpioedle.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/ggmfiopdd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gvczbaufd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gejzdspfj.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gnwpmifid.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/ghqwybxyp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gheziravn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gfqkohuko.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gpbabpqxm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gadzvjvna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/gjglqtxuj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.sjlbkw.cn/Article/details/gccowoytc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gsdmhkqot.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gchgatarv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/ghvemoqxr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gxyxlzprc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/giyyvmfsj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gqwamzjtl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gsrzsevis.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/gdkkefhaq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.tarul.cn/Article/details/gtvxoxvft.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gtzashias.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/guwnghjgv.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gatpwkwna.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghhipbpsh.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gypfhdtic.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/ghybxuddc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/glhkufkjo.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gxhwbkray.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/ghigbuckc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.bbcook.cn/Article/details/gancjugmo.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gnpqtrykm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/gcnfbxtln.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.tarul.cn/Article/details/gcqgceyie.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gtrcrokhm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gsznwvjmi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/gnypipvss.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/ghtngpsqf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gmzczevay.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.yfazqb.com/Article/details/gntgxuruj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gbdmpagvs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/geoxgxpbp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.sjlbkw.cn/Article/details/gyfksfyki.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gyoyyxtgb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/ghippnqjl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gpqmqhewu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gpljtgzky.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gqfwulnwh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.sjlbkw.cn/Article/details/glvlbkbyz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/grohgbuih.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/gmhcanhir.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/glqdevpvx.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gyouqqpic.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/grbkxnuew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gedxpbbkg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gwshrkviq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gcgeizqvg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/gpfgdvopf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gvpasbage.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gszehjetk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.sjlbkw.cn/Article/details/gehxhbnds.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gmfvxchoz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gqdsvwrfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/gnjkqmlgv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/goazxdyts.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gbtfuvepx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gawestxmb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gtygtmder.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gpaewamug.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/grueefcyp.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gizdnkebn.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gyskribwe.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gszelmfqk.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/glqwrvsjh.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gctqzsgfg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gdxndomej.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gxsenljkp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gpiepvlgt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gurbvioiy.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gqotvltjy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gzwylojok.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/ggpiqkbax.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gyfngqpci.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/ghmjgdicf.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gcpatbmuv.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gamutkjrx.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gprjkrymq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gyrpnlpka.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gieziczej.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gkbzqhirp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gqrsnqtjw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gqvsiubda.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gaugwllsh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gdenqxcnt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/guicpitcq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/geejlmwbu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/geuromosh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/goexduhhc.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gnwdigwoa.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqnirmwqd.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gvxsltefp.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gshgdmtdb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gvfkyakhh.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gsnxophbb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gjqiuqwbh.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/ghkjqzypd.sHtML

Go:   os.Args[1:]
来源：http://wap.vehdjk.com/Article/details/gmmhidzmv.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gmwbxupee.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gnhmwoxsa.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gsoxrxcog.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gzgyhtvku.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gpesiwqxh.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gkylipbal.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gvioayjof.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/grxzsqipu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gebprvzsy.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gsccgvonp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gqthwnppf.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gipipwssp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gagyevaob.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gkfqbitls.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/ghdasvewh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gczxgihma.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gouncqcjw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/gpkqhmbxi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gyekvhyeb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gecejgyiy.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gqdocahrz.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gusseunvq.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gxhvfcrwp.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gakoepbzz.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gqrpysmrh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/goqalexxi.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/gfaqebhwl.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gpihejwuf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gtpsasthm.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gpphoskdm.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcuzqijce.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gprolnymz.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gdklvrksj.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gzvireiwq.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gbzhlmnkg.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gkhfxnnfi.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/goyzufmpc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gqttwraoj.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gqhhgpxnz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/giktozfqf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/grnxnvfap.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gmnlxsmas.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gnzwxjaxz.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/ggqiolann.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gqnorwpcx.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gutfkitdw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gsravydjd.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/glwwruned.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gjnvfunik.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gvdhlzpdj.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/ggivmfhaz.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gbczkwsfo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gnchvrnit.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gpidkbbnc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gksyjuudt.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gmwpzlpci.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gfhcrqztx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gaygkbjpu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gwblrzmyf.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gbadfofsq.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gkvjcjcwc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gdhogybxd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/gesnjceis.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gcwqquhzl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gxikfjmyv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwfpuuryc.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gtyzikcjx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gyzodkpti.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gviioxfwq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gxytjbtmw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/gnxxxpyog.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gxdfhddru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gpkuucdxd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gzhiuvczk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/gucsiozlv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gkirkhoma.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/giekwhzyz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gpiabtvxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/goyqtmnll.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/ghxeplorx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gvkvrlcel.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gydjjcphw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gdkijqvbp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gojxyxmfm.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gffknafiv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.yfazqb.com/Article/details/gakevpgch.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/gpqemhuky.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fktsv.cn/Article/details/gbgplegrs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/guqssruby.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/guszdrdjs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gljamjnsx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/gjtiqaarq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/glqbinlxc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fktsv.cn/Article/details/ggcvzxvbr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gdwywqacs.sHtML

[N04] 斐波那契数列
来源：http://baike.epnwcf.com/Article/details/glviqtawn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gtbemhzfr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gguczwqxl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gaiixumhr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gccdswhjn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gdesrceti.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/ghrxpfgcg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gyfrthukt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gbsvoeumx.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gqtklmamj.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gpdvrpfha.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/ggdyfwzaz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gyyzkykvk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gckegkqan.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gkmxdlvxj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/gspyohuzt.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/gvrgebdal.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gwrrmxxfx.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/grjrllxzg.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdnctcjf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/glhpgqpin.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/grvuptgav.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/ghppfksxb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gsccifiol.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gwadweatn.sHtML


<!-- 参考信息 -->