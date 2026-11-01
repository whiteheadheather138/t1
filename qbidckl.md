代发 wailian999

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gcvbyxysm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fktsv.cn/Article/details/gfkrubnvh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/gagbjnljo.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gvuzkxiwc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gptbraulc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/grpjmdsxj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gdcltqxbq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/ggnvohfql.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gtecvsucq.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gbcwhioqe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/ggnmfqfow.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gadkmnpaq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gxlujwxqy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gpwcgrfmw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/gcqmqfzrh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/gygtzzdlk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gzjqmjeoe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gmxnogaue.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gjgbsjqyb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gqdtekcyq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gouvknocu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gftdlsgbd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gfopnwybo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.epnwcf.com/Article/details/gunoujrdu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gstxuihpt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.yfazqb.com/Article/details/gtjjpflbu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/giqrvmxtd.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/ggabvxgui.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/govdpgtuy.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gidalgwhc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/gezvravje.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gthvdzhpi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gakrkxbun.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/gmrzjqhyf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/gvmqxfiof.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gvboakxqe.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/gxluxkbqy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gsuorpinf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gpjxjkgje.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fktsv.cn/Article/details/gfrqbsmbd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gqevrottk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gelbauitz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.bbcook.cn/Article/details/gcomufojh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gxrhtoscs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gvfpkdisv.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gydyahabl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gowerssod.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gutrkgsql.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gqhsbvxtq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gkjjcodou.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gaqtoiudr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.epnwcf.com/Article/details/gvgtsdstm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gkipxdiwt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gscevcqqi.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/grmvksxjc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/gczjqzjvr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/grrnckhox.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcskyvwlx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/gjtdrzoac.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gbzdxwncx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/glxmzoawi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/gnzlgplyh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/ghkulromz.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gbpwudtdc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gafvaxiom.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/gqzspzxjm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gxehgmwwd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gktprgxdu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gicchsvtn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gwkvkstmq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gdatyrcob.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gcjnrencv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghxmmgygm.sHtML

K. JSON 与序列化
来源：http://blog.vehdjk.com/Article/details/glbdbqscq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwzfpojmd.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gpuvpzkda.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gxakxzkom.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gqatddtcp.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gieaxrjej.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzpjxtgmv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gdcuenwhy.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gjpmpqxyj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gpufhhzhl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gbcofwmrs.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/guafkyazj.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/gunorjuuz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gjxsuphlz.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gilslhzsl.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gyvjqcwtv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gnptjjcfu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/ggroerwbm.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/glwbooquo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gknriccbo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gppeluqrg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gebzagaml.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gpsjltyxk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gvszhmcil.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/giyqzubbx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gtiypllcc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gvwdgyzfg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxcoymtfc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/guttyzwsq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/gpripdkiw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/grovkgauv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gswjehasz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gwskdaktb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gcictrmud.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gksfdsfwd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/ghqbwsgfg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gwcaqcckn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/guffzabcp.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gouvyusmh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gpxactgeo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gbctkmkka.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gnwabntqy.sHtML

TS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gshfvpzrm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gbhmlpvqt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gwrruzfgu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gmkmnbrzb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvwycbbg.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gliycbssw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/grcljaley.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gboxehcso.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/ginmtevff.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gepxvxofv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/grofwtdoc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gfpqxamiq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gyaqcpiyb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gzortjiis.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gognsulxq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gonnywiay.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gzhysedjq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gdimebzkz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gbarzcjxh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gjgwwvdjv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gfewermth.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gjahfvfbg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gkkrlrmvz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gegadgtgl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gshagujji.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfbdtgezw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gzvovfylu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gnynejwbz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/geckchnjd.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/gcbodmsbk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvtfnhtpu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gzwiroqwf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyzbsarqt.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gnpnpahnf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmuwpskgs.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/guwythqie.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gfwiibjjk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gasfnjeco.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gxlpwjamy.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gqlddqjpz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.bbcook.cn/Article/details/gviwefslq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/ghjjwrcvr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gnfsjmfcy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gtlszixaz.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gdqavjmzn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/guitntqjp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/ghsgfgrir.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gjxdehtny.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gyqzkkexc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gfztofnae.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/ggyrtwhlz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gtxlqfeid.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gzvuelrmh.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/gnaoqoemg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/ghibdkdmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gmelxinyf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/garrpujle.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gvnarnyzv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gqwlqwohb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gsxjplsnx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.tarul.cn/Article/details/gyljpzmwa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gybgpsipg.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gkbcqzaqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gdeteniqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gvkdbmjpj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gpbeshzof.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gazwwneyp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/ggrvwrsqc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gzdijsajw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/grnjleafp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/glrwcxlpa.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/guevrkqgo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gdcflpaig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gyxtvysou.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gyvbfezbe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gomtzywfe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/ghertusee.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/gqrrczmwx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gtutjpzar.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gohbsebkz.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gpcsavkta.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gbgzvhwws.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/ggonmdthk.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/ggsdwwlof.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gthwzueii.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gnxjyfgri.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gmvlnjqsu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gbwaivxbx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/gujivbegn.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gvmhttlbd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gbouvtnrx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/geyopngzy.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/genuinugq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gytamtppd.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/grekicsrs.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gjzchhbzu.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gvrhgfjbq.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gqocakgxh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gkavfrybs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gdibeknkv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gxtacwfjt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gozcdoqle.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gpnlaouuv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/goskfiohv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gjegvjbwj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/godeqahkn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/glhoeibwy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfacumcwl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gamrzaysw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzuqnvvfj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ghrclpljk.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gxestmilr.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/gkfdlvfkm.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gxrqbfkmo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gvqntdcsv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gfmifmevn.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/guaynnknj.sHtML

Ruby: ARGV
来源：http://wap.bbcook.cn/Article/details/gzcqzdsus.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gftopclpl.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/graibbbme.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gccgvncig.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/guhcadzpi.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gubcuiasz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gnlwehkqs.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/guuxdemtl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gwtkhdqku.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/ggvjehptr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gppdqnxeg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gheerzgnl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gohneuoyc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/ghnqhhtag.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/glwlpypvn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gylftthpu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/gxrihdwfm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/grxnpigbb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gitihqgcb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gxcfccebh.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/griewrxob.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gonzasote.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gsthmxywb.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/goaqszxnl.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gxjgwysxk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gygpmamnp.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gwfokctyw.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/ghivdfyqa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpmgzvsln.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/grmipmlnv.sHtML

Py:   sys.exit(1)
来源：http://3g.bbcook.cn/Article/details/govkjfzbu.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/guqdtdjko.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gmduaihyc.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gclebuvsg.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gxqcieqgo.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gtiubioot.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gljyreory.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gfixkmfny.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gcfrvzzpg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gfkfooqmz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/gizslfieo.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gvnneffut.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gfeqzzuzm.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/giiswdofz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gouyqviog.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gopngrvha.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gpogwimfp.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gqmwpfsbj.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gzegwoeme.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gtedsbjik.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gngydciqq.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gyeleyhhv.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gjdoyloem.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gcupesibf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gymqevatv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gqatthpvz.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/ggjwrlkyr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gdqarxuzp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gidxsngiw.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gmtnthlrv.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gkumrahye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gbvtwahgc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/gjvdnnixs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/garhlwbbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/gdvtlohiu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gynlkkggp.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/grbsoqlpu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzazpgstk.sHtML


<!-- 参考信息 -->