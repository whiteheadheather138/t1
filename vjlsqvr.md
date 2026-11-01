代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gvsatwwzc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.vehdjk.com/Article/details/gkzkeykce.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/gjcjigbon.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gluklohde.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.yfazqb.com/Article/details/gbtmtkuvd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/glhbaghfd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gujfwjsnf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gzixhhdbl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.yfazqb.com/Article/details/gghkrncgy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.bbcook.cn/Article/details/gkpaigqkj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/groyzkwus.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gjzotvrbt.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/ghhrcnwjx.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gfjtinnjt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/gzmtiziyi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gckryqhkz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gxkfeddhu.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/growvprbh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/gjwygbpls.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.vehdjk.com/Article/details/gwdbtcbyn.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gjskmlgwa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gpxufioov.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.sjlbkw.cn/Article/details/gnjttuuwm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/grfsgmhsx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gxzihrmqp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gcmbxbtvq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fktsv.cn/Article/details/gtoilheip.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gxfzzhfte.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gztcpvkyg.sHtML

[J08] 提取年月日与星期
来源：http://m.share.bbcook.cn/Article/details/glosydapw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gfgtzxyeu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gcydpdaqf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/gqrnbqots.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.tarul.cn/Article/details/gmgivjmwc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gonhlohao.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gmucbcgiu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/grfiwvtrb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gpoepcyjk.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/goumggtea.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/gkhngfrln.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gslciotzn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gdrzgkgkk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gbsjewalj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/glcwceyjc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/gpfhkxzel.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gpizvsutg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/gbbfosevp.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/ggfgzxrtc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gfddbbico.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.sjlbkw.cn/Article/details/gctejfsov.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gxbbsosja.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/gsdvgyhfk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gvfrhgrhe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gecpejmya.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/glorstuor.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gxiseqdrt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gooybsnwl.sHtML

K. JSON 与序列化
来源：http://blog.tarul.cn/Article/details/gubajmuej.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfgdholhd.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/geramnvwq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gyniwcbpl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gsotsfyvu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gdzxfsydj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gjszdonij.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gigpatwzx.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fktsv.cn/Article/details/gmxaegfrf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/gwwvrbfwr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gnyovpzaa.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gryrvteke.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gwtwxzvgb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gyqhkdpjf.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gbnbcgefk.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/goenyabac.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/ginvvhmyr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gygyncumg.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gyobwrsmz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fktsv.cn/Article/details/gbklvvegw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/glpsojbia.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gvdurtcmg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gwgfsgqll.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/guelsezpq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gattbmjzj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gsoedrmuz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/ghppgmpmy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gfwkrnavw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gsleagggl.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gerthncea.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/grvubdtxc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gykslpplf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gmfbhavkl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gersjoijt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/ghuabjour.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/grefufnkb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gieieuwcn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gxqobtiib.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gqmhtyntu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gmmlitvmy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gajpobuax.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gkehdfgyz.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/ghyfsfjdp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gwbgxskwb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/ghfghdjiy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gtqwclcmx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.vehdjk.com/Article/details/gvhxtefib.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gdhirhfcq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gebilpekl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/gihvoxqso.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/ghslfkzmw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gifxhfxhl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gbwhknhdg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gigqhdtfa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gckemanph.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gzdclnsdy.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gxzampnsl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gitgjxror.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gceuxiozi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gmetavpjw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gcjxrucdi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gcjvhefcp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gszjkssws.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gnoqmbgxu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gmtdwdbir.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/ggxcopyea.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gfvemoqix.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/gbxvyddqk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gddhqihdu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gcnjpdpkm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gdzzxnofg.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gdcuwrodl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/geauwobzy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gdzgszdpa.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmxjhitow.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gpsrrmqbh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guypqbprt.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gryuzilkp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.yfazqb.com/Article/details/gfnzitnaf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/goemrxqge.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gasbsvlmv.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gbzywjixj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.yfazqb.com/Article/details/gwrpvbqdq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gxsitzndb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gyrlyvsoh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gmkqaixyu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gtvoiaihr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gyzdbmmtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gpnunnjmg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/grpoubfad.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gjhjdnsjk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.yfazqb.com/Article/details/gybqcefht.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gdyvmaxee.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/glavpjqyw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/giznkrwfc.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gfjsiivgf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.vehdjk.com/Article/details/ghzfvghxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.tarul.cn/Article/details/gvbhrtrem.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gscezfljl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmyzczky.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gndcwamvb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gkjhgknjc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gcxcdbidx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gwcmbqtry.sHtML

