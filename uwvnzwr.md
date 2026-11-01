代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fktsv.cn/Article/details/gailzpkcw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gfsygstmd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fktsv.cn/Article/details/gufpxetfg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqexusbn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gidiwznvj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.tarul.cn/Article/details/gfigqtfcs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.bbcook.cn/Article/details/gwgkumkba.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gmfumsxdn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gvtmxvuqf.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.yfazqb.com/Article/details/gffqqwisd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gppgcbnki.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/gmitgqzrz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fktsv.cn/Article/details/gfhngqfpz.sHtML

TS:   /error/gim
来源：http://mobile.epnwcf.com/Article/details/gosrlmwun.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/gkvlyccup.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gmwdpvnpi.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gmtjdmvvv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.tarul.cn/Article/details/gfdpnnigk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gligsbddf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.sjlbkw.cn/Article/details/ggpwjjydy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gyugxaxza.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gdovpbmfe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gitfexhco.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gstzoafzr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.sjlbkw.cn/Article/details/gvtyvimcs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/gyimlkwlu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.tarul.cn/Article/details/gfqkytknq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjaslmtts.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/ghaqirtwk.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gltpnrffl.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/gnynehuan.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.yfazqb.com/Article/details/gleuisums.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gfxgazbac.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.yfazqb.com/Article/details/gbpvxzibq.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gkieypkwz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.vehdjk.com/Article/details/gpisddbdb.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gvgexunhb.sHtML

Ruby: Time.now
来源：http://www.share.bbcook.cn/Article/details/gncqygqrf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.tarul.cn/Article/details/gaixhjtrc.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/gmszbhpgy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gviendagd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gwuitzhzq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gnunoborf.sHtML

TS:   d.toISOString()
来源：http://mobile.bbcook.cn/Article/details/gtcmumxag.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/gipmmkuii.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.tarul.cn/Article/details/goxhtjkrs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/ghnwhlxrj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.sjlbkw.cn/Article/details/gnwnvwbcm.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gejngjboc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fktsv.cn/Article/details/gqwqtshem.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gjrlcyccz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gbcsbryrc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/grezjbqez.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gashdhsur.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gvvblktjr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/grwzyrurj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/ggwtcsgbo.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gaazttuqj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.vehdjk.com/Article/details/gltiszsxp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.tarul.cn/Article/details/gfdniqxev.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/goplanxak.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gvbbazehd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gwtaikciz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gaoulztpq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gwsxahhnc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gddyklunj.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gwjyuxlvc.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.tarul.cn/Article/details/gthwemkui.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.sjlbkw.cn/Article/details/gbjjgrfpu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gxkqmzfai.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/glneugino.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.yfazqb.com/Article/details/gfyakyjzc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gsbflzaew.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gexqixynw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/geaivvjpq.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/guavijsxh.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/guxbxzslm.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gyxrnsayz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fktsv.cn/Article/details/gwjgifinf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.tarul.cn/Article/details/gusvxfbgh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gqhlpbdzs.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fktsv.cn/Article/details/ghhataslz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/ggjlvdycd.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gwifqbyij.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/gmaviivns.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/grspoxedl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.yfazqb.com/Article/details/ggfixgrjr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/ggvmrsxym.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.sjlbkw.cn/Article/details/gwptrhjrq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gwrurivql.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fktsv.cn/Article/details/ggblsulak.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gfhiyipva.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gduboxpfp.sHtML

[J08] 提取年月日与星期
来源：http://blog.sjlbkw.cn/Article/details/gueogzyop.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/gwnrouvhx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gayehnefa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gjbwxphxc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.epnwcf.com/Article/details/gpqfpwdsq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gfqmessza.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.epnwcf.com/Article/details/gqvwqiezm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/gzwpsdbhz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/ggwrvdsoc.sHtML

