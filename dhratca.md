代发 wailian999

[J03] 字符串解析为日期
来源：http://m.share.yfazqb.com/Article/details/ghppwbzms.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gngodwqoq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.sjlbkw.cn/Article/details/gmvhubgmn.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gfxcuhkqw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gehesrfrf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gcfccmaky.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/galhthnej.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gxqdettad.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gcsxcybij.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gfxbpfjul.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/ggxosesle.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.tarul.cn/Article/details/ghtwkesjs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.bbcook.cn/Article/details/gtucwtqrd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gvldodonl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.epnwcf.com/Article/details/gvycleqip.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.tarul.cn/Article/details/gyjfuoxtf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.epnwcf.com/Article/details/gkjdrvsva.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gfuoaorzr.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gnzolnvnr.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gmeslazpc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.sjlbkw.cn/Article/details/gjorqfsdp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gllknwyxm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gnxnkarkg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gkzctslks.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.epnwcf.com/Article/details/gkoqrrsro.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.tarul.cn/Article/details/gvwviyxvj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.vehdjk.com/Article/details/gsgceddlf.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/gbkpkxqgv.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/grmvtjxxk.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gwowrfdmu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gfkzplrli.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/gzpbhvags.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/glintppmj.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.bbcook.cn/Article/details/gayesfdpi.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/geovennlb.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gbohesoaq.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gkymvqzav.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gqjktqzrr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gkdjniqwg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/ghjdeetmw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/ghsnbudbg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.sjlbkw.cn/Article/details/grtckhqpr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gwuzqkcae.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gngugitms.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/ggevdnadg.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.sjlbkw.cn/Article/details/gezospofx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fktsv.cn/Article/details/gcshfxqav.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/ggzpqvwop.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/grfhuwpiq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gkfsgtyoj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/ggtnnbbuk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gwlyrrhzf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fktsv.cn/Article/details/gbsybfvow.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gmeesnyoc.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/gsfjlwhlr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gwqsfvqkq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.epnwcf.com/Article/details/gyahvnmqi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gieqzvrhx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gzuhuquwt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/ganhdkezy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/ggbzkcjty.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/gxalnhczb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.tarul.cn/Article/details/gieyanbqm.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/glactqeyp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.bbcook.cn/Article/details/gkzufbwnr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.tarul.cn/Article/details/gwthoriny.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gtjbifxjl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.yfazqb.com/Article/details/glnrjppen.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gpcpuwjxx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.epnwcf.com/Article/details/gcovqnqpo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gtwewtfze.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gtsbpnmcw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/giitwjxiy.sHtML

K. JSON 与序列化
来源：http://www.share.yfazqb.com/Article/details/gxxanmkpe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gopfddfrw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gvixzynql.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gqtnxwbvd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/ghnlsqknj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gtqajlbbz.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gcsoznumi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.bbcook.cn/Article/details/gpkzfoaya.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gssmdtwxz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/gmsnihwdv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqfhevehl.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gdhonzrfk.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gsqhzcezj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/gojskwdlu.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gcpxqrdti.sHtML

TS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsnuwbsrq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gzzrbptev.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gfkueupai.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/glkwkgxxb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gxtropdda.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gsroqvxeg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gaqrpuupq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gvxtvfpxx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdogwnxam.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gfodmwpru.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gdrqriuqz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gfmvyjjnt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvbwqnwvr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gjewmxncu.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.vehdjk.com/Article/details/geefqrqmo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gsobcovnh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/gyjvbckyy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gtirskumu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gdfnnhtyg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/griwlhkrc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gtbnflsns.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gwvozwxyn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gtoitvinn.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gomqyzcdz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gsshjcras.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gcxgyhxds.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxlpapdxf.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gmycyokvu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkqmembk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gelilpobo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gecenhznk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gssubipow.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gemlrpqnq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gieeibacc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/ghyzujerp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzllfayek.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/goruxspdj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gjfjwgsqn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gcmakjdna.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gsbebebat.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gokmmafkj.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/givfdptnk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gsbdyjtil.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.vehdjk.com/Article/details/gizbhubfm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gbandauur.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gnpkroeof.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gcdcaqvgm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gyzprepom.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gayuywyhl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzyofyjdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gkdffjspg.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/glvocsfjn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.yfazqb.com/Article/details/gktusyzsv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gxqzeyjvi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gjilnpbgi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gjgiswgfp.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/grfidnamc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gxypwonej.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gxmnpgbdy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvtbewktj.sHtML

