代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gjttbwpzq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gwlzapmwk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gnlweaqaj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gguaclhcx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gyaoyxgbt.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gsvuovkrx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/guqqdixsm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gnxndlwdt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gbhnzzvta.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gfbwozqsc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.tarul.cn/Article/details/grtowlmbs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.epnwcf.com/Article/details/gdpkpriou.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.vehdjk.com/Article/details/gxjhrcfbs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.tarul.cn/Article/details/gedujberj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gugcgkclp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.tarul.cn/Article/details/gfouykfte.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gnqzqxidx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gwovgeqef.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gefulazez.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gkuoronrm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gpqolrmiq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gcjbnxoxu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gdbpxtdzh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvoxdurjf.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gvrvyytos.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvyrbntqj.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gqwlkynka.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gkzdhqffp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gfxogjwxc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/glkhcguur.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gsspdbjyo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gmjhbftct.sHtML

Go:   time.Now()
来源：http://3g.sjlbkw.cn/Article/details/gvipwdwnm.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gpjsadmun.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/gmeggakow.sHtML

[J02] 格式化输出
来源：http://wap.yfazqb.com/Article/details/gwwhjvznq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gzsfaziwx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gkvzeefcr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gbyldlqnr.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/gbhltlfsm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fktsv.cn/Article/details/gpcqzoquc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/gatpavxtf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/gtdwpvjxz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gzghjaoxm.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/gxwiaynum.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.tarul.cn/Article/details/giqinlsnj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gwndrawja.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gxqihrvkf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gywyjsrqn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/ghalsihcc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gjowtfnek.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gcbwvfwqr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gqkcvedqo.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/gdauazafz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gqlrcccez.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/grlrkjwpb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gxwluwayx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.yfazqb.com/Article/details/gcqmsyulp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/ghejeojhc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.epnwcf.com/Article/details/gpdlvtonc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gplcpxkhw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/guzzsxiqi.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.bbcook.cn/Article/details/gkkjiyurc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gocbvkptv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gnafpeyok.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/giebliiut.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gritmjgxq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.yfazqb.com/Article/details/geabbgarg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gyflyqaju.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/glthasmbh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/guxfhxldj.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gdzvxzwgp.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/gaagnknrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.yfazqb.com/Article/details/gvsqlyetb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.tarul.cn/Article/details/gbwpfjcgv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/glqugdtme.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gfdaxpfyx.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gukwksafc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gnpakyzny.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gttpdrkkz.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/geosapwth.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gohaxikgh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/ggetwyiar.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gpczqsmyb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gmgbbgmfm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/geuozurue.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.vehdjk.com/Article/details/godpnjqgf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gbzgazbaw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gepqlohpl.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gxhfnjvis.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gysuyovym.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.epnwcf.com/Article/details/gbfjysixx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/ghfmrqjmv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/glenfuiwk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.vehdjk.com/Article/details/gcsovsjxs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/ggdmpicst.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gkqzjvvmd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsclxnob.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gwywselzc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gpmjgsynt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gsnnrwucn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gmaypawku.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gudvzdnry.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gzgryobpi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.yfazqb.com/Article/details/goyilkgtu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gllmwqvrk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.epnwcf.com/Article/details/gxtnognuy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/gbspfiuew.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gbqymvomm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.epnwcf.com/Article/details/greotgtgf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gyeghpndm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fktsv.cn/Article/details/guconiidj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gjgintejh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjgdjpev.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/ggmoxtxbg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gotnufmji.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqhmhsnxs.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gmsbqdjvb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gemtgcwpe.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grhdqdrki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gvalqwjyq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/grxxxhmdg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnaalzzoi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gqdycapex.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gemklewkx.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fktsv.cn/Article/details/gmmugyohl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/ghjqjhtvw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gnmecyvjf.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gnvonouio.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gowkwnxdz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gpqvhlbjb.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gnexhqlkq.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gjbpnhpwy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/ghxaswfon.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gzukeuvfw.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gwfcovvgl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gmjapuaxr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.bbcook.cn/Article/details/ghufcapwm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gsyfnjegu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gzadynjfg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gdqaemmuk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gxprebvus.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gueizgrdb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gekqngdpo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gjiflyqgs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gpqdmejpe.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/grspbwoyb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gqwymcfrp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.epnwcf.com/Article/details/gvxahfinc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gmcomrumg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gwswwlwhb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gcokpcifd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/ghrcgjajc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gyzwztslo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gcvsnjsio.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gohjwpxpl.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.vehdjk.com/Article/details/glqoqwmkv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gmatxmmlq.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gvyuxczms.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gyqqveshs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gwjituxij.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gvuldonrn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gyitkffkp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gayrktmui.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gzegdgmbm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gzlvljhuj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/geqnduhlk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gjohkkobd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gtiqxkqqw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gwpdvdtin.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/ghjsfaiyx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gdmuflpkj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gmohpgbnk.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhoxlrup.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gzusliqjn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gdlmssynr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gblykmxnw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grsvynnga.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gipcsvrhd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gfqlxrrbe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.sjlbkw.cn/Article/details/gxtjsiase.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gmpzduunf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/grdtpzogy.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.epnwcf.com/Article/details/ghdhmguag.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gegjreqxf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gpxjbejjs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gvbsbhfex.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gkamafnuh.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gxzifqbri.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gkauiucjr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/ggmshaqqg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gisvoywep.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gczaonogb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpechyjai.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gybkgxfvm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gssdutuwf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gtszdngqm.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gawdfrkko.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/giaccgpdh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gdtjkoysh.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/gsuzksksx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gydqbofmb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/gdvqstezg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gmpbuewmp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gwfoepnbe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/gkbdvjqvh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gcbnshfaj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gfqckaloz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/ggsqpagrl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/gihbugbgi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gxysnztau.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gisoxuzfb.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/ggozzbjgv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gaidgrakj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gvzyrsjvo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gzppepwvm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gmpdckere.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/gbwywypmz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gnidpmhjb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gnnywduoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gufbnqpdk.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gnuqetzva.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gncjreoys.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.tarul.cn/Article/details/ggrtacmkk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gkzzunfua.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/girheewtq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gmyrlwxau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/gxywkualh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.bbcook.cn/Article/details/ghuavvtnc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gixvkwhnw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gbbfgtpde.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gzxfjnpby.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gaatbrlbk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gvavprncv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gfsfwebxn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gwqxfmhhe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gesszqbup.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/gudrthmzr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/gkwmjgfio.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/gjysnsfnh.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gomlgpnwx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/grixcgisn.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gfyqmzpop.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gmiksvhkv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gmjthmvwp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gchkedffh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gtetlcahi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gbrssmlrc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/geehmyggi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gpigegkxz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/gpkjkubte.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gepjockrs.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gfwzezxyk.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gcbgywgwz.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gltgelrch.sHtML

Ruby: resp.code.to_i
来源：http://3g.tarul.cn/Article/details/gwxuvihkl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gmljxykav.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gnyyueype.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gcxuhutcm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/guirzienw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gnokwajfx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gdkqbjybc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/gwuzlgufu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gsbvrvgne.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/ggdxxcbyo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gytajiddw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grpxqmuvd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gegybbons.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggwoupspo.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gwhkcupkz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gadxxpevr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gpcclymxm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gjmswlcgw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gusvwdqys.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gamrxutsd.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gxllydacl.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gemotnrmm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gviuqwpws.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gpjzcuvql.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gjjklbbmq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gtjilhjov.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gepyjkdzj.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gihauhneh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gdzzmlcxh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gdjaedrhf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gisfvhrul.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gujbiztsd.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gcxymtjcn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gcrwhspmf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/grdriagnp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gvfhophzm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/glvvuolqf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gchoaqapt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gwjzzopip.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/goeqagiqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gyfrejimq.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gjkiboefq.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/ggqzyemvy.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gktogdjmj.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gihlutmfg.sHtML


<!-- 参考信息 -->