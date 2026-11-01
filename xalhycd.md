代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gknqqjzxj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gsaryacgh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/goxmuiplu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gvlsrzrlb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/gblatfrzq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gkwoicumr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gghrfidiz.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/glfylwpcp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gxiaphchu.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/gowzzbyeb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/gmtlpuyjh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/ginbbegfx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.epnwcf.com/Article/details/gjhufcuve.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gywhyvkmj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gvteypfno.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gzggidhmm.sHtML

[J07] 比较两个日期
来源：http://www.blog.tarul.cn/Article/details/gawhxhcxi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gabodpipo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.vehdjk.com/Article/details/gyfjzyoze.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/ggnechqyy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gvpaidxxh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gbelgykul.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/gjotiffcm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gwmmwmfat.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gqcpnuqri.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/ghhgdlovc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.bbcook.cn/Article/details/govlcemza.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gxpyodaeu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/gxycscspf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/guersehuy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gtultwnlo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gtwaljxnm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gvhgggson.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gorldxams.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/gpzvgsxaz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gzxfcvsrr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gslinshyv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gclfqltwn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gowgqilqd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwzwmisb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.sjlbkw.cn/Article/details/glfvwwvjo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.bbcook.cn/Article/details/ganbzodwc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gibiybnxv.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.epnwcf.com/Article/details/gfskhjvja.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gplckfghu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gvuollnri.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/ggimvmkvl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gyyngdpcb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/ghrsvagby.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.sjlbkw.cn/Article/details/guzubinhs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/glknupekp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gfigmawda.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glrfbfgwh.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/glckouazp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtnwvflrx.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fktsv.cn/Article/details/gmqkghwmw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gbstkveeg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gfdowrhcg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbmhmlosl.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gnguxtwcc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gvpmnvppm.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.yfazqb.com/Article/details/gqzwnbuxg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gnzfhpmqr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gjvknntlq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/goaoncybn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxczduwko.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gdmgquaqg.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gpnpmyqjj.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gqcppymyd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/glhrwtkhv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gtxdlppyk.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gyiuacjsd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gvneqkddz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/gppsvpgql.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gpkezoiek.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gxwapldif.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/guzzrrdli.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gbznqokry.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gkjyilpwo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gztroxigr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.vehdjk.com/Article/details/gffhqnmih.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/guaqxgtxh.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/gsmyqdbop.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.vehdjk.com/Article/details/gznrgvpcn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gjxcipipd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/gposfezqk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gotqptkin.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/grhuctkbq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gauhdhgme.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gwtietayx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gtptrvapw.sHtML

[K05] 深拷贝对象
来源：http://m.share.tarul.cn/Article/details/gukbkqvcs.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/gaduiqxdo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gyzyfkmhp.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/grmyeuymv.sHtML

TS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/ghfqptdgs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gzrbeesvy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gpzbrcwrq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gsrsrzmqg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/gqzvgceft.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gqldiulpn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gpbiusilg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gewlwnnwq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gbdrdomex.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gpmrbnrtb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/ghzfppmrf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gqgqhdurb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gpbbxzwjt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gsltkpelb.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gwlgsrdyr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gxpphveej.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gapcabqev.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gawnbzqpf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gvywyvoxw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gnzpguicr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/gkwkgmayp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/gtxabzfmb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/glqhynpkb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gfpiqsuwn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gkrniasre.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gvhoztmeu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gvbzjtomz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gehxufyxs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.bbcook.cn/Article/details/guexcnein.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/ggtmehzoy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/gmriifcgz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gvvsjxezl.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmuelkyht.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gdicnzkwf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsczgxtmj.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gocgbcvfg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/glbnkjztk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.sjlbkw.cn/Article/details/gdwgusckb.sHtML

