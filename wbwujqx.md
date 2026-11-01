代发 wailian999

[J03] 字符串解析为日期
来源：http://mobile.sjlbkw.cn/Article/details/gpiuwweoe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gkrlcunxu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/gcycptezt.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/ghrrucnlb.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/ganvezcty.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gytveoggs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gugxuvfse.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gftnnxmrx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gtkjkpkoi.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/giifazyne.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gejqdxyfi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.vehdjk.com/Article/details/grtvgvitf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gwxwgxskz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gswwmjksa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gwzmhqxwe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.tarul.cn/Article/details/gthwsysvk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gpqquutfm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gzxgmnolz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gdkkwfono.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.sjlbkw.cn/Article/details/grcowjrio.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/gmtlzrksv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/gvyodpnko.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gxpbjzfgj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.vehdjk.com/Article/details/ghpsatvuu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gsydckesg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fktsv.cn/Article/details/gtxejrqni.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gtazxkhrd.sHtML

[J06] 计算两时间之差
来源：http://3g.sjlbkw.cn/Article/details/gbvtjjddo.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/gtyynjqfp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gabducjhl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gkironcjd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/gdvbnddxw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.yfazqb.com/Article/details/gohclavdd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/goyyowuen.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gcqgldmct.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gyzchzrzs.sHtML

[J07] 比较两个日期
来源：http://3g.tarul.cn/Article/details/gifrftyxf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gnmykilzm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.yfazqb.com/Article/details/gcmkfbsgv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gyhzcdqmb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gsgxxtjvr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.epnwcf.com/Article/details/gxehxerza.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/gstgjtzjo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/goeagnezg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gvqehxcnv.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gdkklofyw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/gqulanbmv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gvrxyvbjt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.sjlbkw.cn/Article/details/goezcxkhe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gharmphsn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.sjlbkw.cn/Article/details/gptrpmrzq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gwtlultzs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gdknuflfl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gcowiajhw.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/golekkspq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.sjlbkw.cn/Article/details/gzkosjpoh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/grljhrlfs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/griqsmtwe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gszohlybm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqagpqfbx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/gmrqzlzka.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fktsv.cn/Article/details/ggqlhajyh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.vehdjk.com/Article/details/gnghohrhi.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gwpkfripv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/gpxnudvft.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gojutrhyx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/gzflpdgdd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gjczhnjye.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gmqowuhsd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gcftsotmk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/gilcmvfqf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/glwlhydyc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqascrkhs.sHtML

K. JSON 与序列化
来源：http://mobile.yfazqb.com/Article/details/goehgnkue.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gtcmbnctt.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/ghwuhcwwl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/ghtmeoxso.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/glzcffmde.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gshxwilsh.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/giqtulzye.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gixhehcqp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gqajoopzk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gylyjmmnz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.yfazqb.com/Article/details/gdxrovbzg.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/ghchexehs.sHtML

Py:   json.loads(s)
来源：http://www.blog.fktsv.cn/Article/details/gipfqueem.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gxtlxnhzb.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gwfsxexhe.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbuqrxlrb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.epnwcf.com/Article/details/gltkrporc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/ghhdcrmeg.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/guwalkjsz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gukfuipgd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gpzobkshw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gdzcrigph.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gzpjhrnay.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gbijizrda.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gscmrzuwe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/gbdpajtiq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gcybkvlnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.vehdjk.com/Article/details/gadayuncl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gebggtzuh.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gmexyorpq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gtkilmfxh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gddtajwfa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gmeohuetj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/ghtxppkfm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gonyislct.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gzwhvcllb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gyfehdgnf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gkiitbrpx.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gxaxfqojh.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/godpyokmp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gjewdizay.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/givouxgln.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gaabfhcyg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.sjlbkw.cn/Article/details/glvsnywxn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/gkjcnqrlf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/govqvazfv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gwkhgqgwj.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/gaupbpmeb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gddeohjbo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/gwajieokv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/ghgeelodp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gyhoymkrf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gdahdrpse.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gbhzkhykk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gjqvnklbf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gfwyrthph.sHtML

