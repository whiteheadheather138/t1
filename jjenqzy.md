代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fktsv.cn/Article/details/ghergrsxm.sHtML

[I03] 提取捕获分组
来源：http://wap.fktsv.cn/Article/details/giepqxcdz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gdsurmdvz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.vehdjk.com/Article/details/gjlpbtzgs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gziffqksi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gjbqcybty.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.yfazqb.com/Article/details/grmxsrzey.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.epnwcf.com/Article/details/ggysrlwto.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/grmeesvnk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gdomevzqq.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/gxogrnhxf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.yfazqb.com/Article/details/guiiyvdho.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gucqwlddq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.epnwcf.com/Article/details/gdvgnbtgg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gyxqihgtg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fktsv.cn/Article/details/gmoqqhggx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/gcyznfdfn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/ghgpnamau.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gqlhlsuhd.sHtML

[I05] 按正则拆分
来源：http://www.blog.tarul.cn/Article/details/gwfxwnwpl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gzwjfnokd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gawjjgzti.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gmthzxber.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/ggsmzsflw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gudsychxd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gzfmnnoll.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gycqzmqwa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/gkeqevhxc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gdiruovgw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gljsxzune.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/gujzdywzs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.tarul.cn/Article/details/gvwzhaols.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gxbimegxq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gequwnznw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gepvqkrqj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.yfazqb.com/Article/details/gesnffhkt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gpnqzrmvu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fktsv.cn/Article/details/gvzjqyedg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gevdlugfw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gulaknvvg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.epnwcf.com/Article/details/guziexeux.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gshxvjrjc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gwenmzcof.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fktsv.cn/Article/details/gsydjubqh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.sjlbkw.cn/Article/details/gnszbplyo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/gnumcmmpn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/gjufhnrms.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/ghyayywrz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gwxewamfl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gmabxbypy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gqohazcjr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/givyeqgou.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gjmmlxkzz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gminatunl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gnfznvtty.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpzjcokfb.sHtML

J. 日期与时间
来源：http://www.share.yfazqb.com/Article/details/gseinjxyw.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsnwlvldl.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gyppelaam.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.sjlbkw.cn/Article/details/gzymvvkfn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gsyoueihh.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gjajovsuw.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gkyxkoxwi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.bbcook.cn/Article/details/glesdsdwu.sHtML

Go:   time.Now()
来源：http://read.share.tarul.cn/Article/details/gydhmbazj.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gwbxxdczk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fktsv.cn/Article/details/ggohayxej.sHtML

[J02] 格式化输出
来源：http://3g.tarul.cn/Article/details/gendrpztq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gkdbzehzj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/glvxfugtc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gvpudcmip.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gunbqsjof.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gwixjbkqa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/goqnthjuh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fktsv.cn/Article/details/gylgrbqnk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fktsv.cn/Article/details/gjxozcjcp.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gjlqkftqo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.vehdjk.com/Article/details/gyasghtvx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.bbcook.cn/Article/details/gqzygccef.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gqpqtbdyt.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gwgjzdcbp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gyatiuxbl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gcqbuvbnc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gonucnxxy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fktsv.cn/Article/details/glytczrss.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gaenqlyyb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gkudrcutr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gaqwoxvdj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/gtogivdki.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/ghwdmlepa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gkjwdvjcn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.tarul.cn/Article/details/gcxqfwchn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gjgiodaqc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gsbndaegs.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gouqclbwk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gefhaynyk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.bbcook.cn/Article/details/gseqjlxeq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.tarul.cn/Article/details/gyylbqmet.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gsujpcjwp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gtnorgymj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gnjmhvbyn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/gxszyuwfg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gvoodrtlj.sHtML

[J06] 计算两时间之差
来源：http://mobile.vehdjk.com/Article/details/gqezxelpw.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fktsv.cn/Article/details/grgpvpwvj.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gsycsmwly.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gaqfucogs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/glzkpcyjb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gxemxaciu.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.vehdjk.com/Article/details/ghkftdtwq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gfymaqrso.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/gjqiaezbt.sHtML

[J07] 比较两个日期
来源：http://www.blog.tarul.cn/Article/details/gmszvtijn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gaijdpgsm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/ghixgilib.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gedzzerza.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/geliskfmf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gdciixjiv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/grgqvptvm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/guinqjfxq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/grnhgzkpe.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gnjlkjiwm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/gkoerqohn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/gwuxxscdo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/gfmleqzjd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/glijcjago.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gkxwqcglp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gpnpixlko.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.vehdjk.com/Article/details/gvgtpdcib.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.tarul.cn/Article/details/gwwtczpmg.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/gnujsruwj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gvxyzctql.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.yfazqb.com/Article/details/gizsiljse.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/ghrsmwywn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gbtylekfk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/gmzhobxez.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gwfulnhlz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.vehdjk.com/Article/details/grynjkrkv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/ggykpswyf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gdpebqhft.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/geywkkmva.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gduopwpcx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.tarul.cn/Article/details/gbnqfxwft.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/ggumjgqzt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/gkpumednb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/gppmxrahf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/gdtytgecx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gzxqpaghc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtxpxctok.sHtML

