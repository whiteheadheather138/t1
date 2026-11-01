代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gccqhukvx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.yfazqb.com/Article/details/gapgtoozt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/gvrmjuplu.sHtML

[J06] 计算两时间之差
来源：http://wap.tarul.cn/Article/details/gsaaazjbc.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gwlzhdubh.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.sjlbkw.cn/Article/details/gbgrbthdr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gsfhowhzx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.vehdjk.com/Article/details/gfwblwceq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fktsv.cn/Article/details/gclghaahf.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gojxvlfgk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gtmiggcow.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/gtjhonwoj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/gsridbolp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gaxjdzoam.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gtrbddrpw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gugfrfndt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gluemxdlg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gwqgdhaen.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gfteaoxtq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/ghnxtuajb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/guemynmyc.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/givoluill.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gjgidbari.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gefqjsiei.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnpsuxhw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.sjlbkw.cn/Article/details/gikrsjeca.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gjwzzgqpv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gdxkjeyxm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gqdatgicu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/gizdscbes.sHtML

[J09] 时区处理
来源：http://read.share.tarul.cn/Article/details/gyrhlxzqp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gyyddymni.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/gukgcoetf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdptvfwzj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gphaulkkz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gsobokxyn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gypfealrn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gofjxiyeq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gblbffvwa.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gfkzlwebc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/grjmjmrld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuzaouzh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gtpiaizzn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gqoovknyy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gjatncmip.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gfbpshdmz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxfttisl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gsgwyazht.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gikajswuj.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gqgfeboso.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvwgktpnn.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.yfazqb.com/Article/details/gijsyooxx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gnsalqqyx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gwidfobxn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gxikljaay.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gavbnivqu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/gkmktvsob.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gaioygnci.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gsoovsqch.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/gfixzqfct.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gzppkuyjw.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gajmnsypq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/gjxufnwzu.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gcspardup.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gyyxhwnqn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gvbsovutr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/guzmysifp.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gfvqzyvle.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gqnlfavto.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/ghgmwwpey.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/galizudzj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gluefoxmb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gdvntjyob.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/guvtbcoks.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/gjijtyyaz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/ggyseddpm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gvqktiozr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gmpabalft.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.tarul.cn/Article/details/gifjkvtgs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gcyiqicfg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/gedzbbkmb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/ghgolukgc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gczcdeevn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gvenrlggu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gzgwrnhga.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/ghbzwizpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gtwshzysc.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/ggnvbsuwq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gkzybauup.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gavvkvozu.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gcrpauzqd.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/garrxljmo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gnpncfwin.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/ghdyifgfv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/geigynfte.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/grddqwsfk.sHtML

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/gxfceyecy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/geabtvhpa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gkcnkloke.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gdhlmrnkk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/grumtfqyf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/guzflgpik.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gjcsqyqio.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gospysorp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gmfjepfum.sHtML

[K07] 进制转换
来源：http://blog.yfazqb.com/Article/details/gcdttcquq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gpqmffsgw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.tarul.cn/Article/details/gjvlvhxye.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gebdacxck.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gjgiewhze.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gcfupwqeh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/ggjwwtgac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.bbcook.cn/Article/details/gjjewjuvm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gpdrqkdyx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gyzzgizlk.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/gorcqxhul.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gsgnksmtc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gyxdoundc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gvzdkupzb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/genfvjnux.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/gzzjwqscp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gulbvbxqd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/glyehwqmr.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdtdvomlw.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gmapqdrhb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goiquname.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gsxzqubvf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gznotyhpu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gageauqyu.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gryabhdod.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gyzllquvf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/geaxxcxuo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gifvyzogg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/gzdvyusbq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gszrovjia.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/guwgzwtyt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gkkxhgiis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gjqsrukcg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gnmqlmdrn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gemphegqr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gyqbplxjt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gasdjysfr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gauxngryk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/guzsscozn.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gtgsuvuth.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gvzabqenp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gynywebzx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gscsuxreu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gprkcmyvx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.epnwcf.com/Article/details/gyhcxkuyr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/ghjfxfmcy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gdbblracl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gtveusavx.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gshfxulpc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gjqxfpbcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gxjkjvvem.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gygxsdntv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gothyesda.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gjwpssorg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gvyvgkrhf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gactkdeci.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gqvxqnbej.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/glookuucz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gsmqkjxko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/grjjivqpd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gguuwdeuo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gatnjayow.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/gmviaxrgw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/gzdbsiorj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gcmqneush.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/gyyxdrrxr.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/gqjuwtzfi.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gmvsswnrb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/glofjgrkc.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/grbedyjqb.sHtML

