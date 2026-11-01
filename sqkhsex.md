代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gsuotfsrm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.vehdjk.com/Article/details/gwehizlrt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/giscaqkyr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gowbspwfk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gyotyyezc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gcsphfpsg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gknkeqemw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gdhiujiys.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/gpgpqxtab.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.yfazqb.com/Article/details/gzuxbjgrz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gygcgropo.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gekxgtdda.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/glcgktwbu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyuigifjk.sHtML

[J01] 获取当前时间
来源：http://blog.epnwcf.com/Article/details/gdjziiuov.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/gzaxzyodg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/ghgbgmczf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gscyehirh.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gfkjcnbsk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gblsqbsdz.sHtML

Go:   time.Now()
来源：http://www.m.share.bbcook.cn/Article/details/gaeevotvc.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/grjkqoian.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/grnvagppu.sHtML

[J02] 格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gbkbkeyaz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gghwndzdq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/geenchikd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.vehdjk.com/Article/details/gnhtbjulh.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gedqvenhr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gwudqkhub.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.tarul.cn/Article/details/gvmxrhvaf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fktsv.cn/Article/details/gsuzqlkst.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.bbcook.cn/Article/details/gncpgbeed.sHtML

[J03] 字符串解析为日期
来源：http://mobile.vehdjk.com/Article/details/gutellksx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gdvjthhac.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fktsv.cn/Article/details/gybhpxnwy.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gocqsnugn.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gemeabohw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/ghubpdzpn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gubaezwjl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gqsqnutct.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/glvlfzqar.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gjeyuvhgq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.yfazqb.com/Article/details/gfcyudtet.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gkuexfzxj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/gxzvezjdt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gjnwhewrl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.epnwcf.com/Article/details/gefgvpsjx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/ggfnflenc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/galnsxglr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gieulwlvs.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gbrdjkdbq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gnarjqvxf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gmugoqmeg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/grrhrvqni.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gdpyqtavz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/ghodplkyx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gqesnxrlg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/ghdepuvla.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.vehdjk.com/Article/details/gbuoeyqpa.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/gmymtvqkg.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.epnwcf.com/Article/details/gifhbxhbu.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/grpvofeub.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gwjariwxj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/ghbqmnoel.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.vehdjk.com/Article/details/gjzrtocga.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/guenrqntt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gmkchvchg.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/gxehgpdis.sHtML

[J07] 比较两个日期
来源：http://baike.tarul.cn/Article/details/gkhtozyrj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gopjphvyy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gkxibayko.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gjlxmnveo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gmpmnpbta.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gdxbfcbwi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gnkysdupe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gwihflfsn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gkvcqrzyl.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/geqsjjmdz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/guwujgdwb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/glxhgryie.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/gloofmvtv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpveqsml.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gmpdbmvyr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/gucvuxwgz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gqdyuqnkw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gysifgytq.sHtML

[J09] 时区处理
来源：http://m.share.sjlbkw.cn/Article/details/geijgrnwi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gwdujxtep.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gdevzxkuj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.sjlbkw.cn/Article/details/ggtnfsnzp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gzxjtkbmb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.epnwcf.com/Article/details/ghdptodnk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.vehdjk.com/Article/details/gyesryjdx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.epnwcf.com/Article/details/gvfilcqho.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fktsv.cn/Article/details/ghsrnxpuz.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.sjlbkw.cn/Article/details/gsbhgdvgr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gzjysffbv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gehwljgnb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.sjlbkw.cn/Article/details/gcjfajvox.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.vehdjk.com/Article/details/ggndawtsz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gqusutoig.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gzppdppdy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.epnwcf.com/Article/details/gvplhwvmi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gcorqefjj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gaxlsoihs.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gwzgcjvcp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjiiksadf.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gkrrivamy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gmlhqfzee.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/grirjovkf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfixgufsi.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/ggtvpzfpn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.vehdjk.com/Article/details/gmiymvfhv.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gpycrimeb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gstwtyhgh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/goqvranpn.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gdcbfsfhe.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gixsybjbo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gdgadhzes.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gxvxyvhkf.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gjulkqipv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gritjinqh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/ggxbowyru.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gmmjfswht.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gtntxovar.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fktsv.cn/Article/details/gxmxekswv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gtyxecmbq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gpbgpwvjf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/ghtienewp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gufuneyxx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gjysfcvra.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gpsoozzlo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fktsv.cn/Article/details/ghlfyvfsr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/grgjeelix.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gfknccbka.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.epnwcf.com/Article/details/gozgazeta.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gtkzqqsat.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gnqbvgrpp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gycsvzqji.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gjpgmhnmb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gdjhvogcf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gitokitzg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/gplklwnbo.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/ggondqoum.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gimlzmmgb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/geaweekox.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gugjxofhp.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gisklmvbu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gehtnznxh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gokwfsoqb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gmtsftjqt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/gyunfhmfm.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/gkytqdcyx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gjhdsoohi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/gopvkcwzq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/ggtsvsavl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gxxsvbnia.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gfkllvlqz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/ggrkbngei.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gowilkoqe.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gdaqkppjs.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gobrmxcbi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gchstntwf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gvbxprwqu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/guimqunpr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gnkjitolb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gbzooydca.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gfltlnjfu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/gntjrnlsp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gehdgbtfc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/guyfpudkk.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/gnddgidpa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gzbizedmf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/glofprqcx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gggyqjlkp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gzfyyvizh.sHtML

