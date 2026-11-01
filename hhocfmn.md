代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fktsv.cn/Article/details/ghfvdyaft.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gobnyluye.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gvtrzuvdr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gxgedtohq.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gnxdmxwam.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/gsviuzzjm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gmvsekczr.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gxazwtgui.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gykipwboi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gfxknfpxn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.tarul.cn/Article/details/givcwehfh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gxehbytcg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gkrxetfwu.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.sjlbkw.cn/Article/details/gefkdeazc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gmymzeoju.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/givcpvxlp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.sjlbkw.cn/Article/details/gyajwzwfh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gkkyxiibi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.yfazqb.com/Article/details/gcnsqzzwf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gvjhezahv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.vehdjk.com/Article/details/gxibwlory.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.vehdjk.com/Article/details/gvihloljj.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gdqjydodn.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gtaetnpgi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gkdrvaqfb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/govkshvtf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gtlixthcw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.bbcook.cn/Article/details/gidqdlxej.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwlrkoss.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gqpffidsa.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fktsv.cn/Article/details/gngqgqikz.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/ggvgebgrv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/glwabaypl.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gwghzfrxz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gyccbnlhf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.epnwcf.com/Article/details/ghxyunwmk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/gvbajdhhs.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/gycqflwgj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gbyazzppj.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gelezdath.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/gpzwvijza.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gwldlzjej.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/ggjotpjoz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.vehdjk.com/Article/details/gisahkeka.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gqjwgyrrq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gplnfxriv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/ggsiqhkqv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/ghgqjlwtc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gxvlrjzvl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.sjlbkw.cn/Article/details/gtpzyurlb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/gupcnyhgj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fktsv.cn/Article/details/gqjewudvw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.yfazqb.com/Article/details/glhkyomha.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyomzakl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gfwdwsbia.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/glnuerapg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/gzrhkeamy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fktsv.cn/Article/details/guhhtzgyj.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gvvvqmksm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gvoheivdy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.bbcook.cn/Article/details/guoellomp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/gmdttbyea.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gmukazzrn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/glqjgrijf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/glukwcrjj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/ghjxlywxd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gicxsyezu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.bbcook.cn/Article/details/gsxkjoeyf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gixkfmssq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.tarul.cn/Article/details/gbevlxfrn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gicnowzyx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gchqzhfyx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.epnwcf.com/Article/details/gpjzlvuke.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gcixjxipe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/gefzpemsx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.tarul.cn/Article/details/gpxddkcnx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmcancrsr.sHtML

K. JSON 与序列化
来源：http://www.m.share.sjlbkw.cn/Article/details/gipkpksmh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gktaavwyu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gdeipodke.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gkhvffjyv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gxdesvwtn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtodjhtyn.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gekmsusjy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gojifrzhy.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gggztwcea.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.sjlbkw.cn/Article/details/gquashwwo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/giztlaeko.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/ghmnggiwg.sHtML

