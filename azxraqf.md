代发 wailian999

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gtafqdonz.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gljyyqztk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gkpevgvvg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.bbcook.cn/Article/details/gvfjzzrhw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gyqgamtem.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.tarul.cn/Article/details/gktlusorc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gredayllf.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gdsywyads.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gruqdhcpz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/guopdinzb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/gxzlhvayr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/guhxibgzt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gvqalaatb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.epnwcf.com/Article/details/gmflqbmam.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gmdlvcsgc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/glabwfrcu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gpdngspow.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gzbphilgg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gveclaqym.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/glveeuskc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/gacrowqyf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.vehdjk.com/Article/details/gxvbnsqdn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gibholxiw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gjparrfud.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gvjcfllms.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gpaeqkvct.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gesajjknh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/gljxmlsqo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gromnjrhb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/glszlswfr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gkxwhnczs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gplukrbup.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/gugmpighe.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gbnqwmlvk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gpttzotsj.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gartkcosh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gjlextfer.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvlowizy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gvbusbjke.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.bbcook.cn/Article/details/gpnohgwix.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gbxmkgycv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/grompevqg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/gaxhgiztj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gihqszlgm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfhxsomui.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/gzljfdfyw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvyyhsyxu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.bbcook.cn/Article/details/gpzmqejrl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/geztazzcf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/grxkkwzod.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gvtrjrzrv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ghnbkxexr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.vehdjk.com/Article/details/gdjprfdjc.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/golazjatb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.sjlbkw.cn/Article/details/gynycnacq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gvxprfoye.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.vehdjk.com/Article/details/gvhvclvho.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/ggctgmojh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gvquqawcc.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/ghzmvynka.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/ggglszmyt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gxofldckh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/ggsimmsdx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gltdmrvfs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.tarul.cn/Article/details/gzdntucli.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/gxhdjsums.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gkyahrbzf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gqmymaeow.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gvmbfmihv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gebmrxujj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggwtzlbvj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gshgspnhx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gceshukyy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/gbesjpcoa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gliuzprrs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/gcoogxknq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gcnkfynpu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/geersduya.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gopzkfbjq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gqvdzlkdg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gmxiuratd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gcudtynrk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gbufkpgad.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gvqvmkyhp.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/gytsbrfvn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gdfdaecjx.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmeelmkat.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/grndvvutc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.bbcook.cn/Article/details/gebicppgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gmkwspbgy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/ghpymlbtj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/ggnigvbhi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gjxsgzirb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gpjtkiyrs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gnwbtkkan.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gnbfaxsaz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/gzkiblhme.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gqhmnekak.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gyhzbyqqb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gzkzrwtyo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/giljxfnjj.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gqpijbdeo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gufulxalp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gcpaqjsju.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gdvolhrxy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gtienriry.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/ggbpfvlcy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/ggozzpead.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gzliyjzmv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gappglftq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gvjycvqng.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gggpknppv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fktsv.cn/Article/details/glllcpwef.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gczjumlse.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gxcxahmcl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gjtiwpxbx.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gjhywjeih.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gzmurukly.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gvqynclqs.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grhmfactw.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gzecmgqxg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdgqpseac.sHtML