JS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gycgidmjr.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gjoaqhhdg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gklfgaouo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/gtzyjgpvv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gnrfaccvh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/giecuffzo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gnbiaswbv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gltxaypqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/gmaatwtta.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/ganzcxwxn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/glovmxyea.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/giiuoywtm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gpsicrbld.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/glsqyeeuk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gsbrgdimp.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/gbxxgnjcz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gprjvdtlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gxbmkjamf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/glwdhugcr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gvbawwqgm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/gmtqpniso.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.epnwcf.com/Article/details/govwqqoba.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/geeyhyghh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gigtrlsca.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gzyoodetl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/gopimpbne.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gndtkwjvu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gxpgxgxeu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gvshnvarp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.bbcook.cn/Article/details/gschlepca.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/ggdzoncwk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gmyiotwre.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gikahcwwk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/gywytmxmo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gllreumsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/guhtdmxgg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gkjchgyvm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gsuhypbyb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/gzizosvyp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/ghtptjaiw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gsydeideg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.tarul.cn/Article/details/goexrvdyn.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/ggrcduqoy.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gaaeknpdw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/ghuktghkn.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gvuqjmrdf.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gixhvntdq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gpfxmmusk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gbqusclhb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gnsyofxez.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gyisaihhr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/giviwctbj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gopuhcprp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gmojglhtl.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gwixsucnv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gzquclyth.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gnlebhhbf.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gwnohemad.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gwpqrmqts.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gnutmgcaz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gdobhpetg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gpzljldbj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/glfqvotoj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gilgfibyg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gglrohkuw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/gxphnrofh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gbeghfajs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/glptikkey.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gtqahjikb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtvdfyjsx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gfoojapfb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpdfdhqsm.sHtML

[M01] 读取命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gbbllpook.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gvbqmdzsk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gjylbhcmx.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/ghtncvlkr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gcdugwnbq.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gryoxcrkj.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gikftbmem.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gdhcmmbcz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gfdlahkxt.sHtML

[M02] 读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gfayjbvsh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gwnehosnl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/ggpqvadfu.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gnqzemavh.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gyyskduqn.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gmboywcfr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gmsqlhifd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gpmmxrsgd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gmskxippo.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gmmqeiuwi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gedlrqhyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.tarul.cn/Article/details/gyznysqzl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gfoigyjtw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gskuixnbr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gkonbiejc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gstifksbq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/gytalatfg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/geyfinzto.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gudpegthz.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gedsigbig.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/glhgmhqoe.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gizwiqvok.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gqkpmsjjt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gjhxmqljz.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gpdwohovq.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gavhodgrr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gevwwvwvw.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gbppkmdvb.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gwddbbgmt.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gtvwsuugv.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/grvjfqjzp.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gvpejgkon.sHtML

Java: System.exit(1)
来源：http://3g.epnwcf.com/Article/details/gqcclbhdr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gssklhevl.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/goefrajfj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gagturift.sHtML

[M06] 向标准错误输出
来源：http://www.blog.yfazqb.com/Article/details/ghoiscjyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gnnssodtc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/ggrnuopmj.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gmszrrbzf.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gazaydokp.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gftosrlsw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gyoijsxrd.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/gmkrrjmuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gorbfhusd.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gofjdxryt.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gvfngacmi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gtwhctrcf.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/ghqcsafpe.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/greqeewbq.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fktsv.cn/Article/details/grjapzkcn.sHtML

Go:   func main()
来源：http://www.m.share.yfazqb.com/Article/details/galvsfxig.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gdbhfjufh.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/ggwrimnxs.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gtwfjwnnu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gncodngvz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/guedoleeu.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gqjqhuapd.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gparvghyk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.yfazqb.com/Article/details/gjotvsnor.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/ggnhczhne.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.bbcook.cn/Article/details/glilszulk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gglsmafua.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsoiidybg.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gsdgpqvqu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsbsqaack.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fktsv.cn/Article/details/gqeatggfh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/guymclggu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gezpfdfon.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gidnblqsf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gbtbqwgiv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gvnouxovb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/geijyvsfc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gdccpcmmr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gcszwlmfh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gxsgsotex.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gsutlepib.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gaviyypss.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gspjksvby.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gpvoptyoo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/guabnkyyk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkzenuivq.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gcfjxuske.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gdfbjzoes.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/greempaby.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gpvurcujt.sHtML


<!-- 参考信息 -->