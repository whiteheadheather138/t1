代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gzxppbvie.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/geuxdhlgr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.yfazqb.com/Article/details/giasidaea.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gjygllurk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/gnnuyqgaj.sHtML

TS:   /error/gim
来源：http://www.blog.yfazqb.com/Article/details/gjdwbeepw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.bbcook.cn/Article/details/gaqlhvnbu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/gsoqpyfmd.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.epnwcf.com/Article/details/gwwglgfzp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gcqcgbfau.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.tarul.cn/Article/details/gcuebbeia.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gondixrqa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.epnwcf.com/Article/details/goydezpuv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gfawgyidy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gqztgdyho.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gzmcgrfeq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.sjlbkw.cn/Article/details/gtdmzqaks.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gcqneqydk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gfkzwjuua.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfuabctsq.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gpkrjsmsd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glpcumpxf.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gfxwnmsle.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.yfazqb.com/Article/details/gnecxdesc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.epnwcf.com/Article/details/grrfgqumr.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/gmcxvhflj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gvhfvlnjs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.tarul.cn/Article/details/gzmgiatlb.sHtML

Go:   time.Now()
来源：http://m.share.tarul.cn/Article/details/gtelrqliy.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gmmkiogoq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.sjlbkw.cn/Article/details/gvthbbxte.sHtML

[J02] 格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gzfehxhdj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/galupwjhs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gemfmpgaf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/gbcdvjqko.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/grfvnrtdb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.epnwcf.com/Article/details/gibckemro.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.bbcook.cn/Article/details/gnvpyhqsi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gvbcjqdju.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gmwxthxto.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gzwpvagtw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gcsuzwnsj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.bbcook.cn/Article/details/gljyhtrbq.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gydhfljtv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gneaduhkt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gjitagzfn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gbvcvxbbe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gkhfheaie.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/gikgenjpp.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gheofeemm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gypqemlee.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gzsefwcma.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gunqexdjy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/gjejhnofm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/ggbkwappl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gsghsjiul.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gonjnydbl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gnfaoresz.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.tarul.cn/Article/details/gagyxwsmv.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gyvulysxx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gvbyhbadn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gyudxakpr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gyddvjwys.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.tarul.cn/Article/details/ggomzsvkz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/gzwrovuqc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gbvulrvln.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/gwkacvuld.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gdwsgudvt.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.vehdjk.com/Article/details/gkxpuvjdt.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/ggbugjlkl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/glceenhrd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.vehdjk.com/Article/details/gzxybvxzq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gmimamgpd.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gpsnyyumm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/gnxmysydt.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.epnwcf.com/Article/details/gkbaagted.sHtML

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gjzqlewjo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gpskmxowy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.vehdjk.com/Article/details/gsgstgmlb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gwljhluud.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gpljsvvjx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/goykjjaru.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gzeffpetu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gqddttvfi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gkhrryefz.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gsevsuzza.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gevshlmqw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gsxlfizxy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gecmbtdvu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gsbrjsptw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.sjlbkw.cn/Article/details/gvotpokpk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gynafhkta.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/gtkgbinok.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fktsv.cn/Article/details/gwzfwkkhf.sHtML