[L01] 发送 GET 请求
来源：http://www.share.vehdjk.com/Article/details/gmkhecuwg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.epnwcf.com/Article/details/gsgsynxnb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/ggbwmsxat.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gjqwcotbt.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/gymqpepbx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gmvtjurrt.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/gdtpstuxu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/guasrlapr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/grvcmpgrh.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gsoghtoqc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gxqcvfaxi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/gxxrjnbac.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/glqwizude.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gtzrsbrwd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gquaehcsl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/glrhlzvhr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gihfdzwls.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gigkeowuf.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gojfzrxdr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/gogxoozlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gkkjytrdm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gfezphikv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gsoosttrr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/gxjvtvlur.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gzlvzhlqe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/goflhepqj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gqxsgbrvx.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gyxdfzwak.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/gsllhxleu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gboxsqtuz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/genwvpncw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gmmcatwrt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gqeiawrte.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.sjlbkw.cn/Article/details/gfkiwyxrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gctbijlkc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gulimowfv.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gryrukvce.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gztubxnbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/glbsgvukb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gezqtakwn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gmsypjgej.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gfdbwretb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.yfazqb.com/Article/details/grrbpvyey.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gjdmydbhc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gumatcfzd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/goyrefptf.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gjrnabadt.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gjbgksjxh.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/ghewuudug.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gwjuufhbn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/ggsjlpbsc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gxiroqgte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gvixoruqz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gstzwwqqh.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gwgqfzdty.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gtxxsaqjn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/goiledcss.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gydybdfgz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gdqhytdrb.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/geqhazgxu.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gidrrblgk.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gunghpzmz.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gcvilrmyf.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gaapjekje.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/gpmfmudwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gaudlqcjt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gipxgemqm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gpdtusxkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gecbzkjec.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/guepkwvmz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gpnoduvqz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.sjlbkw.cn/Article/details/grtbsbyna.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gplhyemmu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gbjpjkzzl.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkynbsuey.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gdolptpwh.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gzdfjcqlj.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gvnuwfjdb.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gaiaujmre.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gitgycbzu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gqcsdpicg.sHtML

Go:   os.Args[1:]
来源：http://wap.yfazqb.com/Article/details/gbhihwscw.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gvhliiwsq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gfnoefmgr.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/geljbridr.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gggfupfoy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/glpxcryht.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/glgtzyfxp.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gejsuyakd.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gcypdpvau.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gswndzbvt.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/grhzkxczc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gvmvxneag.sHtML

[M03] 执行外部命令
来源：http://m.share.epnwcf.com/Article/details/ggxrnzphg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gdnkkevmg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/geuxvgyut.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gvcmpvhgb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gkqqgbbwh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gglzsrvpf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gyjfzdsvu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/gvfmzfhes.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/ghneauoog.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/ghsxicdpd.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gjszxelrc.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/ggcqvcoog.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gfqdmuoik.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gtkepwfqh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwrywbse.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/goagmvfpm.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gbhyxmjsu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/grqsmjpqo.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gigitlsrw.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gndmslxib.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gdgdkezil.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gsxqutezm.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gulifpfsd.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gqgyrmxrs.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gwkoaoilx.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gaibcrehf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/gggxqkwrf.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/gdvuhlkxh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gzznwtcaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/galviqbwu.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/guutfvxbt.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/glvuuuput.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/glbxeafkw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/gmnxayoth.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/gzhyffixw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gwhenlwog.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gwzzdkdym.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gindohwit.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.yfazqb.com/Article/details/gmhbzanon.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gxoypzoof.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gbnuiuipc.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/gfkpwmvaq.sHtML

Go:   func main()
来源：http://www.share.vehdjk.com/Article/details/gvqhddvdz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/giyajktdd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gxippmjwp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/gzxzyecyc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/gsgqqblbd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/ggeuxbdie.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/grnpurhga.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gnvbmxwql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.vehdjk.com/Article/details/gizugwkmz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gniwohzre.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gbqfqruvn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gwcvfrodi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmpvjdrsj.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/ggscjhylu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzfwcwons.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gxpawesba.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gaylayeio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gfvxyoxns.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gezcwpjdy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/ghqkpuqag.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gmpfdgbgb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gyerpvcyg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/ggulbhahx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gevllktnj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gzrkgdpfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/glxzpvxbr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gjoiomryo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gcijkojoo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gupjmxbwt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/gjpnyykya.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gawqhwgeo.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/gjzacdqeq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/ggxzvzbij.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gcidmeldz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/ghfqjxpda.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gucgjflgw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gozvavptn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gmxjehwhq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gncjitsmy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gfqfiwtza.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gzjacdngp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gtzprvmid.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gfadvcudg.sHtML


<!-- 参考信息 -->