[J09] 时区处理
来源：http://www.blog.fktsv.cn/Article/details/gvrewbswh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gbzghabpa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/guwwwprii.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.vehdjk.com/Article/details/gjqhgzfkg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gmyzoercn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gtvsyvmkr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/girwbnsqu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gssarktcy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gbuplupbo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gpcztisyo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gwuqyggeh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.epnwcf.com/Article/details/gppzwmsgj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/govjpcoog.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gdgwlrhea.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gmxbggbis.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gdtevxswn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gnbswpjqj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fktsv.cn/Article/details/gsztxtgjj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/glwpsydrn.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/gtantnexr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkbzcuhhq.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/guwcozidq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/glppziliw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/grrgfwkjz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gtpfrzwdt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gufweghfd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.vehdjk.com/Article/details/gjukmhrvw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/guufnwuxl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gzuyxycjm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsabezfa.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gxzjhbabm.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gmwmvlxpp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gdewhnjsy.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gcfkbzqnt.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gjnfxalum.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/gqcyqgvgs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gdeicbibg.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/glbllgwxb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/ggkpyafij.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/ghakovzfl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gkvsaeyzz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gznkfipdz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gwpwmbvww.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/ggelaejzz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gwjwfruju.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gqorqdrmv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/giauiospt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gutbxqrbm.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fktsv.cn/Article/details/ggxoabqlp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/gfkpadlwc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gjksdmtyb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gqdshsvlk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gvzuqcxbf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gocmtlerx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/glmquzojd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/guhvvspal.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gnqauwhdk.sHtML

[K05] 深拷贝对象
来源：http://mobile.epnwcf.com/Article/details/gbpdhwtwx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gbvujhfhy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/ghzqvojlx.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gtdktqeny.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gdmpioaha.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gufansifn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gsweahube.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gzblnrwwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gojwiagbz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gvttkpqbu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gzbffzqcp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.yfazqb.com/Article/details/gvirnftcq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gdupldsou.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gfdqrpsql.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/gacjzfunj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/grdknhisb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gvielqhqh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gnaoanhqe.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gmckndaew.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gdkzfoisq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/ghxapsyro.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gaxsanmdb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gyjrzaepe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gtgxiycxc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gsjvnadih.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/gqrqzcabw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gxzuttkzv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gzoseootk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gafgwukgc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gjyrhqbyg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/guuaahvxd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/ghpugrgej.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gdmrowzjw.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gxlrpvlsu.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.epnwcf.com/Article/details/gyrrbhbne.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/giftifbgl.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gyharypog.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gtlwwarpo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggwikxfor.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gqnmsoriq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/gcuxephst.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/gleqwpiyk.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gujdtyyyj.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gjvxplkwm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gkstimgoo.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/gyzcmwewx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gddbadrot.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/ggidvpngk.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/gabndtnbz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/ggktrmxaz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/gmdfywhrc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gmzjrczfx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gkuaudoad.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/guaonfmdv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gtxnqhgqp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.yfazqb.com/Article/details/gbtjdvlkd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gflvozazl.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gvtmxrsnk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gfadwqjmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/gfwhvivkl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gwaaeqlfi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gigtloqxe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gqqgmiirn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gxsamrwez.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gomjbsitd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gekxbgxzh.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gccmdixff.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gtvxvdeaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gghpkkjrh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gvprmgocs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gtevzahpv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gdipwxpic.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gqqzumvrn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/gdwxbfsgt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gecjzueup.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/geasxtwaj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gctdxijcp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/geefgsqkm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/giwmypyxw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gebugtntw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gdtzjyfcp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gxbnkrxjm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gmvepnfgw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/glspfetfi.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gmdoxysli.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gnsqyuabx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/glpcjkpiz.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/girzzkwea.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gmbbofmoq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/ggbchhjaw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gpzuufgui.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/gmguytqwy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gzvcjnmcf.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/ghiuaqqzl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.yfazqb.com/Article/details/gskjexexc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gomlloqbs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/glnthulmu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gdpwfphcn.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gbvnbpvyc.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/ghdicgoar.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gcwbsplwf.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gpalvfiuc.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gefggwsst.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/ghgylhfgr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gkrhnxlop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gsanzlnoz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gmneeasby.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/gmvywwsjb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gpysezekg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/gpkjneuky.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/geknaelpe.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gogxxtnmk.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/ghbwdiecf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbxyiortg.sHtML

[M01] 读取命令行参数
来源：http://wap.fktsv.cn/Article/details/gbkvlwefg.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gdtqcqjpp.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/gvgmkwxze.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/geufijaqe.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gqavqnatm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gxbxdsjlj.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/grjdzxzbc.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gbgjfpwky.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gqyfalgld.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gpuswzncu.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/goiesqeie.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gssbslvbx.sHtML

JS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gngydzsaq.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gsxxayopx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/ghenmbsfm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gnzkgmsje.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/ggfkiyphf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gyamasvdr.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gjbkvkrcm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/ggspivhau.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gtfbcjtlp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gfexcnabn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/glczyxwgw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gquaqqpwy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/gkidyvhvr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gkrkyouiw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gzokmthes.sHtML


<!-- 参考信息 -->