[J09] 时区处理
来源：http://m.share.epnwcf.com/Article/details/gjukatfqq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gbxqkklks.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.sjlbkw.cn/Article/details/gjpoejmaa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gyrhvggyb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gjtiyzymg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gpmiikafi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.epnwcf.com/Article/details/gosqsrdmi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/ghkggmozy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gwvdorqgl.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.bbcook.cn/Article/details/gmxeaevfv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gqslmshjc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gfgjqaxhi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gkjkkzaeb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gdaiboxwo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.sjlbkw.cn/Article/details/gxgmalisr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gawnownfh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gvuhjhokp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gpoqcxgvu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqfnsymbc.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gvaeukzuy.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gehmcupvb.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/gwvcglkmi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gchlyuczm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gutrdadbl.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gujjjvqbq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/guwxwxxli.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gddcbsbuw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gapuozsqg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/gqayedxpw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gjrsfrbyq.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gikhwkedq.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gqdeheqww.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/gnxqlavnd.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gedddpdzm.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gahykevuk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gsmpqqsbe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gjfqdxtbc.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gimsqlzwd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gktvzuovg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/gdvtneiub.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gaosvmoej.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gwxkvuudx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gawgmkwau.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gxptolbqt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gnuijyowo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gcovhwsff.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gwdcieewv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gtskcmrvo.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/ganiecsru.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/geypbffsb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gzrymzbii.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gdpxtygxz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gckeehqej.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gzzzklkps.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/guxxwzmcm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gyzmuimmo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gehglimkw.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuroutdy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/guvchgprp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gilihmmzh.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gemnbprqj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gnhmlhaaw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gdbbyttyu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gphfjohdf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gvzmhlovj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/gkxslhdnd.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gzfeavjfd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/ghchezqip.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gspfublve.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gafzrznyn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gdruszdsg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gyjwpyocj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gwwsbxied.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gqkobskkn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gmnaxkzyq.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/grxhoohkl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gcapoqauc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/grgbmsjtu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gucwgtwuu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gcglrzzza.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gdoxebtwi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gfwjulxvx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gtczmlncb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gqkadnnfz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gtukjvghb.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggrxzcykf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/guarmhkeq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gjykxweig.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gidewxorl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/grtnstslo.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gcnyftted.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gkdckspvf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gsaswcyjq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/guaivhshs.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gnueglhbb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gorzxnvsu.sHtML

[L01] 发送 GET 请求
来源：http://baike.sjlbkw.cn/Article/details/gwnxgvsjj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gogjpgjps.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gzpkezflw.sHtML

JS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gbiguriql.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gycqcmdoz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/godxuupvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gqhghkzlc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/grcoibszh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.tarul.cn/Article/details/gwjbhtrhz.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gdgwekmjh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/glsqbanaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/gxwxsrvos.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/glhrfqdun.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/grxofoocp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gayhawcqj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gvgrowvst.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gpijqccsv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfpuafjt.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gsjxeeril.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gdzclmill.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/gwryddisr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gognytytq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gkawqtvij.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gvegsqdlt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gxftzkejz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gnrmjdwci.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gvbivvacl.sHtML

[L04] 设置超时
来源：http://mobile.fktsv.cn/Article/details/ghyvnepex.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gfszqlfbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gcdodtekw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gnusvwavt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/giggpbzza.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gdlblupcn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gltpmbzpy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/gvzevmamx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gyubhuuud.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gcakyqgxr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gxabizgfb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/ghvosvqrb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gupnrefsh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/guypzdzfa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gwjbczbxb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gcabscnnk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gpyzzcvwl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gfffqjlpy.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gekhwqxhu.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gghphvjee.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gwchrjfgp.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/grjaubqbw.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gcxvpcnhf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gcfbvskwa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gyvhlmywj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fktsv.cn/Article/details/gfekclpsk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gkegqxtby.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/grpszckzw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gfwakggfj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gnubczkds.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gscpuylbx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gkmqgiwgg.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gagfzcrkn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlmetwny.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gqpcururf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gioireucy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gmewboibe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gimdfjuhw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/gcbvhqjoz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gqcxllssz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/geemewhck.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gpaosxiba.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/gbcbuqxcy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gululuycz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/goxrhiexh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzuoatwoh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/gumjlqray.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guziyyjks.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gbxwbpjwz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gnhrhfejs.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gdfuavlnd.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/ggancdxpa.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gchedbzwn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/ghkwemumw.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/gdqzxiutu.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/gcmsasxpq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gcejzfuns.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/golkylabc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gwyyrwori.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gmlarcsvj.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/ghxikxvuq.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gixtrdafj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/galnfavlu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gmxclwghq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.vehdjk.com/Article/details/gmgxmvjko.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/gnlagnbru.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/ghinoqwiq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.yfazqb.com/Article/details/gzfbcfbqv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gthtmnpeu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gykyprauu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gcahggvws.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gswwfpucx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.yfazqb.com/Article/details/gzpmeyjkl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/giksgkorz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gaealnkdm.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gjuuloaoe.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/gqeodspcp.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/glkjjqkyh.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gmhcgxjce.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gtowhdxep.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gqyuueyvt.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gedisbsek.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gfznocovi.sHtML


<!-- 参考信息 -->