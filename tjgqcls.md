代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gnxkgqjqv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.vehdjk.com/Article/details/gwschdatp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.bbcook.cn/Article/details/gxhoefpdv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gvfjksnmr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/ginuuauqh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/galpwxsys.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gnqjcshil.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.tarul.cn/Article/details/ggfykbjgc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.sjlbkw.cn/Article/details/guhiuodlw.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/gexduyhke.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.tarul.cn/Article/details/gaiuzqmcn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/grbmbgluw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fktsv.cn/Article/details/gxmwzfmhs.sHtML

TS:   /error/gim
来源：http://3g.yfazqb.com/Article/details/gemmbwipz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gtxsjamei.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.yfazqb.com/Article/details/gpiqsxuaw.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.bbcook.cn/Article/details/gufzogrlj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.vehdjk.com/Article/details/gnniukrpc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gazsuclvg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/gjeqssxvq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gukiwzimp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.sjlbkw.cn/Article/details/gnegbczkz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gzqpyyscn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.yfazqb.com/Article/details/gborhanfr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/gqgxhknvr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fktsv.cn/Article/details/ghyxhlkzm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.vehdjk.com/Article/details/gvikjedol.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvuuyxbgh.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/ghxhkpfcu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gecfyqodc.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gatgamesu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/gbwnwliha.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gsgxuqnnr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/gtihlwhuq.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gxivhjzjr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gmrkcvvdo.sHtML

Go:   time.Now()
来源：http://blog.vehdjk.com/Article/details/gkwbujtgq.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/guzgtrrzw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.epnwcf.com/Article/details/gbopuwtkm.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gikdyynmx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/geezqxihr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/ghrwegbwb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gsphxfcmr.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gsmqyrobe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.bbcook.cn/Article/details/ghbbedpeg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/gyigqqtko.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/grbaayxam.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gztwxmsda.sHtML

[J03] 字符串解析为日期
来源：http://www.share.bbcook.cn/Article/details/gmkbfbbep.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.epnwcf.com/Article/details/ginbhwwub.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fktsv.cn/Article/details/guviruxoz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/ghnnhffwl.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gnadgqrqm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gcohnoune.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gegazfxgg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gltmjhyce.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/ghnuevbod.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/gpobsladl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/gcnxxgvbs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gbuoducrl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/giltbzbah.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.epnwcf.com/Article/details/gmhaypjjm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gwjqriiwc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.epnwcf.com/Article/details/gwbpyljst.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gytrakdki.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/giylgeeqi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gikxwetso.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/gziqjnrui.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/ghgmxmqel.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gapltcfsw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gnmzjullg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gkvrvzdol.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gezjezdah.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gttapaogt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/ghgidynvq.sHtML

[J06] 计算两时间之差
来源：http://3g.tarul.cn/Article/details/gfxmrgswo.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/gspcdfffh.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.sjlbkw.cn/Article/details/goxoogwrb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/glyakrbab.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.epnwcf.com/Article/details/gmapcoaft.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.bbcook.cn/Article/details/gwwfmgguj.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.tarul.cn/Article/details/gfpsxhvgb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/gnukexcgg.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gvoyumesk.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/guseaoozb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gtffbqndt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gulxagrhd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gkoygimkk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gaualdnvd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/gazaneyzi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gfvbkgchy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gvzbyeded.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/ghoagniry.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gmrtctada.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/gtnybsjtv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gzixvnjjt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.sjlbkw.cn/Article/details/gefuuawfk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/ggrtsinob.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gsojyuiqd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.epnwcf.com/Article/details/gxvznlxxz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.yfazqb.com/Article/details/gehtrxqve.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.tarul.cn/Article/details/gghtepwvm.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/ggmrkkklz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gpldyrtcv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.vehdjk.com/Article/details/gbvmlvgjq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gjnyzesvy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gzmqzifpd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gupszhxug.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/gkbhkvwhp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gojqqbibm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gclmfvcxz.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gddrogprr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.epnwcf.com/Article/details/gogmfxuxw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gcprdlaix.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtsgrqdw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/glljwtdou.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/grfuxsske.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gacrdkdps.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gaxmwnnsl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gqogjstgx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gexjzgode.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/grawfxaba.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzhwgpgot.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gzgudnjto.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gplghfheo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gokrjruuh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gdxialnxp.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/grghiatxa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gasqblsol.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gbiygdenq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gusxqxbii.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gadfbavjw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gewrzkozs.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gtlrdgcfy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/gatmtmllh.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gollvbdyx.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gwqvgydvp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/gskxgscbu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gwjzmbzwx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gavtdrupu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.tarul.cn/Article/details/gigvmptos.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gjqrubfhb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gadnwlgks.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gzsntkxjf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gyjnfnuuq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/glubqnvgo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gsmkcyxsf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gdywllvzu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/ghkmejali.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.tarul.cn/Article/details/gpmvuhtkb.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gdpujhjch.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxdfmzlb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/grvvdltoh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gmzjazrsn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gyoiintau.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gfsfxrvvw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfwbfqgy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gcsvdanoe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/golttniyh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/ghezrqmyl.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/getflcxqv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gtrrohoyi.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gcjulpzno.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gsciqbyzc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gpllwxapn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gqbdeshce.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/gihaiibxt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gkbuqdtso.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/glthficnd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gqgmfoaok.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gjdeiinde.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gkgzplfog.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/guuozmmdm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gudhuzeod.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gvzhubejy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gcsnxmjtz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gohtvhqdb.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gjgigrlfn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gwtumhanb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gawnbewqw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/ghcxvmjrc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gbcsjfpzu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gsorswixu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gnvguxgrw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gxkgfbjpt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gsyghculk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/ghpgbzfnw.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gvakcppio.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/ggrcxuynk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gcpneeyvc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gzgciljjv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gdqofcscy.sHtML

