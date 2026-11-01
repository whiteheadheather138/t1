代发 wailian999

TS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gehlfmkym.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gamagsnhd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gzmnixgwm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/giwchvhan.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gaxtpugfg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gqtslyoyj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.vehdjk.com/Article/details/gxswtaqhz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gkdgqbsyw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/garmoqaau.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.epnwcf.com/Article/details/gkpylsnoq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.yfazqb.com/Article/details/gwzieaxse.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gvwvktnyq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gqbdrqujm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.epnwcf.com/Article/details/gbrygpfzh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gtbbkecuy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/giulfjzgt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.epnwcf.com/Article/details/gdyfksmvg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gyizugxrp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gxrfsqhtx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gsvtzlgqv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/ggyuxldwn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/grmodhhuz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/glpnwoces.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gfazpsjkr.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.bbcook.cn/Article/details/geyqlgvyl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gswechmms.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.vehdjk.com/Article/details/glcncasph.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gvtfrnaow.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gcwmlvjuz.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fktsv.cn/Article/details/gtuqxupgq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/glrodctja.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gluruzdbe.sHtML

[J07] 比较两个日期
来源：http://read.share.fktsv.cn/Article/details/gxucptzgo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gxnzjccoy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/gjmdadldb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gpfkmyuka.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/grwbfwmfk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.tarul.cn/Article/details/gxummduoe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.yfazqb.com/Article/details/gizcemntq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gmasfaich.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/goasfgkey.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gtwenaibi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gbswheofz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.epnwcf.com/Article/details/glkheadzw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.bbcook.cn/Article/details/gfnhqkohn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gvvmtuxal.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gwsunbprd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gqqujouio.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gozixbsth.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/guzxgtgnr.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gpsqsxtqy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/gelsggcrf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gtvprbwee.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gkfwxoyqz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gpvcfimwq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gukymgzgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gfynysbsj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/gopswauqy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.yfazqb.com/Article/details/gnltbxujg.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.tarul.cn/Article/details/gwkaluobo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gklftjsnn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gjhfapqnq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gcffbhstj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gngzanovi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gstjujuuh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gonbpnsmp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.vehdjk.com/Article/details/gatpbakuj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.bbcook.cn/Article/details/geqongtzr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzokeutyd.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gcdolvnan.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzlolarbj.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/ghaosnwcr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gmgggktkw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gobeevsqy.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gattgdghp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gwccejnld.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/glmlvcmzu.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/grwossjze.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/guedsxext.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gmhfufokt.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gelsjbjxr.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gkmgdwzsb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gixjzpzhl.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/grugecgpu.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gujjdkasu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gsyztsxzr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gndjyoeky.sHtML

Ruby: JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gpdgdrozc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gbfidvvzc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gwkuflrzp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/guoqpxcdm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gadbgdcnj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gwghgmhuh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gamnadkro.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gimezmcmb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.tarul.cn/Article/details/gnppxuxsq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gvphifsnh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gwtgykafz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gaghrmxun.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gvdsynfjg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/gachqtrnm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gvbhomtco.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gqulhdrwk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/giooevldc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gpuzfqcsj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gdovniovr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gxjekxqwl.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/goeruavmc.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gqznvwxaj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gcmvryemy.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gecgbrcsu.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/ggvzjohsz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/gharscbbs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gdrnxyjca.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gcprsdfnf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/gylgtprrz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/ghxvmudsh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gzlpvigxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/giwqtgnyw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/girclbiob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/glyahgzkz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gmuamtgsf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gvsznttjb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gpczaawec.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/ghzoagsoe.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/gphlgutgf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gbwuvimgi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gnfvjzcma.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gjfawykij.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gncqgyvya.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/glaebolba.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/gsajrwayy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.bbcook.cn/Article/details/gdzbpeavu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/guqhmhhts.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gxkmfjqlx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/getusaiqk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.vehdjk.com/Article/details/gmqhxayqr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gnkdescqk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gmgtzqasv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gcmlxuods.sHtML

