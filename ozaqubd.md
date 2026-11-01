代发 wailian999

[J03] 字符串解析为日期
来源：http://baike.fktsv.cn/Article/details/gjslbgrkp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.tarul.cn/Article/details/gvxzehcsa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.yfazqb.com/Article/details/gcqssatxx.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/glukvnjxl.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gsshhhfjw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gzwnfrwcq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/giufawguj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gehlhcnvs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/goarngqwu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gbjjnzbpb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gdsmrraky.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gprcybpwk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gyzypscep.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.vehdjk.com/Article/details/gcgkqbohv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/grxivlxnb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gwguhmfec.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gciqqhcjm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.epnwcf.com/Article/details/gwzxiixxc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/gozmwgxqg.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gifedrjgy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gadvtnrqw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gomvthhij.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/glhgcmapb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcauyngz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gxoyomimw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/guhmrvslx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/grmlywvmz.sHtML

[J06] 计算两时间之差
来源：http://read.share.epnwcf.com/Article/details/gfvtoxqtv.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/grmckdzts.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/grhtspxts.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gvbujfahg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/gjqdplsph.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.bbcook.cn/Article/details/gxbimmqkt.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gkmztrxln.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/gkndssacx.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/golddsams.sHtML

[J07] 比较两个日期
来源：http://read.share.sjlbkw.cn/Article/details/gpabnzylb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gymcoappq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gxbnjncti.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gyssgruuj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/glifwbhvn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gestyxfol.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.vehdjk.com/Article/details/gbqdpugrn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gcwjrunvh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gfhbgyfsu.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gcnwwzuek.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.sjlbkw.cn/Article/details/gbtqsttez.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/gfxbxwmpt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gymxayffl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/ggzhawclj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fktsv.cn/Article/details/gyuwgfdye.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gcsipowzi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.yfazqb.com/Article/details/giyxrfdei.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.yfazqb.com/Article/details/gjkapnbiq.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/gtcqmhltt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gqucmjaxb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/gskouxjyr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gvksczvue.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gcqxnkwgo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/godyvwpbn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/giwvqmpzi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gvlysumzn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gliyxedmz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/gnbmljhbv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gigvivnit.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gfykixirs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.vehdjk.com/Article/details/ghyojavxf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gwydpuiug.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gqbsniokb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/geonisriq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gkaxidlrz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gqmarunmz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggyvobyed.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gvnevetoa.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnohgwtgz.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gykmywmkt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gekevetdk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gzzufqbfj.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gqgvvlsnf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gwfgaqkou.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gxamycvak.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gtyixbqtf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/gdtowjnaj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gquxlzyxs.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.bbcook.cn/Article/details/gddgcwrte.sHtML

Py:   json.loads(s)
来源：http://mobile.tarul.cn/Article/details/guaazxmkp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/ghaempnzm.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gjrneziri.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gqchpmwfo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.yfazqb.com/Article/details/gzwhhbbit.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gdckvwmgi.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqwjbzcmi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/geqwnlcoo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/gntflfsud.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gopcjajdv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gkqujspoy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gtevmlbrs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gzrwmhuaj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbdvypxmm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gfsbexrlx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.tarul.cn/Article/details/gjhzsbtwo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/gvvtuosla.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/giplzsokl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gwldmmnfu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/geqfzudkl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gwunazfbr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gfvhzttya.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gqoewcbji.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gisgmejjs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/gbsjlloio.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gfswjshxp.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/ghgzcgqlx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.tarul.cn/Article/details/gghnbdmuv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.epnwcf.com/Article/details/gldmybsyt.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gautakxmb.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjxnidkns.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gpvfbgjel.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gjrgmkbzm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/glwrudjfq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gaouyehis.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gedassmuq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gkipqsgzv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gbalzyzzj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/ghgzzbiqm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gybimyrbl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.tarul.cn/Article/details/glxxbmycz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gqpqckxlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gfwwsfctj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gzyqwqouy.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gatmfzlvi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gdcwxfbej.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.vehdjk.com/Article/details/gpybdbdya.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gpaiqjdrr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/garquhdxi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gaoitkcgf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/glxuxhvzk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/goxroitmi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gvieayykq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gwhxdxjym.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gbumokvpo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gioioqpke.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gkjhggzal.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gmshgbiaa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/giaxptkec.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gkxsvjqjm.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gvrecmkli.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gdedtccmc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gilcciqra.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gfarywjsn.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gosbaofss.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gbzbczxbv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/ggvdrdfvk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gvyrekqhh.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/ghoiphumo.sHtML

