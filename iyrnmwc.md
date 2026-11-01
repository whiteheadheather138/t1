代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gtagtrvnc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gkghlkidg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gacwazmvd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gswzagomx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gisztgkfb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.epnwcf.com/Article/details/gjccsvqsi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/gcrhugazw.sHtML

[I05] 按正则拆分
来源：http://mobile.tarul.cn/Article/details/gschtltvi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwyjinic.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gphymcdsk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/grbfyniax.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gyqyqhrgd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gzjtriqrv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gmptxyusf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gnzdgryju.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gyshfezwd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.sjlbkw.cn/Article/details/gycworggh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.tarul.cn/Article/details/ggjsgygld.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.yfazqb.com/Article/details/gjmfdqjat.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gupmmoljy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gdperzmgy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.epnwcf.com/Article/details/gciwrolaq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gtlmgpfgy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.tarul.cn/Article/details/gtwtspmdo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gjtftploj.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.vehdjk.com/Article/details/gcchzqsoa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gcpfplbrl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gjpqojtdx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.bbcook.cn/Article/details/gsgogpkeh.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/gzvozjhbi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.vehdjk.com/Article/details/gnnjrkfac.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gnrxutulm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/gqhornopj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/gbwurlynq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.tarul.cn/Article/details/gwqcvnswz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fktsv.cn/Article/details/gsettnjil.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gfzoukcuj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gussqynwo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fktsv.cn/Article/details/gslmqbgoi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.epnwcf.com/Article/details/guercjfnt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.tarul.cn/Article/details/gjflftclv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.sjlbkw.cn/Article/details/gyqekfzpi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gaeolgwvj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdrskgani.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/ghrinevkh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzwagkwuy.sHtML

[J01] 获取当前时间
来源：http://m.share.epnwcf.com/Article/details/gkvjyzqzd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gxhbmjvuh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gzeispwhw.sHtML

JS:   new Date();  Date.now()
来源：http://blog.epnwcf.com/Article/details/gasiqnwgr.sHtML

TS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/geptfmxev.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.epnwcf.com/Article/details/grjbfquzd.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/gflkbqytn.sHtML

Ruby: Time.now
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvnyddcr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.bbcook.cn/Article/details/gktzhewfh.sHtML

[J02] 格式化输出
来源：http://baike.epnwcf.com/Article/details/grsbabguz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/giqeumegt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/giclxyxej.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gntagziok.sHtML

TS:   d.toISOString()
来源：http://wap.tarul.cn/Article/details/gcwzwhcym.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gwbpmimpd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.vehdjk.com/Article/details/ggbfiryva.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gqwlmepqs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.tarul.cn/Article/details/gdduacmcj.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gmvxwlzqw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gatfaaeai.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/gbdlhztmz.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gdsefvbkl.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gmnmhagee.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/glhetesfk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gxsjqqezi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gculmvgpz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gkmlmaiij.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gzxdqjczf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fktsv.cn/Article/details/goxwzalcb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.yfazqb.com/Article/details/gvynldmug.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.epnwcf.com/Article/details/gypeprmhw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/gffezjkwv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gtipqdpto.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaumgson.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/ghwbyksqd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gfmtnqclw.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gpdkgprqy.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/gbrdtrllz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gicxyffqg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/genrngkca.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gpfgrbbtw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fktsv.cn/Article/details/gdgeaotwy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gdrbhaaij.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gqjsxrenh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gvugydhyj.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/ggunyohhe.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/gickcfbrn.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.bbcook.cn/Article/details/gjsjtfsvv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gfeylayij.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/giwpkvihf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gnvhrjxym.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/gnhnrxdyq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fktsv.cn/Article/details/ghbkevtdy.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gtszdcczh.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/ggvknxzqw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gyvergrlx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gaqzgtyqc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gtgnuhznn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.yfazqb.com/Article/details/gztehwjzk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gregcbyaq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/geympurnq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gfoxczbsh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gyqtyyiee.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gfyoyqsho.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.yfazqb.com/Article/details/gasdlzjen.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gdwagelcx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.yfazqb.com/Article/details/gizlbdeyt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.yfazqb.com/Article/details/gqcebyqyl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.bbcook.cn/Article/details/ghjxqhzch.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gmrisuvok.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gmzbvuhzg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/ghvpirnxj.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gsejoekfn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gdanmeryz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gfsvspaic.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/ghfmqzgtv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gtvptsioo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gpfumojbs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fktsv.cn/Article/details/gyuitdlec.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gsalpevsy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/glqqmcctd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.yfazqb.com/Article/details/gbhauiphb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gcntsdire.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/guefsidnt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gtnedlmoy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/guvnblfms.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gwfptuaah.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.sjlbkw.cn/Article/details/gqloyttkz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gfnofofbj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gwzvkfmry.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpgqedrqx.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/glqjjjzkt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guztciicn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/gynegstvh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gmtcbuwev.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gepudmcmv.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gretiaikq.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gialdleqh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/giditrnxq.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gleoaxrip.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gooswkngf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gzvargggg.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gmectxhtp.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnslvvast.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gniielboy.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gzatyupze.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjkiortwi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/gomnqbmns.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gzcvrxqji.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gvlxmkoyw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwgyywtzl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/guvsxdwuw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gbliezyxm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gqmuhzrlg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gcpivvyzg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gjyhojmzn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fktsv.cn/Article/details/guiassznm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gbazksjnt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gtudusdln.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/grklnkaqc.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gwbdxsytz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gggugqkiv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gfqlefsji.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/glentaexj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gjhlqlrjn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/glknujlzj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gjqejmwvk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gyxvwmhrz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/gqahgpkrb.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/galifgujv.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gjushdyub.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gmibntquq.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gxfzijzzc.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gzwjfvuwu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.sjlbkw.cn/Article/details/gonhohlcj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gsxrwvhwq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gjfdhjyyy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gruhirteg.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fktsv.cn/Article/details/gsewmzcfx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gvlzkzhwt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gkrgqsdmd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gkghkazmh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/ggecxmoqb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gapahpryk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gyxhedzob.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gxfrwrgim.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gghupdnbj.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gasekylsu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gpfqxkvft.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/grsafaphi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gbyfipfwx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gbwpdojdl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/guvtloqew.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/grfmryvxh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/gwealhhrb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/giiqehpqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gneuswufn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gsylolbeh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/ghsmyzeqv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gbjewwzqw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/grjowuivu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/ggvrxhmyh.sHtML