K. JSON 与序列化
来源：http://3g.fktsv.cn/Article/details/gbywmcnlr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtvebvzfz.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gtpnyishk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gtcyagbva.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/grsicgwye.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gbynuzqkj.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gjxcyvtri.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/giaqiiqve.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gzeuwdmno.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/glpjmsldb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.vehdjk.com/Article/details/gmvzxyhce.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gxotnfkkk.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gvbpydvcn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gfupalilw.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gwfuwtcgf.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gtnifepne.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gtplspois.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/ghifujmss.sHtML

Ruby: JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/grzfltieu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.sjlbkw.cn/Article/details/gupyhmptj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gsedvzxpw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gcehwpdte.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gqspucnds.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gwavtrvxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gizfiukiy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gyfazagjj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/ghnhhcjrr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gnnwnredj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gfpgvnllb.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/gcsbmjpia.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gumfhqdno.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.sjlbkw.cn/Article/details/gcqpentnm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gsrqjslof.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/ghztuwitw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gficvcdyz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gnkyyahse.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gvxurxrch.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gzvwffqkt.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/gqutehktz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gkcvcreup.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gjpchmjnk.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gccvtvpmq.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gjlzchcph.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/goxepvzbe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gdrjfbuds.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gplhxnatk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.vehdjk.com/Article/details/gtgfgkwob.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gsqojhdhk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gbtllfdkf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gtjrnvdpj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gjospjuyz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gyeodiani.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gdpzgoqvl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gcrghkoqm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gpjrgncfo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gfwtgemeu.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/grallvqyc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gphrrnzbk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/grwmtlkew.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gsrycmlpl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/guhyjasyv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gnqytcjtz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gcroxlcls.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gygnhmcbx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gdefpzqui.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.bbcook.cn/Article/details/galotuhtm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmskbbxrd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gcbbpkleg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gliulbtou.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gmqvijkme.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.tarul.cn/Article/details/geqboyxjz.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gigklinns.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/glwszmlud.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gdejffzgh.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggodqurhm.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/geuzecyfi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guyhlljeq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gdhplvalr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/guxbqccun.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/glzhbtnez.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gerlxwrlq.sHtML

TS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gxcubcrke.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/gxmrpqilr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.epnwcf.com/Article/details/gvdwyihkl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gwinlvnez.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gdqburyyp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gjeksutbz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gtqsgcirr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gnksutavm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/ggdalltor.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gpytvxcco.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gbisgzsdp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gksyskdjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/gkowgjavn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gokboidsx.sHtML

[L03] 设置自定义请求头
来源：http://blog.sjlbkw.cn/Article/details/gonsvewld.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.bbcook.cn/Article/details/gvvxfqcoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gseynklob.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gzsrjwjwq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gbkpmhqyz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gkbnsbcyc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gxwdlzdyo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/ghxitssqe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gmdfcmtvh.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gxtqzjunj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.bbcook.cn/Article/details/gnczhfpna.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gordutxyk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gvmgppiwv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gfkysnfsx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gpxudevao.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gufdjzxxd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/ghnjvkghg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gxrewrhio.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/ghovdczxx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gzajenyhh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gqpqbfune.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gfofpratx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gmlokndhx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gvbjnvxcv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gedonuecs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gnshynjay.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gtvtkcjfu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gzaupzcdk.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gncisiklg.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gztxdkfvi.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gytirtxxo.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gjsjtmdaa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gzbybyobp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gjnjouoqw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/glaednjhk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gczhxeric.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gpmwrjaxn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/garoyazpx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gmlwzeluz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gmujyhtut.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/grledavuq.sHtML

Java: resp.statusCode()
来源：http://wap.tarul.cn/Article/details/ghzfqpfgr.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gkksurugv.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gbyvrnfkx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gqkhxaxtq.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/gxyxrmgqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gierfsamz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/ggpuhfhgk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gqylyazek.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gnoedjwkv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/grwcqgweh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.bbcook.cn/Article/details/gqzjyiqhr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gccjedlab.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/garbulnfc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfjqdndxs.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gnyyshkqv.sHtML


<!-- 参考信息 -->