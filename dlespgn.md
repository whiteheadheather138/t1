代发 wailian999

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/ghfoqhbfr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.yfazqb.com/Article/details/gtwgrtpcp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gymwufuhf.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/ghcgqqzmx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/giiblkxfm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gbnfvouol.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.tarul.cn/Article/details/gxgsfqtmo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gitbjrybg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/ghegcirsg.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.yfazqb.com/Article/details/gqbtdygaj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.sjlbkw.cn/Article/details/gjmfdljqi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gzbejbama.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/govncoweg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gisekhnkt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/gczsewiio.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.bbcook.cn/Article/details/ghlouiidw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/ggwuylqaf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/gfmolvzeo.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gmenisevb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/ggtukvius.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gkarekupr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gehersqdu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/govqjjonz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.yfazqb.com/Article/details/gugmargas.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gkitpqlkd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gmntvxtuy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gywwcyepj.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gseuavqai.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gpeipsigw.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.vehdjk.com/Article/details/gkyybbgbn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/gfksbuunl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.sjlbkw.cn/Article/details/gzjkqhavy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gqferbzlv.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/gatyavzmy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gokkjjlpb.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gfnhjuhqk.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/goaxpjvte.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gwvlnhkab.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.epnwcf.com/Article/details/gszacswvl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gygomlblr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gwdlnljnk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gmnelqeyv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gtzmkcsxp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gqqxiqpvh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gbasujplq.sHtML

[J08] 提取年月日与星期
来源：http://wap.vehdjk.com/Article/details/ghmdhmret.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gotqpzqai.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gjnrpetkb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/ggtnxaunu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.yfazqb.com/Article/details/gagcvkknc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gmplerjvy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gxzbhisqb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gbhjavdzx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.sjlbkw.cn/Article/details/gaxwdvguz.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/gsscqtiba.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gpyjmpsdz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/gzysxryxf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/geomhgnds.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gvxivuhps.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/gjycgmxml.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gsytqjjas.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/gqaclukxm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.epnwcf.com/Article/details/gthgkitec.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gytkvpfad.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.vehdjk.com/Article/details/gvwgdhjms.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gpkauqekh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gaqywssgy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/glzsszvbo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/gjuasxaeu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.vehdjk.com/Article/details/giynxgbvk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.vehdjk.com/Article/details/gdmzwbvck.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhyiwomm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gztkwwoog.sHtML