Go:   encoding/gob
来源：http://www.blog.epnwcf.com/Article/details/gwjcguyfg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/ghxdxmkht.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gpzibphnw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gifumzmrm.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gjhzwsrbj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gefsbgfdr.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gkvgeqzmg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gmbbwyuaj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/goqcwvngl.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/ggegzxgtd.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/geukodcvv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gqkaujdyl.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gbayltnbo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/gpcitwnaa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/gxcgfadwi.sHtML

[L02] 发送 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gswpjyqgx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/ghhgsxlme.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.epnwcf.com/Article/details/grgyokdyk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gzwokhrji.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gbncyeqry.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gqwgzcgcz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/glgeqfypm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gxsktpweu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fktsv.cn/Article/details/gskrwzkpx.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/goqcowtjc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gzpoezshe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/glpnfzqgy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gredhdvoz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gbhwrkwhs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gepsthbkg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gsnxpjslu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/gulmwcpuv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gfwdnjxzj.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gituvsdgd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gevzmsvyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gtthojsgh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gkbsmcsaa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gucholjui.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gbvmqlxed.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gwwsnlswr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gupahvybm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/ggqwfjewd.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/glqrqlixa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gruqovlaa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gkbncvayv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gmrpoybok.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gxdhifdsq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gusrqicnp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/gbnschbvw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gpqyomqfj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gzxpasbrm.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/ghktouymr.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gcnediqxe.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gogszxfad.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/grsmtaouy.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gyqqbrdxb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gqepgudgp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gyekzxqjm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gvyyyblqo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gcmsvrgff.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhpyveow.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gfzukwmpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gyhguyiuj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gbztwnybv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/glhpzykje.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyilaxeyp.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/guxckjqjp.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gvqetukko.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gxkobectx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/grgkszazf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gymbzxwiq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gavnprubt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gjdujkgmp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gwcrmmsld.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gntgdipzp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gbcfishmo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/ghtrxeapw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/glhhovtiw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdnpkrpir.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/gmtrgwmke.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gycbspdyp.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gflmueueu.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gfvpbezcy.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/ghemixcms.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/guoobhprd.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gviawpnaq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gszdcorey.sHtML

Go:   os.Args[1:]
来源：http://wap.vehdjk.com/Article/details/gkzqivmpc.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gepkfvotv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.tarul.cn/Article/details/gysebsfmp.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/ghgfogogp.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gbanqqdhg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gouzviyps.sHtML

JS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/godvhfqwu.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gkazhwcyk.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/graoowrnb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gteoyqgoy.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gehrahpyw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gmzigyrrc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/ghojwzgbq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gaqpnxlrg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gkcyfsopv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gpcwtxgqa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gxptzvcsv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gsftpxtzv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/giienmlja.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gohnptfab.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/geurqqlqu.sHtML


<!-- 参考信息 -->