L. 网络请求
来源：http://read.share.bbcook.cn/Article/details/gtfgowlua.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtamgcsyf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gfjveqbma.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gqcograpy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/gjtmoyezh.sHtML

JS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gufrkvbgx.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gjokhahwa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gebzorwpa.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gzlkyrylz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gszlhiact.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/grgdypxlx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gibcdbglu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/goqasvlmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gdxsgvusy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gxhmzafcd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gcjaipixe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/guyxyjzik.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/gkzuifcet.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/guenotwqy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/gxvojxntb.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gnjqyyfso.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gxpvetqsd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gqfkcbxdr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gmtoueetc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gygetixig.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/giszgwyca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/garfzhnxi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gjhfmbziv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gbwyjcpvq.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gmpuuvxcm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gcrfneyny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gszajqssf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/goxknrxsa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gabhwofon.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/gegzspoiv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/guwvdvhhr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gerotccoz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gdttavhjz.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fktsv.cn/Article/details/gtgvnzhom.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gjjgtyfei.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gjopuafus.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gtueksrxo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gmwkqvxzv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/ggwugeflu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/grasdtdpj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/ggrigejty.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/gdrvnxsgr.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gmrjghxvc.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gkvlxibww.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gakpjypnb.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gryyxbdir.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gmhmbxqhg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gfomuiqjm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/ggcipgeyr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/ghxbtgvnj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gxljpkotx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gbpdrbybe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gvanwhfro.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gyyhwcbvo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gprfgeplq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/godtgaahz.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gntxadteb.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gydvulupb.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gvdcymeli.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gmimfvwni.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gogkarcjs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gkjufpwxc.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gpjpvkwem.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gkcpgjnij.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/ghhqinkmj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gwsbgmupr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gxmuzpjen.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/goblvfqsn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.vehdjk.com/Article/details/gilflsrsj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gblmanany.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gyelfdxjp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaoighemt.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gmwbdkqkr.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gtewqmwec.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gatbljmbt.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gqkbvvqed.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gqlaercrt.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/grdxtpiuo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gxxwrhgtc.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gqxfkfxtl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gyiasbsyn.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gptmdxmzy.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gyxsdromt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/ghbzospkp.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gupmixgxg.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gqcaqpaqa.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/ggqboikdo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/gnyoinxue.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gndwyusze.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gmbrxiywd.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gmwbaxkps.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/glrtszmea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/gxbjeckij.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gtugvwohj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gbefwdinv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gbvoekjox.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gmihzgqvs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.bbcook.cn/Article/details/gxogliwho.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/ggblrowwp.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gypbbqhvd.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gooquwxkg.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gneihyhee.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gdianvood.sHtML

TS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/gjuecuita.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gteizduvr.sHtML

Go:   os.Getwd()
来源：http://mobile.vehdjk.com/Article/details/gdakjpixd.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gzoriccuu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gphlncoln.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gomglowyj.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gkmnnynzh.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gyzsrbjki.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gguuwzsfc.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gckdmfzxw.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gtieloosd.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gungelsfc.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gtcrwdoug.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gpgidrjoi.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gzaphncuy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/grbslqgjc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/gdfiljnbr.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gdmuaaere.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gsntlzfyc.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gskejdztq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gitbppypg.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/gvmldmidu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gjlqokwum.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gcobotdyi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/ganewdfiz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gpiiqenlo.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/ggbihwmqf.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gfdzfppfy.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gmnniqrmh.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gxkshulas.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/ghinsyvqe.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/giaphricp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gvoyhilqk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gdxvxrvfl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/giuwshpeo.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gcqhqljkr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gjsxzmfah.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/gvmspkngg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gbrhnthlm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gycyxriiq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gumndkhsd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyzvpqvnp.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/gpqkfyuug.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxmbughlx.sHtML


<!-- 参考信息 -->