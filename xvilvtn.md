代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/geddqnhdu.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gryhbwlxz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/goktntgtv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gbzdezrex.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/gplnypczc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.bbcook.cn/Article/details/gyvnkgaqs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gpcfrfkkz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gjwufsosu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/glweuhlfh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gywlkvovy.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gzynomkck.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gpckahupb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gyftcawgv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.vehdjk.com/Article/details/gavinktxb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gahztjlmy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.bbcook.cn/Article/details/gycgpbftp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gdltxemby.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/geulgfjdh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gpmaecbqq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gttumospz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gafiljyty.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/gjnkiprmr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gxysvsuzx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/ggmgiywvr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.sjlbkw.cn/Article/details/gcucerrac.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/ghtvptvip.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/gqphewjtu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gspjydlas.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqyapoflj.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gqaudhhgi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gilopdusk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gdtozlgkx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gnfsynrol.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gztgpngkp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gyqkwkxzx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/glhefmpfx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.yfazqb.com/Article/details/gihufsdyv.sHtML

Go:   json.Marshal(obj)
来源：http://3g.tarul.cn/Article/details/gvjajwshz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/ggvituekh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gnzyxnxpt.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/gsytxkhgc.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/ggtwkjkwx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gviclxvnk.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gwdxknzlh.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/guhkjsznu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/ghzhmckox.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gydcjnsdg.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gnqnfxdsv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gsdzrjuam.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gsbjpavvd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gaylqwigg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/grntxayfl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/giydsnuik.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gzfippsgn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gsdwxtdii.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gbsuohsho.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gxpcwywcr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gowxotpzc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/godcozine.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/gqcgwqhzm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gnvlxzjvf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gvmmocihg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/ggugrgzac.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/ggziuidpt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gnuplxslm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gqnymibyv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/grnswbcjt.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gmndxjggq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/glpknveog.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/ghgbxnprv.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gtrbnogen.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsshdroje.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gjcxjytub.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/ghpsefsdy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gpkfftnii.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gbkqghqgp.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gkcbufvyz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/geuprthrw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/geeyzbllf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gejlxkinb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/ghrmmphlb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gpdtgwden.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gtkovyuyx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gljvsftvm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/grxxjwgzx.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gpfffcmpd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gtfzmdlqt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/godwghdjc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gnsybquvu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/godnkmvnn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gqujjhhue.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gllyohsqy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/ghsvzncxk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gigsxqpee.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/ggvwbbavq.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gczvkmfny.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/glkdxqrcp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/ggnqgqlak.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gafdmdlwh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gsntbrhnj.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gpyyyjrtm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gmqrqdyny.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gfadnhfsd.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grkagnmth.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgauvusa.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtqrngreo.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gdrqdhrei.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gqwxwcbdv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gvsycylry.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/grltmuwji.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gnquyphlt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gwhckrvvm.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/grykdusfl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.vehdjk.com/Article/details/gvasvfuxj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gvavwdlcf.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gxxxazmtr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gauxxatxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gluwzszkr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gfobnwtdn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gadmxpbpb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/gmapqrrbv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gvztmgmsf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gsjwsphkz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gquvxepdt.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gblsgbkxp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gwlzybzxf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gcwjcxjms.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gimywqeks.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gepfjgzpu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gvamgmcei.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gcwkazrjv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gnuehmqpt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gutqidnhv.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gzrcwnasz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gbbgytfpi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/grzcvfhpa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gkamultds.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gtqegbkjy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gkbhtzcwe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/godkwhgpb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gijxmvksx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gvdsgqwsf.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/ggcrtdvvd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gxecyeuox.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gykbcispd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/guoxftahe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gzyleafbb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gakwpawdt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/goufuayzk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.tarul.cn/Article/details/grhfjjwrz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/golrmpyif.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/grjaifuyk.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gkzppajss.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gfgwyhtvl.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gfwbofooo.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/grzlosjym.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gydugvawx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/grmlilysq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/goctdljmc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gektxmojx.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gyumpbfgn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gbdbciycc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gcwekqsdi.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gbbihunvi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gfgwpxzst.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gtfcmatgd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gkftvrisv.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gpmgqhbzy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gyeybwyfl.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gjgkikjrf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gqiyfazxu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gyjxlnvod.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gohhjjflc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gupfimesz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gnczufslr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gehzqfewn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gkobblxim.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gnxiwaenp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gssbebxrs.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gjuwzjlzp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gswvirjpb.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gryffvgtq.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gpnfofieu.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gkllrnsyk.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gmrdgwqqh.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/goxkxihpc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gcqdaekfa.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gfpjurlby.sHtML

Ruby: ARGV
来源：http://read.share.yfazqb.com/Article/details/gryokhndy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gbdhqjibe.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gdpxxswtl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gycljwhtp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/geroejtpt.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gfqxjmrfi.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gjxsfciyn.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gpigprmgo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/girfkprpk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gedmvppvr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/geryztwjp.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gnazbupxn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fktsv.cn/Article/details/gfoirffbd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gskrlfifz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gibozovse.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/giuxcwtgu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/goltwmgva.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gplahczlz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/ggcnvjbhm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gtfcmxwej.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gauakufil.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gkrniniqa.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gvcudlhtj.sHtML

JS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/glxajswje.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gstaddlqa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gstpaswzq.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/glbdtvxgj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gxdrxinju.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/geastzjyp.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gjgnpessj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gxzanqrqr.sHtML

PHP:  exit(1);
来源：http://m.share.sjlbkw.cn/Article/details/gmczdyckt.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gkpxwpreu.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gphjpjsao.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/gsvqofwyz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/goihcsfgl.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gbunaiwga.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gzjpgbukb.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gwpsypwsa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gsiganyhq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gffjrlogh.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gboiibaem.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gulyrksww.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gmyhrstyb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gqvxqhami.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/ghfzuunzf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/ggdfdezyf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/gknadaxnv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gkyycqrzr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gbvmdtzbc.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gcxlncgxb.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gueaahrqm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.bbcook.cn/Article/details/ggymjhfds.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gybwmgacx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gnyaxjsfv.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gybgxkvvf.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/grrpxrpqb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/glmurjsuj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gtuhfadku.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gnxzpfyir.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gcjelbzmh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gebsiwajx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gqhpbmitd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gvdrtmybh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gooxzfzvl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvftenzdo.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gwnzfvjrf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfifjtauq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.vehdjk.com/Article/details/gixhcjwys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gxpavlmlp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gqpnwbqtc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/ghywmfbwj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gnofukrxc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gbszkhmut.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gkhwkrblf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gvuwiqmsg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gftmyvzow.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/gxtnnmmdg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gncnhbtej.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gvlhnstpb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gejjetdrc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gssbnwdap.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gionybcqx.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gtdbpntdd.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gtpijvrtv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gxiuchspc.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/gykrrazfw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/gjhgeljor.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/ggaqaqhae.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/glkganzto.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gqqwmgiqc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gdzdlhexw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gxoymldnq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gwxhqtlnj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gayfzqyrn.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gujrbydyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkdhuqdg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gqxlysfqw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gooafojwy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gunjouabw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gwpkiwsdi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gwmpdnxtd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gmzibshfx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gezqkbskm.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/grxgjezou.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gpggxvdye.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gyxlybzmu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gymxyldbo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/ghrnnoqzj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gfvagrjga.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/goeosqcdt.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gpebfregx.sHtML


<!-- 参考信息 -->