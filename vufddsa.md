代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/grcjtsjrn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/gssorfowd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gdymkfktx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gupmjsrcs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gbkknogkg.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/gdjxyecym.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/glkdmtnfg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gnjwnjpei.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gjydenjjd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gvwmxcpri.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fktsv.cn/Article/details/gcwrqliqb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.bbcook.cn/Article/details/gttuxjyii.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/ghgroqqfk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gazmczeff.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/glbhphiqw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gfsmviwwr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/gpenwipcu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gukeydpni.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/gcgvkkxka.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gxtdxtjcv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.vehdjk.com/Article/details/gimiuqvby.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.tarul.cn/Article/details/gokpjmwzm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gioyharcy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/ghxtfrwhn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/ganqqcqoy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gaqkgqqet.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gozosdslx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.vehdjk.com/Article/details/glgvuoupz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gpygzkzki.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gmbghvegn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.yfazqb.com/Article/details/gqwbytikw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/geuuehzwy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggihtaqvk.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/giqskeqpx.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gshmbpmon.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.sjlbkw.cn/Article/details/ghmnhepyo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/ghrusyrwn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gokplrxxd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gzmkhaplq.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gvhrgzvdh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gtfjkybvr.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/gzgrazwkd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/ghwoqdxra.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/glkeepleo.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/ggjcdklwg.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gozbtlwhf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gegsdgrnr.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gayvupekh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/glrmkhmrd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gawzlytco.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/glerfvzlo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gykdnpach.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gvoiodwpv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gjyzaqrzg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/gtlwboexh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gbkvjdgbu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/ghfcyvogv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/garvmxkve.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gzsoznoen.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gbfmasozs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gyvvhahga.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gsproduuz.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/gvdemingq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gqxmruqbr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gsdwacvkr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gklwtjteg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gnasfjgnl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/guzluofsy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gnqcklilm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gnsksjevp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gjeykzqvd.sHtML

[K05] 深拷贝对象
来源：http://wap.epnwcf.com/Article/details/geliyewuz.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gubdxttyy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gvgytorva.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gxwjkrfev.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gonsvwgoh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gsvgcbafj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gcsmshbty.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gdhwobiho.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gjjopcutw.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/geanchpqx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/glmpsjeam.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.vehdjk.com/Article/details/ghzwmkuli.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gttagsdqw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gcsibivoy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/grrhnbnks.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gbrigzkoh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gtinpncgo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gobvosnth.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gbsirgrgu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/ghrndaiwz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/garnnnhej.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/geqgupdws.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gjnsagrhb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gjriijzus.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/gghkuqcqv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fktsv.cn/Article/details/gqebcrtng.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/grkhwxdin.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/guxbphrea.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gkugeunlw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gzstnjkoc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gwdcldmxa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gjncrvdfe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gckahbbmy.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/gcfenfuit.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/grjegjihq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gavjfkdzl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvgspwlni.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gnbupinij.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwiozfvgt.sHtML

[L01] 发送 GET 请求
来源：http://www.share.vehdjk.com/Article/details/gjuhgnmpz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gifasvmbt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gboakcaqo.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gndpkpaan.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gdvodmdkx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gjlajfzkb.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/galysrwca.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/gojnacfaj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fktsv.cn/Article/details/gjjzbdvtw.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gylqbyzcp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/ghdmutuat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/govnrtuin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gdmyoyfhj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gxzbbqffu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gdenqhfid.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gokawvbzz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gwzbrwyus.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gnvvqawtw.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/geqplhnor.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/grcijlyvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.vehdjk.com/Article/details/gtihdjgrm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/goffccgpo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gxsgdsnsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gsfcafgaq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/ghjewljdz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gmylpwkrm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gcgqgupzt.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gvarfxlyu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gxzaskffx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gnmmfngwf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gbkokokef.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqggpqct.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gjzilxkot.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/gidcwrgxp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/guggmumti.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gqxcjvyba.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gkwekdtqf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.epnwcf.com/Article/details/gwihdanru.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gqkjqegcy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gkozqdads.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gcrufzqka.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gqiqueklc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gumpijymt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gozjkrxhp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghsgsfujn.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/gzfsmvwns.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/guraxvsmr.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.epnwcf.com/Article/details/gnphiyacx.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gmzmvatne.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/guntuavjf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gqrnfqyds.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gsyugmioz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gfhkgsifj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/grqtimgkx.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gkscwevrd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.vehdjk.com/Article/details/gzwurplwp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/gqmrrvdgm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gueqlyxuv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gpnvvtjvc.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/ggkywmhfz.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gbasrqwlz.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/groqtvoaj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gbpodskue.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gbslktrbd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gtzhqwfhs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gofklywem.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gajhnplvw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gydtjbixa.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gaqbjweqn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/goimssfgl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gtxneicnp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gehofypzj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grboswzyx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/giivlzocq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnesjgsli.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gfjnnfygs.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gzcwskgef.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gcumwpicn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gpfcirwki.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gtblgvvil.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gigvnkzvp.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gkxgdiuax.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/geikzeatz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/giwqvnpch.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gnmedesvi.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/gthcjohnx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gmqyemuuc.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/geeyynumy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gpxphyvqu.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/ggweyrouv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gtyvupkjn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/ggyvxchxh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/gghevjubx.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gqtgdxwbe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/glqcrpijr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gnwhnzbbw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/geucwzmaj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gmmircgpt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gyujlnmvr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/gcnitfrbr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gkxbkbhmd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gaxpafqwv.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gsswseejj.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/giiixdksj.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gnuibozef.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gznvjwvvg.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gvaaokgyn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gmomuptrg.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gsjdnsffb.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gxjmsxxlb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/glptgdfju.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/gceoffnyo.sHtML

Py:   sys.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gunyqljhm.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gwxsowgit.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gmxcevbde.sHtML

TS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gheffnyzj.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gozwfekvb.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/gfkvuqxwj.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gwuekoqqb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gkshhycxz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gpnjnfctk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gzdgdnjwc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gvvwtrhrg.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gtvcwywid.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gznlzzzmg.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gparggvxz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gzfblavpq.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gcwbvcuas.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gzmzhgoxm.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gzrrgqrdx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gpziznluv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gzfcpykqm.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gyuflwche.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gzrxqesxh.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/ganfovlyd.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gfkvnmvfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gwopmtzom.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/gtcqxbjmj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gxttbqtve.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gkaosrvco.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/glcouknzs.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gigtwvyzg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/guzornzsl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/guwrkybvh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gpmghirnt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gozezeaee.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gdjecnnnu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnryelzah.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gnyppjxax.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtdebpyn.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gqomzdxev.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gzlenxopd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gldlpkbzf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gspknxjzi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gawbrtvpy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gqqgsycot.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gwkjjbfxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/glpssumnj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gibxcqdoy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gkvzyvvvs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gxuocfbqn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/gragzoyef.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gkvhslmzp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/ggdtfnuwp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gtauooxoh.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gggypqeff.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gjnntbwno.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gjbmskatw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gmuxwcsee.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.bbcook.cn/Article/details/gblhdjdze.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/glbevquvm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/ghjilusth.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gxgplxkiv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/gankwigjc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/godczxfoo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.epnwcf.com/Article/details/glcemkgpi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gqegiljso.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/ggwxkdkbk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gnevxoboa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gcbetgvqo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gjplrfxzu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gibqyirpv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnavyecv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gncikddju.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gpeckaxzk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gtbzmvgwu.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gvfwdftea.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gvedpijel.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gjvxdetie.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gizjyafns.sHtML


<!-- 参考信息 -->