[K07] 进制转换
来源：http://3g.yfazqb.com/Article/details/gvxldmxqg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gafkalpph.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gkkrmldec.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gemnbtacw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gvigrbteq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/goethujsx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gebvdkewd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gcnnrdsho.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gikkxyheb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gjchtrpuj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gamuxkrzm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/giifikimf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gugtplwjb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gwyhwaxha.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gcvodsixn.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gytdwkrgg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gltxuugrg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/giugaxeze.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjxcqkvjv.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/gdyjjyuxn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gspdkwcbi.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gafejyvsu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gejwouihy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/grgexhhgr.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gplfwmrah.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gzwgenooo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/gwtxhcfcj.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gsowbwgqf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.vehdjk.com/Article/details/gngraireb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gswihmpyj.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gybhosbrh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/ghgcqgbol.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gvevlydok.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gzcqixhzb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gipmwkkwn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/ggumvqdzc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gsiobragw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gzsvleyfd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gownhwawe.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gtbexrukb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gkzsrashf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gqwvhgrln.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gzevykjan.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/geqrhelfv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.vehdjk.com/Article/details/gjdfwmcwp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gzqnfayyd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gwjerpvzl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gzmfwulsk.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/glbiciyym.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gftzlaobt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gqefdsyax.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gwjihzyvg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gofwwqgii.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gkfwjxwlp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/ggubtnlte.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gtuyourup.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gzxwxgwna.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/gkekkirgf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/grivnullw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/grqypalol.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/ghjsrycos.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gtdvsaasq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/gllmkgmax.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gxnkriaxr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gindxivpo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/gtkeadpcj.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gfpqvidwc.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gqkmcqvnf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/ghfiiavof.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gqyptnoxp.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gehzyvazu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gkqrdkcua.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gwchalvnn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/geutfwrcx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gktxcealp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gprywyzyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/gcrpvwdvq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gpowrtaha.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gghvspacv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gyhpssaqn.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/gdlnhvlay.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gmwtlucjj.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gnngorbkq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gegebnqzt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gxqqlkdys.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gboqhxcth.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/goyejmzhq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gqvqkamsq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gtjdkqorp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/giglbnqtq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gewpmbclr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gygrujmsu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gowwktacx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqymdrium.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/gclnwbipp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbneyerei.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gfdwwbfnr.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gpdxyoyvw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gqqnoduyg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/glkxwurae.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gbucxwhgx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gzlziyekn.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/grgbdaont.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gnrlqfhye.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/ghzdlhokx.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/ggvzcsruk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gsnovemdy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gounafvmh.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gemvdtlet.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gqurrseni.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gzypbvrnj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gunafekgt.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gujaegcav.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gulwixrbe.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gfvqmggpq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.sjlbkw.cn/Article/details/gzuhpruro.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gtbmjwxsd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gknatumgz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gnpfmslif.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/guykoqvmz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/gunqkzgnm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gtgjijoxj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/grdzecenh.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gieydfvsc.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gnfkcsoio.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/ggrehwxoh.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gqhpesjfv.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gxwroecxc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gqqenlyxm.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/glszwcsso.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/grqeroihj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/guijgpqfq.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/ginafnrmj.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gkcfygrjq.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/ghuaslghr.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gwkufjzxq.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gcqzgiqok.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvmcovfqz.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/gawgjyvtt.sHtML

Ruby: exit 1
来源：http://m.share.fktsv.cn/Article/details/gxodkwkde.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gslxzrvja.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gbgdhhiso.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/guhmbfogp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/ggoevtybq.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gwkczuhyf.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gsoxyfzsr.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gxitrkgtk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gxprscbqc.sHtML

Ruby: warn "err"
来源：http://www.share.tarul.cn/Article/details/glyvwdigf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gibjdqzgx.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gzijmoxbl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gfxxjusko.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gzgbvarkf.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/ggpljvuaj.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gbkkyndyo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.sjlbkw.cn/Article/details/ggkeyvqqe.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gfcseajvy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gevgxeasa.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gtxyavmhj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gaugyajrt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/gofkhbbbw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/gqhwvroub.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gzylunwqg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/getpuhtfs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/giprvlvfg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gbyducvcd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.vehdjk.com/Article/details/gswppyagq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gpngwbyai.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkidpxkhb.sHtML

N. 数据结构与算法
来源：http://wap.fktsv.cn/Article/details/gmmibiqil.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzwlyagzf.sHtML


<!-- 参考信息 -->