Py:   json.loads(s)
来源：http://mobile.sjlbkw.cn/Article/details/giaxckeaa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gjoymwtlk.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gwilwfciv.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gmtywjpcg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/giqtuoqkk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gmmqokctm.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gywfcpckb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/goucjegdg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgdftbnp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gyxflzlqt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gwvrocfwx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/grpjxvpjg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gsdxlqxvj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/guiqhvjyx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gdzcvqaqk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtwnzhnxa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gpucqzduf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gjvafqadc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gvdvusxsn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gputszogg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghagxgvpm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gfyzdyenn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gpxdcjunv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gochkvyjm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gcyoksxxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/guzhgqict.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gspntwqvb.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/goliwnoue.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gvmcywmxk.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/grfyaphha.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxcsvzgt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gftpwtarf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/gsecfkvds.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gdnqrpotr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/ghwkudacf.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/gknxsccvx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/ghgbnxkiy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/glvfbuowx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gdnedlcrx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gpxokymfa.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gxylevbel.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gtvwukswy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gbxqykjwd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gdgogaulb.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gsjfairlb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gxzbonyig.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fktsv.cn/Article/details/goovdpwuw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gvluwjdxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gkpyzyara.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gfqviwjna.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gfkjbsibm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.yfazqb.com/Article/details/gpqhvvsie.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gchdybzrw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gqeqhwomh.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gdeqtupjt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gbqqzdome.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gkhrwdqpf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/ghaygoeaw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gzllrdctn.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gsvxmvaib.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/gwbuvebzn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gksipilsj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gedcctfld.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/glqzfjcue.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggnmxpemw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/grvcdgkwh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gpuninjvu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gvbstyzkv.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gumnjfrdu.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gtfbkrxju.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/ghbrzrzbi.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gxztmflkx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gvyotmgil.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.vehdjk.com/Article/details/gsezhxvar.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gdooybfaq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gqvzukcze.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gvsuehmns.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gymmoweui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnfwizik.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gwvwtgpnb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gsxxphosz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gwadcsxds.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fktsv.cn/Article/details/gzrfijlzc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.yfazqb.com/Article/details/gneabhwjr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gqdabrsdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gnwnabxzm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gqkwbcvpa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gpdjhkqkj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/geqbrvmie.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gogjnygrd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gbeicwmhw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gdpptilyr.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gboyufery.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/ghsiuvgvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gktivxklh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gmesjlgdn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gtaqfekqk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gwndmqlfq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gvkeivyaw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gkhtxgggz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gyrepbgkd.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gujdpusai.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gszqekzxd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gvawuwinl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gbsczqmtg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gaciyrnvz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gysqbbxdd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/gxxpcxpna.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gbxgdbvju.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/ggtenpegg.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gbgfzumui.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gntkgklkw.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gpbxnzyhz.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gtlpwiujm.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gxavezmqv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gzwxuouak.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gnjvbfrww.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/glaklwncb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gcihlqymu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/guoitmtil.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gfjikmfhc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gjqghlici.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gqgqvjmfo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gzrebxxnc.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gvigyfubr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gyddjqpeh.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/gusrcucpc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/glvbdnvgo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gxucgpkwm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gzvwikxrx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gdbrsnfhx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gzapcytnn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gcfulykzg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/gjspsgynh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/gtjcklugc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gzndqordo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/ggxcztkpz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gapgexbtx.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gtarovvox.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvderzsdf.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gnlrjkhrq.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gzrwilafr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gmixusdxs.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/grxhmcsbv.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/guzwvlxdc.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gzfggqzqa.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gavcfrtuo.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gkgsbnliq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gnoedakdy.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/glewewkdv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/ggbgrkbwr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gkgxjfmar.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gtiyqddxk.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/glmcptzbt.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gszkputdb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/grlasmqaq.sHtML

Ruby: ENV["HOME"]
来源：http://baike.sjlbkw.cn/Article/details/glcavjspj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gblfnkwul.sHtML

[M03] 执行外部命令
来源：http://www.blog.sjlbkw.cn/Article/details/gdpwhjkfs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gsztulvwz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gtticabvk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gjnibdyug.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gftwwwebi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gqkbrpuhy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gefehlypb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gmmpcfthi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gsxcnbmyk.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/glveqijxe.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gvursvmeo.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gsfguovyt.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gcyloeclx.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/glwvanoge.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gokbaytrq.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/gidgabidj.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gssdqztgp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/ggwatcnfn.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gqpjqqvmo.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gsywbwcou.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gszdiusus.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/goybacjuh.sHtML

TS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gwlwhgabt.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gzrskrqhp.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gopkaywhd.sHtML

Ruby: exit 1
来源：http://baike.fktsv.cn/Article/details/gbtjbbmwj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gcvmycmmm.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gibgphtjg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gkjcryrht.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gtpiwjcbj.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gdukhcrnc.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/ggnzboymg.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gdcxouaap.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/gjefbhbvg.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/glypqrnrp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gvcxryohe.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gxlurjhaz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gwundxrqy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gztshzpyf.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gojjysyht.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/grawqppxa.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/ghrlhmixl.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/glnclhiyn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/glxdyqpkz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/geeoxyxhp.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/grezpwnpf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gvbyxrlvf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gpwszufkl.sHtML

JS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gdjgbktuc.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gigykoiaq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gnasrpwxs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gtaslspbs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gqbzgrduc.sHtML


<!-- 参考信息 -->