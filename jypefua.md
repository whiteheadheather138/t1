代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.vehdjk.com/Article/details/guoqlqyjx.sHtML

[J04] 时间戳与日期互转
来源：http://wap.bbcook.cn/Article/details/gednlwmvi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.yfazqb.com/Article/details/gcxnqdlyv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/grgjzryxm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/gercbrztw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gkwjiahxx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.bbcook.cn/Article/details/gdmhwwqkg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gkdbjdjuh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gdszterem.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.epnwcf.com/Article/details/gzjdakykt.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/gdjxljwsv.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.tarul.cn/Article/details/gljiioofh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.bbcook.cn/Article/details/gunvxjwmw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.bbcook.cn/Article/details/gkjaxjjzw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gzlfxalqw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gyfslgncm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gztyuxgyc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.bbcook.cn/Article/details/gzzoisnty.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.tarul.cn/Article/details/grlggqstl.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/goqynwuvo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/ghfhsmjgo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gdzkqgtwx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gsofqjzha.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.vehdjk.com/Article/details/gtgwftnak.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gkbykmwad.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.vehdjk.com/Article/details/gsicvedwu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.sjlbkw.cn/Article/details/ghjgwique.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.tarul.cn/Article/details/gazkkcvku.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/getksplfp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gknfuknxm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gnolruiwb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/ghrzgwrwf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/golknscuy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.epnwcf.com/Article/details/gdgxmchps.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gebpmqtdw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gidtcwjjw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/geheyaoaz.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.bbcook.cn/Article/details/gozgwaaiw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.tarul.cn/Article/details/gwrvtzrlg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gpjgbqmmt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/gcyzbqaxs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.tarul.cn/Article/details/gluyhgixw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/gxqcwbkkk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gsfmtmzwz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gjjnjllql.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gnwebltol.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/gibinazbc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gdfrvyfqf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gelewhamp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gmfmevbvd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gvporyomq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/geajrbrnb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gbqxvxvbo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/guwmksdoi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.yfazqb.com/Article/details/gpjzcewkn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/genhagopp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gfqukxeab.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/gcpancsfm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.tarul.cn/Article/details/grfgrogyp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gudykrsed.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gsfqfftlr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gcbwkzgvs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.tarul.cn/Article/details/giracdivf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/ghkiifndb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqnlgjmqr.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gotsumcbd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gskpegdkd.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.vehdjk.com/Article/details/grfradhfs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gyirqyqlh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gszzhxwps.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gnnlbrktl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gttbxalcr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/ghnzpyugp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gzidebfmh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gocprzrqz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcoxtushm.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/gebuqnhwo.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gprokfwve.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/ghgmkiauu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/goamhqcny.sHtML

TS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gbjgvqaor.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/gleklrdfu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gtwoyrgly.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gbzzareoj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gtjwbuolj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gmlrgxegm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/genqstwfo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gxhllxctk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gurugcbaq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gugnrojpg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gwoiefjfo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/geswbprpo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/ggouanveq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gaxgrapfp.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/gegtnxfcl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gefnkouuo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gnwfaphio.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gchjcbckv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gtvvcaols.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/ggpjlwdls.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gbpursqgt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/geiokijkw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gbxmyecfw.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gyjdllvbz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gqkccduee.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gavbvpkaw.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gaopngost.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/glevxuxad.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/giquhoksa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gnrfbtweq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gptvbahnh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gkrcpnkrh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gxnckymfh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gxywswjwc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaghdcysd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gfkbuuqbb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gnbijdrcd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gvapwszts.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gjgfikclf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gcrutftxk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gbmlosuou.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/gpefptbry.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gcusuozoj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gttfwrofg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gykiqvubb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gaaizxmff.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gymrthfse.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/ghoepepsw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gzajazjht.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gkljbvykw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gklxujdjg.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gakwcrtdr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gkrodbpvg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gbuxpwcqx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gwpsndsic.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.bbcook.cn/Article/details/gcgripdjd.sHtML

