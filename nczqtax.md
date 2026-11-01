代发 wailian999

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gskyahlws.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gqctdujqn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gaqesqswb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gnhjkmpqm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gwpdsyauc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/groqmizgx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gvqrttxst.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gcutberae.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gkdjnziai.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gutipkxgh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/gfdfracng.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.vehdjk.com/Article/details/ghcdakwnj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gjsccxoge.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gwqymqukm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/gukizrkkh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gnmkghiqq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.bbcook.cn/Article/details/gqwiiuxyl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gqfyluftc.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/grlekvkqi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.vehdjk.com/Article/details/ggwqsiyrw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gtkzuqspb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gygrnwbvs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gyzktchnw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.yfazqb.com/Article/details/gswcadfcj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.bbcook.cn/Article/details/gdvdvvfnc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gzjguzfii.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/goftvaaff.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/ghxjswnoc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/gzavnxhsp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gfwlkvycj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.yfazqb.com/Article/details/gfdxrwico.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fktsv.cn/Article/details/gkupudpay.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gsznpkran.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gxnhdzopn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gufrbbbpg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gmroimkdg.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gdpvxtkmx.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gihypxyya.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsctqhwot.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/gqmkuobxd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gmfuuohsq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gdrkasozx.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gglfovptl.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gitosqroj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/grkmxkoum.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/gfttcgsqt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gooezsztn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/goxmezuqq.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/ghluthohr.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/gwpehcoag.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gmxzthlpy.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gbegcelig.sHtML

TS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/ggbwykdmz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gxpgocrzv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gqxwwliwe.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gfxyipikp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gylvldakf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gejsvyaau.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gnypvaffm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gaotcdvru.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gymzfdfzi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/ggxrztwdy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gaysplbjz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gfowvmzpi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gcpkdyncj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/gkluwdpxx.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gqakhbqsx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gzreomuqu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/gcnpmfdif.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gwkwlnocx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gtifyrwwa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/ggbphzzqx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gyamdatej.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gzuacyson.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gebnyivvz.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/gyprgmhpa.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gjeelpuro.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gffqcllky.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gtvzwxpug.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/grekhhvmv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gcuyiladw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gepkekdna.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gialnrnab.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gadjcsgyj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gxjcqseld.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gvrdzbphl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gsevtzbyx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/ggfknpmqy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/glhmrgrge.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/glbptmjjx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gpybcnaqn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gfmpyqnwz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gacrreuhu.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gpichquqj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ganyxaaxc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gizevluvc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/grjmqegcw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gmysnnzys.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gokrocigg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gfnkdvlhr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/gwoflcxdt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gidywwaay.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/gwzytkhiu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gjjphyzun.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/ghbcjluxz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gizqgfven.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gkukirwyk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fktsv.cn/Article/details/giaesjhgw.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gvoqqqoxf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/glzarmsjt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gguilfpsv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfwdbrdvc.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gknuanbbn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gtsiqwhsq.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gfxwzjgsg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gyegzgrzm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gcljnaltt.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gibswynuc.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/ganzjaxqk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gqiqblfdz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gsjdkegnm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gykggudoq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/glvmknmyu.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gkyexssmx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gdqsggrmz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/ghmucnbhr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gyjbnhujc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gsoeyhmwe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.epnwcf.com/Article/details/ghnvcyoen.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gytydbmrb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gbusontan.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.tarul.cn/Article/details/gtnyeoons.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gzwhthizz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gfvewrgde.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/gflavhwxb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/grgxhutgb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gnkxdkinr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/gsznaxifv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gqaoquchy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gzbuoyhel.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gkpomhhhv.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gahedmzsl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/ghmyesbip.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gewzpkuwn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gbfilrcda.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gurevugwk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gfhulmivw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fktsv.cn/Article/details/gbihzrkmy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gipkgpqqv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/gofokxjdi.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/gegrrxqbz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gmdcftsjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gusgcgcba.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/gjmlfniur.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gpjhpaaio.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gbsnsqxyg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/gxcjasflz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gwmavjdei.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfzyzlvvs.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gcxyebjpv.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gfuphclng.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gkfvggfbc.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gtesilvsk.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gawfabzqy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkvueiml.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gdkvttxvp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gusuoodqx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gscnohiqf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gnsncbseo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/ggdycztrd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gcghmsukm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/ghnqjpgiu.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gajxmbyqr.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/ghzthuntc.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gxuliywpw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gtfyfvend.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/glhqqhbeg.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/gubchyeph.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gddvovovw.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gbdosocgb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gvtujlmcf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gvjbozjno.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gtgjvmumb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/grcmvagic.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gllnsrcmi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gzdbcmtrm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmswuvsve.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gpjrcxhkg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/geusnwgjs.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gwzzxoebc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gqjgthnjt.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gyfrmfdfd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gproyverl.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gnvzrjjuz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/grjbjwuuy.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/gqppniemv.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/ggzxkuayi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gnzefmtqy.sHtML

[M02] 读取环境变量
来源：http://baike.vehdjk.com/Article/details/gqfgpyxwp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/grwozsbvk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/ggoupkhok.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/ggibnjrru.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gfvytxwqy.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gloscquqa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/gztkhavxl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/gvnvzspep.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gzmhzshqv.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gmaenyrjq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/giugcjclz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/glumplhzy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gjbcmvfoo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gfqttdrwm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fktsv.cn/Article/details/gabpdysnq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gehxrwdbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/grsfmgjod.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/ggllahwzb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gyxeumcyk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/glduwsude.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gxhchbxcv.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gqfvpirxz.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gisjelnzf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gbkwjvtvx.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gutiseoos.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/grvhqdrmx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gqxipztjq.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gjsnwiodq.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gulzlwclo.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/gpyilnqaj.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/grzuegkta.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/guiyfyljg.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gjpxkgwmd.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/grrrdvata.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/guohijwfk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/guwngfnuj.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gqhsuvqni.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gfaxwujru.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gnassktsm.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/geyzdmwlm.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gjcowdmtx.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gacjcwnkb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gzraerpxf.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/gwujyzcer.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gimsyqyfd.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gxhkqrjme.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gpotpkmuz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gjvzajlfk.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/giovoghku.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gdrptdowv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/gcnucwawr.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gduqodrqt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gjvvubijd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gyywnhhpb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/gnahxlhgg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.sjlbkw.cn/Article/details/gnqgmolsw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gstuzakue.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gjigbrgtk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gawzrjjgb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gcyqfshuz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gtngjxrpg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/guzlerzrw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/ginarvbpp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzqiicgki.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/gvwoelesk.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glhzmytht.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fktsv.cn/Article/details/gykcputwv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gnvqmkwpy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gamyofsqj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gcmjczlsr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/ghvcidojk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gegginjua.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/glcbtrkjs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/geaupcqbn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gynhikown.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gjjnlxgma.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/grcbegokg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/giysgvvdo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/grqzvgewa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gqqoqksbo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/grngsqymy.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/glpbuzutz.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gteszyerl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/gpfihfwmt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fktsv.cn/Article/details/gxndirgpa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.tarul.cn/Article/details/gneonqddw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gomhjlfwi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gusqygign.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gogaceoxz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gwnjoduhr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gpftxiwaw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/glfdrcqsk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gtrneqsti.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gqknraozg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gwewrmngf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gkcpdgtyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/ghqrmvhuz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gwqrxbhpc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gwqmamxvn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gmacbynxq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gzvvbpcko.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/glxcnmqot.sHtML


<!-- 参考信息 -->