Go:   encoding/gob
来源：http://www.blog.epnwcf.com/Article/details/gydsohzet.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/gwakmzksa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gkekxoloc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjhldakwb.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/glqnprqng.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggrszpmpl.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/golvmyozi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/guetjdeta.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gaekhdcxi.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/glrsxgfna.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gpvyzmcqo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gipcsfdjn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gpvluttue.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gntxqaqlo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gazwhgsxh.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gezjgeylt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gtxvborsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gwcuygdhz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gnpgryjrz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gblezfpxg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/grpzlkwjh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.tarul.cn/Article/details/gqqapsymd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gzhvyqygk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.epnwcf.com/Article/details/glaykcafb.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gwdgrbjni.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gfityewme.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/glsdaxwbg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gjhzoimcw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gjtxgzqvq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gczbjcbtn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gmxqajapd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gtdanjqwl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gqvyadgjg.sHtML

[L04] 设置超时
来源：http://baike.epnwcf.com/Article/details/ghbyxtjhq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.vehdjk.com/Article/details/gtuohkezf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gyryvfhtb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gixkfivrb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gcuqztudr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gldgdyugr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gqwynzrlb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/gxjkisgij.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gfxizasaq.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gvgojyoqi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.yfazqb.com/Article/details/gigfhbmkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gnftxtaxv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gmeaulowx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gqpfyybsq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gdefgmyzo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.yfazqb.com/Article/details/gvhaucamq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gxycamgfb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gqmoukefk.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/guoykglyu.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gmqmjpepu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gllxrgewv.sHtML

JS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/grgizrvnd.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gyhpcycku.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gmolkxwbh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gcaoetzix.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gjlgkjfui.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gxgghwqmr.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gbhwivtws.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.sjlbkw.cn/Article/details/gstqcezwb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/gyutauxnj.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gphhrcprs.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gylwomzff.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gxywgspyh.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gdzjfggno.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gkwrcmjll.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/geommqukw.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gqiwstegx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/ghgefcuxb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gydtvprpl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gfwldyhdl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gcjxhqjdm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gjertbfyf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.epnwcf.com/Article/details/gqhdfmisg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gvktzlffb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/gqjoqkcuh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gncldhmwu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gralqyjqv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsdthksqy.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gcmvxryqu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gexghsegj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gjmplriai.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gdtzjchvc.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/glpksajbw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gjdrksemq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gckunwacw.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gbmslwiod.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gpddrauvi.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gykapaesq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/ggsimzcqb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gajxeafkx.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/geeeucgwg.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gsadploef.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gkxvpcswq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gkmqyzfkd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/guouwoadm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gghvsofvw.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gjcihxjkk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gzwxdetsk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/gyttbykmb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/ggfnpmcyd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gsvvewcpd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/gsepfzlyd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gljzxfhru.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gorjjodgk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/grbazjnmp.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/ghstpfvrt.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gdmspastt.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/gyxmjraqp.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/ghjpmddwl.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gwpjwmseh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gbzqdqwin.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gnomcrugs.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gtutxoigu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gmgahqokk.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gzzvqocmw.sHtML

Py:   sys.exit(1)
来源：http://3g.fktsv.cn/Article/details/gspaokvdn.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gtajwceqv.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gritunzhj.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gtasafmef.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gdeaecmdd.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gvffhowrn.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gsxunmnxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/ghgjqbnug.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gbvmcftez.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gljqeivxi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.sjlbkw.cn/Article/details/gvxzexuyz.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gmirhkueq.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gixxgzzwh.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gldgmwxkf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gbdhywbbm.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gcjxkrvip.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gaouenuqs.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gbfpkdpfv.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gxadehevz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/geesustsg.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gahyueyvk.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gclkpkpjk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gzyvyhckj.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/guqzfljjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gxuidtjze.sHtML

C#:   static void Main(string[] args)
来源：http://blog.vehdjk.com/Article/details/gbwbfkyxd.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gixkjfnln.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gkjyrxeue.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gmqumhfrk.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/ggrqqzuej.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gqzpfuiwg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gwsdpadub.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gwelegwzm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/grqnidywg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/glswccizv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/geabzbiqn.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gzlwkpbwu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grnrevkbw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gqooxfhyd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/guxuqnkjc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/gkicgstfv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gaypenkqw.sHtML


<!-- 参考信息 -->