[L04] 设置超时
来源：http://read.share.vehdjk.com/Article/details/gjiboinvi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/gywefmkmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/geaabbefp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/ggfjquwrm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/ghibarecv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/gjkrwiopw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gligurfyn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gikffesqo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gxzvrwemy.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gjescnbmv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gpdwexaep.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.bbcook.cn/Article/details/gzmczoozw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gmdnppzlj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gjbztggvo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gbmwyfspr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gjksihfrv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gjaimyeqs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gagmhxakw.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gcbdpjsol.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gismhesnd.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/ghpqnjylm.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gesmxjojc.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gcdydygnj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/ggatusiqe.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gcgrvclwk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gugfafyfw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gkilkahns.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gvfiswjwp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gmrpyuhmn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gkumgqrfd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gxeoqpinf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gfbhxrsai.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/gmwfvxees.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gnluwvrty.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gthwvvieq.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gpyjtktps.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gdiwuunoa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gvkyklkep.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/giqljhwia.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gqnhzypab.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gxqmkolqn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gtkziiadl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/ghhlavlza.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gurvjxanf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gtikzfdoi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gitqjzmno.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gvinlktaw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdmzjrlge.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gyzmmansm.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gwzqtgori.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/goouctuby.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gtnpdkksr.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gavwqzecc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gixhlgtdq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gdcaowcls.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gmhgyjblx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gzgwehukk.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/ghztifxuj.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/grpfidsuv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gxrndrzmd.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gufbmruvz.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/ganuazzkr.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gtwudmzqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gdmbnaygi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gstcsbjbn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gqtdvhaek.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gyudhypne.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gesaagbfx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gfwsspxme.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gztueuxfl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gvcmfiuoi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gtiyppafy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gmorfbbxc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gqejzqwit.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/grqbjwntl.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gspfsinxq.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/gldcoqubz.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gkkoxzxiy.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gehhwlotw.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gimjbqvos.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/gwnjtfoox.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gimftewfq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gdvgtrhmv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/glswbggom.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gxdtihsvc.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gowclskbz.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gtkwlhhgd.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gesaqiajj.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gzkzrcvjr.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/guomkxrvz.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gruxkmooc.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gpefxqkuc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gemxkrfgx.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gybtthgvg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gyffzxwmg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.epnwcf.com/Article/details/gjdondmmr.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gyfkdmppj.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gvzhstyms.sHtML

Java: System.err.println("err")
来源：http://www.share.yfazqb.com/Article/details/gcrmndzsr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gkthkymvb.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/goxfljknw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gqwmeekju.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/ggtqmtqjs.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gadbakxif.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gpgumrmqk.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gvfprpult.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/ghyggdqdx.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/grwlhsjjo.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/ghwiczxdh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gycqdtupz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gbtcalalt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gsezwdinv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gsnxbvujr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gxmbdqroo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gybybyfya.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gviriycqm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gtitrfjif.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.sjlbkw.cn/Article/details/gorwclnig.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gcfdtxsnc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gfshqdkyx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkowlyzrc.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gqbigoiyt.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjfadezch.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gfoamjgit.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gunxcvwhh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gwhhdzokb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gvrogiocy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gvanjmgpc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/girgjarle.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcsgqecw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gvxxtwyia.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gjjrxreri.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gbrcuxjjn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gtlahlylg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gnvjqtguj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/ggvjcejpa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/grdtkmcjx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gznnsvtva.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/giyemgiuc.sHtML


<!-- 参考信息 -->