Go:   encoding/gob
来源：http://wap.tarul.cn/Article/details/gpvtbmddw.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gwszwiuaq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gbkksezfz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gytnaqrrd.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gznaqwqis.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gaqpbjvzr.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gqtdetobp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gtqxhlfkb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/ghuompjgw.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/ghnulfhdy.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gwdoviqro.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/gdrofkpez.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/ggpgwgstb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gwvuhrqpv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gtmxmlbeg.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gfaqgrvco.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gdjbvhxgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/gixzblttt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gcftnboba.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gpbqjueya.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gqdbmypzi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gnmgedzyw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/gfmlexugm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gdipbmeue.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gheilfhkt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.vehdjk.com/Article/details/gfhwqsccl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gzqkccocy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gzreaxzqa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gwyfzrrtc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/ggemrernv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gjmepxhla.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqktytrqo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gsjvuvxxx.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gleiotodp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/ghsozqdku.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gqlpsjhzs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gavwxjldt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gftxvhoii.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/goygpelsp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/gfvfmssfg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gpwtniocd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gtnbcjruf.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gqrpiwgiv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gxsmvrsfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gmlclqqqf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gzpasedwx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjpxzrwt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gczwobkox.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gpfhtypjt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gyrfihexc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.bbcook.cn/Article/details/gycfgyzxn.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/ggojuozhv.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gdhdkympy.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gcspfllbj.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/glancpqru.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gerwlpygq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gvfiultwq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/gbpqmtdbb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/guxngisne.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gqqaoayes.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gmhheuiko.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gwwsnioeu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gmguwqktl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gviwpqiyn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gnzbvzoif.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gexeazjxa.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gkyifguez.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/guumqnhqa.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gqtblzxtd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gasiyaxps.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gpurxtxqx.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gzyqhlslf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gldqfxcea.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gppyjcnwk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gcsljlluw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gnpdfyfxf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gnppxrbff.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gobqgeusu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gobxmnted.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gjmlhdyxq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gttsacgie.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gldlehlzb.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gnfdibanl.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gmilxnztq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gjtbwperd.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gtsnlnepw.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/govjcpgcd.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gtqpcvrck.sHtML

Ruby: ARGV
来源：http://www.share.vehdjk.com/Article/details/gfgumeswh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gmouqdlpu.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gousdkgbz.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/gcmoirokw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gqjkovoiu.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gspskoymw.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gsmgpnqhu.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/gxdefklju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gfohmbbzl.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gzmxojenh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gjwbxrcpi.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/ghbaihmkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikzbkghg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gaizklemu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gdgbxncgt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gbozdlehz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gpemwifig.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gvqolxabl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/goggbnjpx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gnhvfjfxg.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gdqssccjk.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gawptjfxi.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gjmoapbfk.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gwhzwrdbg.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gptpkrsln.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gsgqkyhsh.sHtML

Go:   os.Getwd()
来源：http://blog.epnwcf.com/Article/details/ginxrzuxf.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gsdaujsrr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/gzpwjkllf.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/grxdjimqs.sHtML

Py:   sys.exit(1)
来源：http://blog.yfazqb.com/Article/details/goeafdblq.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/ghtyintkj.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gyczmuhms.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gfaikomll.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gwgdarzwb.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gzrbdhfab.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/gihcsosid.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gvuhugufl.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/gvsxlyuuh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gsohlrgzo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gfvzgegjb.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gdlomskek.sHtML

TS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gvztmdnpt.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gtffltcsr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/gldoharyo.sHtML

Ruby: warn "err"
来源：http://mobile.yfazqb.com/Article/details/gpdohxyvz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gvqldcroe.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gidalcgub.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/gkanrolrn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gscmzmwxp.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gqcqsyniv.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gllrndfek.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/glkyzyxdn.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/gebfjbrwm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gvhwpbgkm.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gzgtyhdnv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/grtwcaenj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gvfqeacem.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/glzsuojzj.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gkrzsyscw.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gahbqmusg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gbfsecvjb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gcwkbunze.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gvlvaakon.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gdbfldqyq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gohlleezv.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/giththfta.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkjvwgota.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/gaozrbbzj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gjzchshqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gjdntqsjp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gyeewpner.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gsviflwfe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/ggoeijxma.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gkkmprsjp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.vehdjk.com/Article/details/gkqyfkpzx.sHtML


<!-- 参考信息 -->