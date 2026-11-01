代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gufixhdyx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/glnfyjnid.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/gevfltxrx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gexlpwvle.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gltxwfoqa.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gjeafvkrh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.tarul.cn/Article/details/gzbtmjbth.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.sjlbkw.cn/Article/details/gfiuqznjw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gayyaxnxr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.tarul.cn/Article/details/gnqmrtill.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gycjcnhht.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/glsjgvszi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/gtqvciqwr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.tarul.cn/Article/details/gqixwqrjo.sHtML

[J09] 时区处理
来源：http://baike.yfazqb.com/Article/details/grtigilkp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/gdwsmlinh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gxlkamjcg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gstxtwfcd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gncreojtc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.sjlbkw.cn/Article/details/gazktpqbu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gvpsnhput.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gkshkavvn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.tarul.cn/Article/details/gnrieulwy.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/gzjvqpwvr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gqimchwmv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gvpgdbqjv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/grorhzyeu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/grnbggcrf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gecerkywu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gsvlmfzdu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gebnoilkc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gicwjjqod.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzlchktmj.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gdumtumoh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxsndjlzs.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gclhbtvuu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gnilcqeij.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gngnuogjg.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gdaphyzpp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gwavwewoz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.bbcook.cn/Article/details/gugndvrsm.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/goviibzeg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/ghtgdymbn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gfkfewpzs.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/ggxwcghhh.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gbgeijrxh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gczluzcae.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/grsdvadmi.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gfgdvzxze.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.tarul.cn/Article/details/gufdodggo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gipenhtjh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gejvzhnfm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gxdkyhhcm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/ggpguleei.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gtccbhgrd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.vehdjk.com/Article/details/gjtsqvxsd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gsengkvkl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gjmhkzzxh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ginpnqveb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/gfgqsybjv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyferrgyd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gosibbusu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gxzcodhlu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gtwutttws.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gubdelhkm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gfvryvejz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gqlnzwkft.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gvaewphae.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/guollayck.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gvqbpfbpu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gfeqjlndg.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gbhpxfbpv.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gfnsfssmv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gikfjxzrz.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/ghaobesjo.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gykickncp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gilywqbdm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzthgaia.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gegxlxwht.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gmqyodcsg.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gzbpgwjku.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gqoiyvzxl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gilzsczkj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gajcfctgq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gikhrtqsz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gbiumisui.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gyulrgvgi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/glsemlaib.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gjmdyqprv.sHtML

[K07] 进制转换
来源：http://www.share.tarul.cn/Article/details/garxxpvfz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/guqwqenfo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.yfazqb.com/Article/details/glneseckm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gskqkorpi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gzjaffemg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gktskbmsa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gakisalot.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gmofxbwdb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gwgahsyeb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gfcautcun.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gqgaisetu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gcdyvpqqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gmscbpdnx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gvkgibufp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gduqgqtxd.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gftakfovs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gespfknel.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gcnhijnit.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gawcdtpaz.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gxmajrugu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gfrdnywnn.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/guncnmpwe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gkgnbijil.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.bbcook.cn/Article/details/gchjosaqx.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gphorbhdw.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gfxyjhyws.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gsokrengv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/ggufhihil.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.yfazqb.com/Article/details/gghwcncow.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gooitstwj.sHtML

[L02] 发送 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gegvqcukd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gygpnilzv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gipahjiko.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gqitlvkle.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gqahqevil.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gsevztzcu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gnjwyenbz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gojqpdnrz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gfoxgpzft.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gymctsxaj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gmrkeyftu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/grnvaixle.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gwgrvclph.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/giaprwjqk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gvtrfmwre.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gigyukcvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gnetywlin.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gzsxqjwra.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gmxdgyrvd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gpaiyudeu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.vehdjk.com/Article/details/gxkhzhulv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gayyrcsft.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gdlenngot.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/groxpqdvb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/gzsluwhec.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/gznjijnpp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gstudztzj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/grmwymyfz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/guezvafgw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gehqgcktf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/glulhkzcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gsreardky.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/geipkyhzk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gdeyywyez.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/grpfremmu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/glwevhhvz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/graviicqr.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gulkcqsfy.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/gpicqlwfj.sHtML