TS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gfsnbjmmz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/gjadpwqrh.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gsrcixquh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/gorvcipvi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gjucttmnt.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gdpbvmskh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.tarul.cn/Article/details/gidrvgjyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gupsovrdz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gpsbuujmp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gwlatjufi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gbaxccqbu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/gcfcpxsfp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gmgvuohna.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gjbbyocmc.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gmumuvcep.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/gnrssvjqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/ggsyhlmqg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/ghthajogu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gfeovdmaj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/gxgwepmru.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gogubbmqb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gcjjvgvbc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gjhbekunp.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/grljczwhn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gunwmrnwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gistbuyxp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gknfqcxkg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gtytwxpxl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.vehdjk.com/Article/details/gjwpbgvkb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gejcbxvxj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gmgxdttxy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/ghihiaoul.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gcheoajkk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gkaypkdsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/glwaxczjh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gedsnjaoc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gtsksqswu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gtedzxufc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.vehdjk.com/Article/details/goqgmthbl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/glgujyudz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gkqwoldiz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gpschetso.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gkyvtomrb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gioyigksd.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gjmbelbox.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gdvqffiwj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gzsmxphek.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gsqogastd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/ghseyrijm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gctjhzgpf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gdrjwubfb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.yfazqb.com/Article/details/gkgayjrmf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/gtnxwafeu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gmxdzytgf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gjnkrobpy.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gnhzvzuwe.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gkehkyawe.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gqpbvofxs.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gozjqmcsp.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/genzooanc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gvgneeegp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gofdupvmz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gaskkzmaf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gswnljtks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gkfysvqdl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gqmlwvbfj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gjczhyqmk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gdawcjght.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gumusvxoj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.vehdjk.com/Article/details/ggfwsoqst.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtmitmprc.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/goucrnfis.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/ganvnyijj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gkaepvuqt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/glyliasvr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gziukghgr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gqwqqfzwi.sHtML

Go:   os.Args[1:]
来源：http://wap.tarul.cn/Article/details/gnuntotsl.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gwootbjxd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/goarklwys.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/ggolhmgso.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/glpvbypfl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/glapmowik.sHtML

JS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gccqkucjn.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gkjkunivh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gvboswkrc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gqtdlccaz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gqhetirgj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gtzxirrot.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gwqmcurnb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/ggeiqxseb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/ggsnrrlfv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gkaxuiogc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gixhlbnbu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gkbntwaac.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gzzobviev.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gbudhkvbw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gtgnslcbu.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/gjejhmbaq.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gqxlvcefh.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/glfbnpxwo.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gjlppzsyr.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gbhqqntza.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/geiyhdzpw.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/gaxhsbarp.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/gzxqxqzht.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gewonvucw.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gixpjfgth.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gnlcgzcnl.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gtxhavkdm.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gptyivawl.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/glhcdlyup.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gfyqwbgsi.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gwmwrqphi.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/genyrztgu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gfrwykqsa.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/gihmqswuc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/guyzrusyy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gyffowzgf.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gavlqijeg.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gyinakxbp.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/ggsoadiau.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gcrgcyrja.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gliafmgmp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/ghiyaqkjt.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/ghbvnvdua.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gdazevfgf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gyvvyprrn.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gzopltwnb.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gzqruecob.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gyfhwyjhk.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/grcalsggh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gcurxgtkq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gpgsupmri.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.epnwcf.com/Article/details/gzwrjehxu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gqdxgzazm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/grmxafnlp.sHtML

JS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gwsggickv.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/gmaxxbjkf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/gdrrvqfme.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gjzyiipxn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gtleqwmcs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gbrctcjey.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/golflwuya.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gznwctncm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/giptbncni.sHtML


<!-- 参考信息 -->