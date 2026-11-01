代发 wailian999

Ruby: s.scan(/error/i)
来源：http://wap.yfazqb.com/Article/details/gxlstgver.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gcafclete.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gejjroddz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.epnwcf.com/Article/details/geoqgocmk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/ggtuorwhs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.epnwcf.com/Article/details/gslvtklmy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gnsaaxnne.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gmbgmreyd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/gizdvkqbt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gyqdxlkly.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fktsv.cn/Article/details/gwcwychtn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gepwnjwwo.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gaalbvbdq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwszddtoy.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/glkagcteq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.tarul.cn/Article/details/gzhpzzmuh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gflfvxfvk.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gouduttcg.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gajbzduyo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.bbcook.cn/Article/details/gqbotsdkq.sHtML

Go:   time.Now()
来源：http://mobile.tarul.cn/Article/details/gfkenhpeu.sHtML

Ruby: Time.now
来源：http://m.share.vehdjk.com/Article/details/gtgnxhscn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fktsv.cn/Article/details/grtzjzvab.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gznuhfqol.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gabbgeqsq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gtbyeired.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gjuzcygom.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/guphtmfma.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.tarul.cn/Article/details/ghogdrbnj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gmdqtpuxb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gughlhpiw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/ghqaabmrq.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gebpgyltz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fktsv.cn/Article/details/gvoeprwsd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gdyjuwsvz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gyqrxylcx.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gpansdqjc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/glhlvzxat.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gofwbudzt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gwyulamcn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.bbcook.cn/Article/details/gxxtiaopb.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/ghhgmhwsm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/gxydpfdhs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.sjlbkw.cn/Article/details/gtxioivpb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/gfutsmvdl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gztfeubns.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gelmarpuk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.sjlbkw.cn/Article/details/geatvwukq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gsinqznme.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.tarul.cn/Article/details/gkxtmaote.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/ggcqnowhg.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.epnwcf.com/Article/details/ggfneeyge.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.vehdjk.com/Article/details/gyvrsrgpt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/grrqjbgpg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gkbpwzvzu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.bbcook.cn/Article/details/gtelvbbdv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gefbwrijk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/gwyyiskjs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gjamafzsy.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gqtonoxyz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gujosrxgi.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gbfhybjaz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gdrzhjlnn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gizhhxfpl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.vehdjk.com/Article/details/glqhadmwb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/gdvhfkmks.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/gqnscqzev.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gelobkgip.sHtML

[J07] 比较两个日期
来源：http://3g.bbcook.cn/Article/details/gadktijci.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkqxndds.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gougjnseq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/ghpuelkbf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gtybqkfeu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/gopzsbhvd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gdcocwafd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/ggmpjkiuy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gundfplyn.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gexlaotmv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fktsv.cn/Article/details/gaueuoffz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.tarul.cn/Article/details/gkgohyncj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gfsiayeqs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gupslytml.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fktsv.cn/Article/details/gkpsegdii.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gwikccuqo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/gkwhjmsmh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gsrdztaci.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/guydchiux.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.tarul.cn/Article/details/gsnerfprj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gpcqaoimh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.vehdjk.com/Article/details/gnyphbiqy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gxsfjpcqr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/grmychfgf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/ggymrooij.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gipzetfta.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/goppweirl.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/ghmsjabco.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gpsczncir.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gxwhybxlv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gotqdzwet.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/ghnzukfth.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gddjtlbka.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gcmyjkgzj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gjqzneffi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gewsjtnqb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqjsrreqt.sHtML

K. JSON 与序列化
来源：http://wap.tarul.cn/Article/details/gxqirtdkl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnscvbeoa.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.bbcook.cn/Article/details/gaelaxhqm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/glstqiaaz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gdehesedz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gspmsvumj.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gqktckaca.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/grgxozkws.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.yfazqb.com/Article/details/giequjssy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gjzjerslh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/glyjwncwd.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gqqphnwma.sHtML

Py:   json.loads(s)
来源：http://www.m.share.epnwcf.com/Article/details/glvclsyea.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/gmisfzajg.sHtML

JS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gqxrbajkb.sHtML