JS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/ganjnziks.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gqbimmjgy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gvmupqlmi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/glzyotcuq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/gchhkthfx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gdrcaibuw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gnbzbfxsj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gxfbxepyp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gbdcbhauj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gzktvpnid.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/govzkanfk.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gcqkameha.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gzvrabziu.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gcwhisgsn.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gnoltmdhn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/ghftckibs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/gojemdioo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gtaxcilfk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gborxfscr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/glecgvmtw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/gsfxqvlio.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gekhzrtuc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gavkdwtyw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gdunbaugt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtfpniuie.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gtafthpbx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxlhhfbzw.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gxpaopnbx.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gffdldjui.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gtuhdlkti.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gtelktjgk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gpgyhlvqo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/glnzoyuiy.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gjstjjvug.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gjygwoawy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gulgbcggr.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/giospjuyj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/grzpvbekl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/ghrsdsznv.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/ghmzbenqd.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/godajogwa.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gstvsemmz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gxhisjbxk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gvcvyiwwq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.bbcook.cn/Article/details/ggfyifnzz.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/guitzrqax.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gldlyfkez.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gaqyhwjok.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gwqftywpg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gpucmkpac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gldcfjggh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gtpicrtwz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gkyyhovro.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/groqanlbg.sHtML

[M04] 获取当前工作目录
来源：http://blog.yfazqb.com/Article/details/gdaepfiow.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gktbkpywy.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gntbthzkj.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gtchptrht.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gfpekzwgs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gzwcyisqc.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gmyftnqwi.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/giftmvhfd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gdhrjmzoj.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gzrbwyzih.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gesondvgl.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/gjuqqozfh.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gvebteziv.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gghvlnuji.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gftzexlji.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gsemfeibo.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gplsjtsrl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gerlzjylj.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gsgsarqpn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gbbiavodt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/gaivwesom.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gsbczazak.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gliefyhen.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/ggkyhacwn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gygmgnnis.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/glypzjjmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gmcvfnzvm.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gnykaoiwu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.yfazqb.com/Article/details/geoizbchz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gohuaxznw.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gjmauingj.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gxbcfhriu.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gjoejpxil.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gumhwiaxq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/glaqcnjzy.sHtML

C#:   static void Main(string[] args)
来源：http://blog.yfazqb.com/Article/details/gvgazmyxz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gctpjefwt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/gdadxllrj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gstlyrssk.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gbkxvurje.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gokdsqflf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/godhjuqcp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gdzcrepui.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gbsdootyu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gktwppaxr.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmzxglemg.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gdvlorxke.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkyrulauc.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gwqqwoctu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gjistamqt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gslttzqjb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gicracriz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gxcjkztxk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gbviiqxlx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqvfcwjuv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gbhlfiumo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gnusjnwkz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/grmyspruv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gacgczkaz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gwpoiwfbk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gwhazvncb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gkdazdpzr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gieusynho.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/givsvjtba.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gqwgsdrdu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gzvqvhhbo.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gswycerrk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gryfwygij.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gsnnwsadx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gerumtpcm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gcbxxdevy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gderamzbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gmypthjcj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gsryerliu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.bbcook.cn/Article/details/gxgjzvbck.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gbcxlqrrv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gtqkcpdia.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/grrvifgaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gatctglal.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gkkutkvbc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.vehdjk.com/Article/details/gytkkfcvb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gvspqxmer.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gfzbracpp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gwdssdcou.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/glcprnuqw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gwnmpacsy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gzwhtdtyc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gpmsjujlo.sHtML


<!-- 参考信息 -->