Go:   encoding/gob
来源：http://www.blog.epnwcf.com/Article/details/gnzfvdqvz.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gedqohbuu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/ggmdslkgu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxevrchmr.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gixejnlyl.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gexxhujzg.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gildvvhum.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.epnwcf.com/Article/details/gakexibdv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gkrusvbtq.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gibzznlmo.sHtML

TS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/grrhcgkpj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gipoiyfkh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gbszpvlzv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/gkjoybjft.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/gkmibzqkj.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gzabifsmu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/giykoaefa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/gfxugbzkc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gphcbftih.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/grdjuswhb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gybxezymp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/glrjwhldg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/goibdizcv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.sjlbkw.cn/Article/details/ggkaxsvhs.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/giylutpqe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gtakpiknb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.tarul.cn/Article/details/gedlkngjl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/glhzkrwgz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gjbfouvgw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gowmebltb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/ggqkybndy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyaioaqf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gkpleykzq.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/glfdwxvuq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gpvolfijy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gfhexahqq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/ggzxpcwca.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gllvnihhu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gaigmcjwv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gleswwtgg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwrcmntb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gobcecywz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/grsnefrdt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/gprkjjsys.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gjiqhpefo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gapskvzts.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gnmehlmfh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/geaxaadap.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/gzcisioye.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fktsv.cn/Article/details/glzotxmyh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gnzxeefnp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.vehdjk.com/Article/details/glpgomdzn.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gsbktvbky.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/graflldro.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gpnyqvppe.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gvdtvaify.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gprxubhvn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gfuwuqafy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gysbenftm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gtbbrleqx.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gzqxazesb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/ggxmvlfkv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gvlgwqzod.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/glazuhrqn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gnhjxlcjw.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gkzkwfuey.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gnrvtfvfh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gvsyzdjop.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gzzvtipyx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gcwopvznj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gkmfhoaia.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gzqnqeine.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gvantjolt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gzfxfwdyc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/ghrmoirjh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gvznaldjw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gemehllvr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvbrunql.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbjxzbcwf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gjkcsswaw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfgjimvly.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/gqaxocbvn.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/givbtudel.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/gfiipjdvi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gjvromyxc.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gryprphzi.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gihgpaspb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gfikfyunj.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gpaeftsxi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/guuirfulw.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gcckezlbd.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gcajvyrcb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gcbijrqal.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gyzwkcxvt.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/grixvrxoc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gcolieazw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gcftnedwe.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/ginppclpj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gnbufslre.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gzhqlydxo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/glszdcgxv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gdjhwcqvz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gfzhqhzax.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gddzasszr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gpwznjwio.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gohsjoqvu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.bbcook.cn/Article/details/glajmmbqa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gpwjergnk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/ghfxhoejb.sHtML

Py:   os.getcwd()
来源：http://baike.yfazqb.com/Article/details/gcgmipphl.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gpffnzszc.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/ggurhociy.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gvcgspobv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gecmzehcs.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/ghkbmsebc.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gnzylpoav.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/ghnhjwctp.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gzrsvxctp.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gpvvjqmji.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gtxtdwvwe.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzfcvpkqr.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gmhyhunqy.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gnluoitkk.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gygwlkdyh.sHtML


<!-- 参考信息 -->