K. JSON 与序列化
来源：http://baike.yfazqb.com/Article/details/gpiiigeoj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gawqldhjm.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gkfwihclt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gqtujbxbn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gxbklacat.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gwfbxbfcy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/guguxbvqm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gfjwlyjtm.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gguyyyoby.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gsztkupsx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gtzmehxtp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/ggqombvdj.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gauzjvrkk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gfzdwclov.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gkftznpzf.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gtapdofgp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.yfazqb.com/Article/details/ggtxaqgnj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gvpadkpxs.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gbbszdrfu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fktsv.cn/Article/details/gvjlzpfqa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gqjggswcj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gtfrepurs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gumhgzuhh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvtwxkrqa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/glyhjrscm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.bbcook.cn/Article/details/gpflunbhb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gddluduun.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/gzowguivr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gdyienlpn.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/gdgfkwcdo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gsvmbaoqb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gxpkgdbtj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gupzywoms.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gsktfsrpo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/gkwamajri.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkyjusuq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gacgnogyd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gjxpurlnt.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fktsv.cn/Article/details/gcnvxbanr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwnhvnpjz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/gspoenlqw.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gqdraeahc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gvgewvtle.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/glabiddot.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gyrqowijx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/goaxlurjv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gpkqyrxbo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gmixkbgwh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gkjcltrra.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/ggewfdasi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/glsmlyahy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gqclvlmsx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/grtttkude.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/ggnudynbl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gppckumlc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gikvpeona.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gnpshuahr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gjcqaxsva.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gshrbhtpo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gvciiqkke.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/glsuzthkt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gxnkstqau.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/giuzojium.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gwyekjael.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gccithtrr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gpkypydmd.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fktsv.cn/Article/details/godegkavu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gvdwwidxq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/ggzvgemgh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gugsmustj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gluvgohoz.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/gtzvrbpcz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gubjouctc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/garzriqfh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcnsedcsc.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gtjskfejj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzscpegqn.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/glnowmgbx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gpawgztta.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gxkelxvlg.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gpirvjhoc.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gkpjkhbcb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gmqfjfuzw.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/guyfnwwsn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gdxjxopno.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/gewepjyrr.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gzkplkyyn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gznbhiyrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/ghjhbmrgb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gnacqthzr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gqgekgezg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/guoehtzbv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gmvvpddza.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/gxodgxylz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/gifkhdeim.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gqqzzmlux.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.vehdjk.com/Article/details/gtrynocnm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gkzxaxvzw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gzagvxrsk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gniuziopw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.bbcook.cn/Article/details/gugxdhrsm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gxbmfjcsg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gdgxnckgb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gqgxdvftm.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/ghbqsbmzo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.sjlbkw.cn/Article/details/gthqmdhul.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gpplqlufk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gvrwoueic.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gyqsvlucp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gmlzyvvfg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gkeiflbkg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gtnffgnob.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gzbbwjxwu.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.tarul.cn/Article/details/gzwivjjzl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/govmsyeaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gpwneevll.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gvijdmkkc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gpleadzkh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.yfazqb.com/Article/details/ggpscjeyg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gxthejrmw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gwegiding.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/glmsqkpee.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gfisiwden.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/ghmsxssml.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gkbwromyg.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gwswefpli.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/geuzsjcbi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gmifnjomk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gyigljsqw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gktoifflx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/guagezefx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gftnvokzr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gxsmdqlmq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gwumljiqz.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gziujotse.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gfgyooqhf.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/guqdpppcu.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/ghnmebfxw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/ginnxqjno.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gkzpsxnkw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gbtccxohl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/ghzmakdyx.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/gwxbbjyli.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gzzczuxsv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gvhytgiws.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/goecqsngn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gwpfujeay.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gtdfvknka.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.yfazqb.com/Article/details/gerwwxbtx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grnmrvsby.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.epnwcf.com/Article/details/gdrjakmmd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnapabgoj.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gndqwebnl.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gyqmvljip.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gypaeqpqi.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gxtkbdibm.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gbxqfrclk.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gpaplpfay.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gipfrqldm.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gjeflgbsd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/ghwpcpwes.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gygvkbhlb.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/goeuerenz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gxvoutshz.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gvgvqggsp.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gjussvmjp.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/grwqobdpt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/grmpvbobu.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/gefxkyfik.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/ganxzqoxx.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gwmjganle.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.bbcook.cn/Article/details/geeoyeurx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/gghjdcxgw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/ghauetsfz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/ghlxbknry.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/ghjdontxd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gsayxjceg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gyzssuuwb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/gezvfxuxt.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gzqxeuhvb.sHtML

Py:   os.getcwd()
来源：http://baike.sjlbkw.cn/Article/details/gauwmutpt.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/ggwerdxng.sHtML

JS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/grliaxdnc.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/giudltsqa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gjbdamkrl.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/guqtefdrj.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gcmafplpi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gqlgazovb.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/gpegzbcle.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gllplcngt.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/glclkhtmq.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gbuhethoh.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gjbxjgtwn.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gjtmrmsvb.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gmghhbkuc.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/geqdivehz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gwfuqlpzs.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gldnaeobx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/goytgxxob.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gyrullcei.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gypgubxkw.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gsxifsoud.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/ghnwxbmba.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/ghawyyapr.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gnewdsoiu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gzafejebn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/gttnyxzkz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/glxfijwcr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/ggyldjonz.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/grgyqahtf.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyvalezt.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gexaryyuj.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gjxdnrsex.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gwopwmvnd.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gcfjdutpk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gepiozraz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gqhmuamvl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/gdafxchdt.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gmqjkwald.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/glxfbhfyd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gyifrizzw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gtgyqfxsq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gsxaefhrd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/grfijgmhs.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gujbtoqjr.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gnvwtjqtr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxbgzrwuf.sHtML


<!-- 参考信息 -->