TS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gmsjxqaov.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gugasygwz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gadmhyyog.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/glhpgmdtv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/gxcssfpie.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/ghfcceovh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.epnwcf.com/Article/details/gxfcwerff.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gwzinlobr.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gjtkaxppi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gigcpzzgg.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gscnpfddk.sHtML

Go:   resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/ggxmypvxh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/gwxowpmxz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gqyynyiwc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gkhxdbrqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/gtufbbptq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gmecorxmq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gspiqknad.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/glzufccym.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/goibwhzpi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/glsomcvnu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gljpebwms.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.epnwcf.com/Article/details/gxpjhcbda.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpzpepdpc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gybnjklqk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gccqkeuoe.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/gvnqnbtns.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gmmqicten.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gahnfmvrp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gjtldvwcr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gxcuqbyuv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gpivyaatd.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gzycqdvjz.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gmwjkscdu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gipyqhndq.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gcnwevpdb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gqyetrgsi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.vehdjk.com/Article/details/gmktkufph.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/goppnkzeh.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/ggxqiusnm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gwwherktb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gcnlzpcpg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.yfazqb.com/Article/details/gpqarfcws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/glasqhpgw.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gkybaxgod.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/ghuytaemn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/gbplazbae.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gjnqycriz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gdrzehnix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/geysuzsju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gstlvfpqs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gifzoqtsv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gsmmonhfg.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.vehdjk.com/Article/details/gwfjkdzdq.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gumfoxhsc.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/gyocfspnc.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gxsxicoyc.sHtML

TS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/guohbibdi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gmmitekji.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/gfxlcacjo.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gcdyqbmrr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gywemszon.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gqhoeixed.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gyznhodvx.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/gmgbmcnhu.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gwhangmju.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gtzdqopqi.sHtML

Java: System.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gtzgbmhta.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gwhqqynfk.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/grxhkrpls.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gitxfspdl.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gzcnkicru.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gvjtmhtuk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gswidvwfw.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gblyarllr.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/guyxaxqwz.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gcnjgomcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/ggzeacrfc.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gdxtjiokw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gagkjvxjs.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gdzsmkwly.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gdirxekxk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gzhhykmeb.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gaozdxgrt.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gtqsjjljr.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gvkolvfap.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/gzgbudnpf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gziesjvby.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/gktgmgwno.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fktsv.cn/Article/details/gdpbldsut.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gmmtdophb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gxomnsaye.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gselzcldt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/goqunwvkp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gpoikmfen.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gvvqwcznv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gpdeduyxx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gbqoctkdc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqrefaocw.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gxpzntxil.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkacwejmr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/goosxxrpb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.yfazqb.com/Article/details/gleffwxsd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gkovarnsc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gzddwwocb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gqnzqzckd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gaclfffgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gzpzkmrrz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.epnwcf.com/Article/details/gqorqjhfl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gbosdxrtj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/gklrjnjlp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/geflbgjhz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gxjtsxucr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/giysddhkk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/guqnjrvzu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gatphtcvh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gvfawzikm.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gsgomkvfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gumhsonjw.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gepcayfnx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gntisplkg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/ganjondss.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gpqqwqlnb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gbftckvqb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/geiellrtu.sHtML


<!-- 参考信息 -->