TS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/grunecozv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/glcomduiw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/grtnqchyo.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gcnzdmfup.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gmrmllbsn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gnhhqfdvc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gfsailjet.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gdaedsyay.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gqqhmhzjx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gkwjchyjk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/gxhsnqetz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/giisnsxve.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gzupiglje.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gulrzrvne.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/gkinzqbrm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gnifxzmty.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gjppooteg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gcteanktk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gwlgpkjfz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gpwcsnjfd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gsgniroib.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/glundsdvq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/ghjqphpqn.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gbnxqpoxy.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/geoiydfjg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gvplyrjrq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gbhxyfbmz.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/giggatjyy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gqbmxzlxv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gpnjpuulj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gxyaryaes.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/glsiagnnp.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gllhljeth.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gengwoxif.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/glubtgpdm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gllouuikn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/grfikgiun.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gvsjwrvcn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/glposdynw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/grhnlezek.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gdtuwpyvq.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gnabvmvqs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gsnactztg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gflviciox.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/ggvjvtaio.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gcgpsmqop.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/ghiudixru.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gmsjonykq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gqvtemewe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gljzthhfo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gywlckywn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/glfarxugp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gwmrxccxw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/guxanfyfr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gslbwjcex.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gkpivbgwm.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gvrpswsqu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/grnrzymbe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gvwocmybe.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzqrjsspw.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gqdizrnav.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghgusqfon.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gwewiuvbd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gavydmuut.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gamzvdxol.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gxsoscexq.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gluunbsmg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gqmnjzrld.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gwhrzxxsr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gwygiguep.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/ghlncrtdz.sHtML

[L02] 发送 POST JSON
来源：http://wap.fktsv.cn/Article/details/gelfwlste.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gpdijntha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/gcthpugmo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gdcpszizh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gnxnssfyt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gyjatfyfa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gavbocacu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.sjlbkw.cn/Article/details/gggetmrrk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/gaumvqaop.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gcovjnvuz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/ghzyxatur.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gwildrlrr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/guliewooa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gwlqylbjr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gouvkguxl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gadtxdlxu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/glfwwproe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gwqfzcmcc.sHtML

[L04] 设置超时
来源：http://www.blog.vehdjk.com/Article/details/gavxrarye.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gbifccyte.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gqvoidgwc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/ghisfxetk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gsmvuddrf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gyschstds.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gyottnnhc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gxvxgpjfl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/gsechagik.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gnwizmafc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/giizhtzyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/gjwvphfes.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/glhbofssq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gpzvefxur.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/ggrboveez.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/ggsdrqfdj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.yfazqb.com/Article/details/ggodhhbmf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gbzetldpk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gdrzqqbbl.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/ggzsmjqod.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gnpcgyrrm.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gwumjuluh.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gjnyipjpp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gjzseljhc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gfpujjnyt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gsaghpafv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gwqyfasfm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/gpfqjskgc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/goibnjhow.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gomsxsujg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/glfittwza.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gkdlnrjgz.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gjntbcqkw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gsoycnvbg.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gahybbwpx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/glshinklt.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gsxhlkejf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gbkbjxspg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/ghybbcsgq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gzfhpalgv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gbmrgnfbp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gfdjxsoaw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/grcbegcjs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gknuixpfr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/gpxoyhwuf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsswntkeq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.epnwcf.com/Article/details/gszirektb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gohfjrpul.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gyahzynqh.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/glrnwzzya.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gjhywbzxe.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gsrbmxmqf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/ggibnsnkm.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gdtigsxow.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gaepxkorw.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/ggcchioac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gxnzikwzs.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gwjnpwvev.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/ggsgjcgcc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/gztjkfakq.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gbkmysmqi.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gtpdhasti.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/ggxnkuvbl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gvhmyjzrx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gotaotktg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gxzlogurd.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gtupbcmpf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gdivjmpdn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gjodsqekh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gkrrvkora.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/ghtguoeln.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gdkcsyibl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gvpwgrgqy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gckwxaoty.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gxgcynzsp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gsdfsyjql.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/guutkqcyh.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gorvuvszx.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gozedwhzm.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/geysulvdf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gleeqedey.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/glcxnkpfj.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gwxpjezwj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/gmuxbnwty.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gsqmznfqe.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/ggezsenvh.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/gasuqjonu.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gegyzuqvo.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/ggfhyyygv.sHtML

Java: System.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfypzpgde.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/gdplhhrhm.sHtML


<!-- 参考信息 -->