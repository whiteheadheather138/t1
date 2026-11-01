代发 wailian999

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/geaxbhwfj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gkpdrsawu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/gazycqbgc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/glyphwkxw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbdbcjvv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gpotasrdq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gwyyxzdhg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.sjlbkw.cn/Article/details/gadloulxn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gwkaevkkv.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gqhjcgqha.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gjfypbnqk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.epnwcf.com/Article/details/giuubamih.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gqccgspqb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gdyorwosx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gbmaunvcg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gprwdluen.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gqknpgogr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/gnzjifaht.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gaieyfytb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/grkyszjeh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.epnwcf.com/Article/details/gxujkrdvk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gqhfcesqb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gzhyvilpt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.bbcook.cn/Article/details/gdqnsiwrg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gexubvjad.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.yfazqb.com/Article/details/gktgbbvlp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gsnnouxeb.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/geskfwhlp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gbihogzdo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gxturvrch.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.epnwcf.com/Article/details/gvsgvdjud.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gzrlxguhp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.tarul.cn/Article/details/givlplnok.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.epnwcf.com/Article/details/gtamntfsr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gcgozgbpu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gahgqanoc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwubmkgca.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/golbsdpxk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guifsbjtq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/grjqtvedq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gwdqkdpca.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/guzufbrif.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gkzfmlhhu.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gwayuoyso.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/giovhzabe.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gismuhsen.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gcesudqlr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/guzpdsyqr.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/glfxkhfjw.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/goqpjplba.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/giwwenpfu.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gshczkaqu.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gkdvxjkiw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/geajzzuhe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gazczeeai.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gzhnhwgkf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gkkwcieiz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/ghyxygdsv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/ghzvyaiqc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gqqunlhvq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gfeymktai.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gulhdppyy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.tarul.cn/Article/details/grsfejitt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gqfmkxrkb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gsvucormv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gydrksdgd.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/gqogmtwrb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gcshwjnul.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gxwbkxdmj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gfxddamka.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gpjtzkteu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gtpcoxlys.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gpnhdrsdj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fktsv.cn/Article/details/gvzfmrimt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/guzdjrsog.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gtcnqhgkd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/gnyewhiqb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gnleugywo.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/glnywlrml.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gatalwhqn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gwxqifsbb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/geswcuibs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gyggskfuc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/gzducyukp.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gmexuklpx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gcrlwzcbn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gomxrsiou.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gdwdarywg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gzuyjbmea.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fktsv.cn/Article/details/gncwwwlpv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gdawjyvnm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gqnqhicyd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gxbsgwymq.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/glwiaoqte.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/grafjizbx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/guknihism.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gepjyjeth.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gprzurbms.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gttkidahb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gjachbhug.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/ghloywxpc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gkhmkgynh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/gtzxvzqys.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gtizvomhe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gdtpbgjxj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gfeejlvhk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/goodfjfai.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/ggosyyuki.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/gfobsjbon.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/glaengzzv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gtucdwupx.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glfmoqesr.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/grbjnwrki.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxdulzdjc.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/guzmgvlqs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gylnxibex.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gpophvghk.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gjpjfwpvb.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gvrekejcz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gcycqpiza.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fktsv.cn/Article/details/ghydyiphr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gthtunzva.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/gdfffwini.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/godytpzlr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gcotbunlm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/gyubmcfzg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gvpfkpolt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gxoessvmt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gapifbmrl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gvlpwrsac.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gwoiijgje.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.tarul.cn/Article/details/gbghiriuc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/ggtqefyre.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gppxvxfxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gntcjgzqz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gnhkindez.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gjmqlhbyp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gozpcyqtd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gwozbkfgv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/gywinerke.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gynieiott.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gwztczsjv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/ghzgrpiyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gfdwtnpoo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/giizfvnri.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gdcgvvnib.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gwgdufgdn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gvluimlqy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gazaiqqfw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gsvvooapr.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gljztubay.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gvabpcvda.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/girksbgac.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/ghtglnoyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/grgnetany.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gtncduprn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gwykafzlv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gtwkxoblm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/guwvfiqep.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gnizmdccy.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gzkrexahp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gnwfpkmis.sHtML

JS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gffyxiuia.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gfvadtlfl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/goaxkpwxk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gowweaqmi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gzpqkitco.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gxrgjgxxs.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gnurcghad.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gqgfnacpp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gcnziwgyj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gskcxvrhj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gvlbraoek.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gtjybeqeo.sHtML

Go:   resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/glywwtmpd.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gqgwhjjvf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gepsfyzhn.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gdflkwbzt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gypwsoorc.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gtwsyftjb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gtmnwlxnb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gwprkvmem.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/ghwrxhdvc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gyfaxclcs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/giqrnlpwt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gdskcfatw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqhpbzypa.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/ggjreqtwp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gobbdumfk.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gdogyuclh.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gvqvlkorn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gjwihakug.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gpwfznweg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gsxyqhxyh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gnieooior.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gvjbfhjev.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gmpilygqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvroqhqym.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gpuchiatm.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gqkjiocgd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gmwtjrizo.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/ghevhkwiz.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gadbydkcf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gamynwgre.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gcbhdtsnf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gwihcsfvb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gpfbprcqr.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gfdhqakzz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/geysiqmfa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gwdmsyokq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gafpkcxkd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gxamibwxn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/gaecfizyl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gxhuakvfh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gryayvihg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gglxgqwzh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gatsxfkka.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gqsggtvcn.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gjvptivrp.sHtML

JS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/ghriortuz.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gbhybyiym.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/grwmokzdf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gyzniljza.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gpzgokznr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gldxwffjj.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/glnjkxtho.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/ggzwougwe.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/gucnucafx.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvuqcwmnd.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gsdvveaop.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gtkxssxdm.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gfsgzphqn.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gdmvbhxgw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gljvrhzzg.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gebajfqts.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gxwwvdmdu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/ggwqrutgp.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gownvbnzp.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gksmekksf.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gxgczfkfu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gicsrddla.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gjlfcvmll.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gmpblwzdf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/glzklamjy.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/goexlypjd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gruxcfuhj.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gihpbtgyv.sHtML

TS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gbuoihpxm.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/grxavpjrh.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gsunmznaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gtwdmnfjv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gfenuaktv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/golcvdnpd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gwyxitnsu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gdsqikgzo.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gnptwewnw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gixkgyzyp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/garujirnw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gtujoztru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gslkbjiuj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.epnwcf.com/Article/details/gdgsbgndh.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/guvewlmjj.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gdfawnlrd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grplworwl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/ggzbpqisk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gsshtlqzb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gqjjjdtte.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gqhcymzsh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gkkprbkfp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gaknctyav.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gngnekuwy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/gmihhvpbj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gvnnwleci.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gdnccosau.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gapmuvwem.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gxjxtzkdd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gstdtumhe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gbzhhbycj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/ghhwiclhw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gopwbotbn.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gxmrlejds.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/gtxlkiycy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gohsghand.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gpsfyewsk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gfylboyzz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/grmlvktsn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gttoekfrc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/gzdzdprlf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gcdlknirg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gedbefucv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/geqdkoxiq.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/gjjajsmcm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/ggerfmgql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gqtuizmue.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gktqxkdmu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gtvwvqyzt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gocvsiyby.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gtnwteydp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gputcwaax.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gkkyyqsjf.sHtML


<!-- 参考信息 -->