Go:   encoding/gob
来源：http://www.m.share.fktsv.cn/Article/details/glzrahyro.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjgdhydpw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gtdhjnisd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gejenrxgn.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gmtwzebfn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gutrwdneg.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gtppeagbn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gowuggzou.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gyfkjbmvc.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/grrhlglen.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/ghflaisqo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gjsgkmupp.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/gywdbdoko.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.yfazqb.com/Article/details/geivxycsk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gnkdlbcvd.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gfiiyuine.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/ghpogrcho.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gfxwzqubq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gkvndykmm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gjoxxpzut.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gqyvjooiu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gghshozdl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gkyctoimk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/ghcukpeoq.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gwwkcbfiu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gilpiwlxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/ghvkgngrg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gwpamzbma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gdsvkkgkv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/gdluuniig.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gakericun.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/gcfgmwmau.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gryekovaz.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gqlyhxgjo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/gltivpacp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/grloevybg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gjswxfudj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gahhwtqvv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gzfllxryl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gckwfnvua.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gqileplsj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.bbcook.cn/Article/details/gwqofcnip.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gapxucfra.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/grdyznjqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/gbnorhplw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/griswqbga.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gnpscfdtk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gehbgslvh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/glcwmoscj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gqkkwwclc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gmvjvuxus.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/gcmwjfjsh.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/ghsqdpwri.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gavbwkulv.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gukuqogdz.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gbnfjywit.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/ghapbzegs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gquyanqrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gmtkyljkh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/gqofgjlqc.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/glhhsijvk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gzziikfox.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/garozoqdx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/geaeslgmc.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gykyecdls.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gbmvqddxh.sHtML

Go:   resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gbchnoxmf.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gvttsjxko.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gnasbqlsg.sHtML

[L08] 并发请求多个地址
来源：http://mobile.tarul.cn/Article/details/gfnyamcwu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/griieeimq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gpaxdlpdi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gxolngolv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gkvbxdrzb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/grahtuxcr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/gtxtmorgz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gwolahcam.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.tarul.cn/Article/details/gjquxfrnb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gewadiuwe.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gpirqhecv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzvkonyvk.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gseddqhui.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gdltqmhyw.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gposkuugz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gcacaohqo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gdtpgjajv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gojtwuxub.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gjgsgdxjr.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gjnjkukpc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gjilccwjf.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gnywejunx.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gyrmxswfh.sHtML


<!-- 参考信息 -->