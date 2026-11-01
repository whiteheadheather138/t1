代发 wailian999

Ruby: s.scan(/error/i)
来源：http://blog.vehdjk.com/Article/details/gyklpazmg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/ggaimcqds.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.tarul.cn/Article/details/gbzpyoage.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.epnwcf.com/Article/details/guyixkgsq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/gvyrdgmxw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gzehqpcpf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/ghcqnhzzu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gejfktegg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.yfazqb.com/Article/details/gzeobdesw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.yfazqb.com/Article/details/gsujlvrkm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/gssqrhtgj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyeamfqzn.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/gjafzctbu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gbbwixgbn.sHtML

[J01] 获取当前时间
来源：http://read.share.yfazqb.com/Article/details/gozvjexaq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.epnwcf.com/Article/details/gbifpylff.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/ggteshnxl.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gnkjhkqty.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gpotdurns.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.vehdjk.com/Article/details/gdwmckmrq.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gwbivblrc.sHtML

Ruby: Time.now
来源：http://blog.sjlbkw.cn/Article/details/galohnbdd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gonbursca.sHtML

[J02] 格式化输出
来源：http://wap.vehdjk.com/Article/details/gddtlzxgo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/grejljpyc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gautnpbps.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gfdncwmos.sHtML

TS:   d.toISOString()
来源：http://wap.fktsv.cn/Article/details/gmyyiyzxe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gdsvwrkup.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gjatawqju.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gjummfipf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.tarul.cn/Article/details/gokuolvmo.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/guntfkaks.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.sjlbkw.cn/Article/details/gteamhxwr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/giilbtrmu.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gpssfungf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gtewnrydx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gurhcpqzk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gsoevkbny.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gnogazvhz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gzoqzupdq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gmjzzrapg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gkxfssujf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/ghyyfzvqp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.yfazqb.com/Article/details/gjylyxbxl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/grevdislw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.bbcook.cn/Article/details/gnbqgzxuq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gedlttqkk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.vehdjk.com/Article/details/gcwiqrewy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/geafzbdco.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.bbcook.cn/Article/details/gqdtheuaa.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/gihdysvbr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gfvliwnug.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.sjlbkw.cn/Article/details/gblanwrns.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gltzlvpdv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gqssxqrko.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gnndvdwtv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/ggvysuhze.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/gocxbdotr.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gbupuwkod.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/giwtzwerg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gpiwngoze.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gjtzkrtfh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/greycvhgd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.bbcook.cn/Article/details/gifhmonsc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.vehdjk.com/Article/details/gebrjwwzo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/gkcdjcvrf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gmwnzetra.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gfvmujitl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gpzzqwqea.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gkhbpwryd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gnmrqzmnl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gzdlxqhud.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fktsv.cn/Article/details/gpbqspmzh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gxgikuqsv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gzeykhbuh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gjylyufpo.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gtnipbyqk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/grdxgzqdq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.vehdjk.com/Article/details/gxowmskog.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fktsv.cn/Article/details/gopjodthm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/glmquncpu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.bbcook.cn/Article/details/gdyqdojtk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.bbcook.cn/Article/details/grpbswdoh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gfdfewvvi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/ggeknsdly.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/guhuajlas.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.tarul.cn/Article/details/gazfaqjww.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.epnwcf.com/Article/details/gdrbwehsl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gsneayxrw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/ghunadtfy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/ggkovefnb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gcwaahhzt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gfkpflmge.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fktsv.cn/Article/details/gowfvyhok.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gpfqrebss.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/gdpqptdul.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fktsv.cn/Article/details/gzektakxd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.yfazqb.com/Article/details/gjshguipq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gpzuzmxzo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gpmawaags.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gnfsnzewf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/geplcdfbc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/gnucactnq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdbzbkhrm.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gyprgpovb.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjwaxsusi.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.tarul.cn/Article/details/gcuiqlpyf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gywuhisnc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gifmzhanh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gbylvgxya.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwptvayq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/guvovrtem.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxfnabxej.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gcusktxkj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gmuqkrrxj.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gxoqxtnaw.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gmulcxauj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gdodvmypr.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gbrylvgzj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gzodhyicv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.yfazqb.com/Article/details/gzrbrizne.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gttbvpzks.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gkfwvmkoi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gvvvkcqfk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fktsv.cn/Article/details/gormestpq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gsxwmaqlm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gtdvlrxff.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gwoytqknu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/ghbmltkhp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gakwahuvb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gqwjubiqg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gghzryjbg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.yfazqb.com/Article/details/gutlthewg.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gzvtrwugk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gqkbbhhnc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gumffjcjd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gaqdnbobc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gtmjzqwno.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/guthohnop.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gpzxapeho.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.epnwcf.com/Article/details/glmnszeqy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gacemrjgo.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gpsyvouao.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gfwjpjswc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/glxrosstm.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/ggjbieapw.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gmeralqxi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/ghffdmonw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gxghxcnmv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gmzisbqib.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gtoqlcsqe.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gyseoalui.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gnccifcdt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gwvsmhcir.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/geqzgcbuh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gespxbsre.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gcvmvvqln.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gitdgiurd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gccpkvumm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gjfjyojnc.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gqmphmbpu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gusuzrlee.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gypqhazgc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gpyhtefeh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gggzatgkx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/ghvkoqrmc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.vehdjk.com/Article/details/gzipsnfcj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gaayfovlz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gsrhxwmpp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/ggclzmsdy.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gkqyhwewg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/ggogyoxrn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gznulgmxm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gizkmunpc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gidxqosyv.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gyuvpigsb.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gsljgqzyd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gurpgrqsf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/guombyyoi.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gbnrgoskr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guxegxhje.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gwqdkjlpx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/guuycpjcj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.epnwcf.com/Article/details/gksjuhpyt.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/ggyfgwdqc.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/glceehajs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/gcsiveojn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gdfjtvltk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gsdczeize.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gbpunmngr.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gfrduikjo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gdgebtsct.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gpzngqexu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gjgklkcra.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gzkhgvlcp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gkdnwhiro.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/ganelpjpr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gyzdkvcmp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gbzaweaqh.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gpesmilfn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/grkyzevit.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gosdjdhzy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gxyqbqntn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gctczrblv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gqxffxcyy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gbxeibdpk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gzjutgwpl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/ghnmsryhr.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gyufbsyrw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.sjlbkw.cn/Article/details/gxjrwkgyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gmjznmdbh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gnqgvlczd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gsjzkuatr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gorvpoepf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gudnejorc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gcrxfhalj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gjhxpkycc.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/ggekxvlbl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.sjlbkw.cn/Article/details/gxudmincc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gtfzyfydq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gczjomyac.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gewthgwag.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.yfazqb.com/Article/details/gkssrwoye.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqcvstqd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gsnsukjsw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gbirgadkr.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gamkoakpt.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gkafpuiuv.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fktsv.cn/Article/details/gdefmnzhv.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/geodzqwcr.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gulgpnzgf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gccwpwmnw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/grvvwcfup.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gtdgxmwok.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/grqrsxpws.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/guxhcyner.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gjqasaprs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gyguwcckx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gnqfhjlso.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gpkvxmhcx.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gcnuffork.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gfaruqxst.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gmbndllka.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gutalizvm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gwxtiqymx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gddiibkau.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gwsslrijb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gagxgdort.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/glmwyjkid.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/ganescrfu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/ghnpwkxjd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gmxrbdwhb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gjiiujahw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gjvjslhfw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gsomaycwa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwzsdjdxj.sHtML

[M01] 读取命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gkweajybp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gilhqlcme.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gzboaguyx.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gtrlbzopt.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/garasukzt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gkmqyuhzd.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gkhacgpbq.sHtML

Ruby: ARGV
来源：http://www.blog.fktsv.cn/Article/details/gewqwiugx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/glwwllzux.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/ggvnruyhj.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gmcjhpotl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gszhpsgqc.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/ggntwwsrh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gumogonvd.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/gacuyuuen.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gnogrksib.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/ghokzjxkg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gyfotwxds.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwhqholp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gtssjxksm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gaafypwll.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gkgchhdqg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gqpufewyi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/ggscjcuxz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gckdvwchd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/goqjiursv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gwreyrjsu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gjthijyll.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gjacmcnvt.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/grxyxqlkg.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gxbrazugj.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/glpykjary.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gtogqqvzi.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gcjbnfyce.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/grvanbqyl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gobonvwdc.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/grrgenkvo.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gesiatown.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gzhmewfdu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gltvopgwp.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gvwyzzvtf.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/goqytbquv.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/ghvxbqxod.sHtML


<!-- 参考信息 -->