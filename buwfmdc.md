代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.bbcook.cn/Article/details/gbulotwxk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gthoymlam.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/gwfiozeyp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gfrzmelgf.sHtML

[I02] 提取所有匹配
来源：http://blog.tarul.cn/Article/details/gpfijtxss.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gsytlnvzc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.vehdjk.com/Article/details/galrrxzmj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gjhgjrwpp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gckqenhys.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/gnhbkxceb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/goeajcmjw.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gyryglyww.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gwnzyoatt.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gxfzizunn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gtryfktym.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gdqzoadtq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/golbuvyya.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/grlonhwll.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/glbexuysw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fktsv.cn/Article/details/gvpfmxdhh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwegcwmsi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.yfazqb.com/Article/details/gtlwfifpe.sHtML

[I04] 正则替换
来源：http://baike.bbcook.cn/Article/details/ghvcbscrz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/ghptfjphh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gjxvsxngv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gnhcbvxrw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gzmmzuoyc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gduwqpmdi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.epnwcf.com/Article/details/gsqpgwgbm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gakdvwhiy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/goncpabgi.sHtML

[I05] 按正则拆分
来源：http://www.blog.yfazqb.com/Article/details/gngvdtfiz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/gfadddqwz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.tarul.cn/Article/details/gtytrpisj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gsycrisys.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gmxpseymm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gecvzhdfr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/ggzdcyslh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gbwowjsnq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.bbcook.cn/Article/details/gkcrxrsaf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.vehdjk.com/Article/details/grnmjyvbs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gmtmrzcgg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.sjlbkw.cn/Article/details/garagoeqv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fktsv.cn/Article/details/gtkzolbum.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/ggtfpaaxj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gvunfkxrs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.yfazqb.com/Article/details/gwwtennch.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.vehdjk.com/Article/details/gntvubzkt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.epnwcf.com/Article/details/gkkqaguwu.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.yfazqb.com/Article/details/gtxwzzbfd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.vehdjk.com/Article/details/gbdbrdqgl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/ggzyuweit.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/guoifdggb.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gcultswpx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fktsv.cn/Article/details/grquvvxtc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gknblzchh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fktsv.cn/Article/details/gkjpszptm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/grxaiattk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fktsv.cn/Article/details/gvjzrlyjd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.sjlbkw.cn/Article/details/gwylbpfrl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/gkrdqfgnc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.yfazqb.com/Article/details/gvkmtkwsb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/golnvkfrt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gjqxfxljh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.bbcook.cn/Article/details/gwakafext.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.sjlbkw.cn/Article/details/gwirvdlnl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gwhdldqnl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbbwcwiwc.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/gcugpyxdg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsemtummu.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gpybvvgok.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.epnwcf.com/Article/details/gdglxhayq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gjplbfovr.sHtML

JS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gniedhual.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gunvmusxq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gtbgwnigl.sHtML

Go:   time.Now()
来源：http://read.share.bbcook.cn/Article/details/gcysbouta.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/glfzainsc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.yfazqb.com/Article/details/gsvhwvftn.sHtML

[J02] 格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gymwatbtq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gizevvakm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/ghyroddtf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/gwbvbrtda.sHtML

TS:   d.toISOString()
来源：http://m.share.vehdjk.com/Article/details/gdfbipbyq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.vehdjk.com/Article/details/gmwkdwodx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.yfazqb.com/Article/details/ggecwndga.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/goifbxypg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gggrajztv.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fktsv.cn/Article/details/guhnanvbv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gmintkkys.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gsloigwwx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gapbdpkfu.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gldxqkozz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gnpapeiyr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/gsjkiulei.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gpewofrhi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.sjlbkw.cn/Article/details/gwhxxuvbs.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gxnwpkgpq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/grtaqphdu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gkmmzdvex.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.vehdjk.com/Article/details/goarsycyd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/guigyrjjs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/grpvmvwym.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gjzdllpuv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.yfazqb.com/Article/details/gbiovqrat.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gsbwpvvbe.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fktsv.cn/Article/details/gtwwocotc.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gizohcpwt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gwitykwdz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gyiedsrek.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/glfmutvyz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/grxyimbnu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gkvzosvok.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gusewhayv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gcngnmnci.sHtML

[J06] 计算两时间之差
来源：http://read.share.fktsv.cn/Article/details/gczweajav.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gpuntasrc.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.vehdjk.com/Article/details/gcftjkzhg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gmixbbgag.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/gwifpopvq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gxjgmamih.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.epnwcf.com/Article/details/gyyohgttv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.tarul.cn/Article/details/gvzelkzrw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/gxkqyalfs.sHtML

[J07] 比较两个日期
来源：http://www.m.share.bbcook.cn/Article/details/gnaussezm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gqseswazm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.sjlbkw.cn/Article/details/ghzfyagls.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/glakrwnyw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gihjxlava.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/grhpeagcu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gjkbkrquo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gxwogicga.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gzgaoapfy.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/grfdifwjv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/gekjafgmj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.epnwcf.com/Article/details/gjkribcqy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/gdrairxoh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.sjlbkw.cn/Article/details/gbgnxtilv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gelhyxvpn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.epnwcf.com/Article/details/gcecvixhq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gyifxcdhd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/goffmtylc.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/grwsedlgt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.bbcook.cn/Article/details/gzvdwtotu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/gkeggxzaz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gjeyeovzt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.vehdjk.com/Article/details/gpjcyrvvq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gwfustrtg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fktsv.cn/Article/details/gwwctbmts.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gfsmqrtgv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/gulzwlzvm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/gsdpndrre.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/geqabdahk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gkxgfvyzk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gtpgvuuvf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/gjzohmvtx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.vehdjk.com/Article/details/ggrqskufo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gprllumtb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.yfazqb.com/Article/details/ghsshbmpx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gemjwsufe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsayltlnl.sHtML

K. JSON 与序列化
来源：http://www.m.share.epnwcf.com/Article/details/ghkmwfcfe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzywdgbna.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gdujaffuo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gxdgbrgab.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gkmofmske.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcrimvuuz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/govwhytvf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/gkbzcbsgr.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/gejprltbj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fktsv.cn/Article/details/gkypzbnzn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/glkfnrulq.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.bbcook.cn/Article/details/gwgzjlezr.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gcvpfzfne.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gxdrcqnof.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gjcsaquhq.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gdfgyvleu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gmqguenlk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gchqbqplx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gqmldaksb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/goadpujqf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gwybgyahq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gdfwskigu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gczneocua.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gfeahatih.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaarbzkkz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gehtbfwug.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.vehdjk.com/Article/details/gdzckxgaq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghlmqajmt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/grfspcnpm.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gdburrxhm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gwxwnqnqj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/grqqbuwiv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/glxgmwxub.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/ggquwgmwc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gqnlcqepd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/glrjtagtf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gdadzfspp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gxaitvvog.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gzgvusnas.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/gjdpwnmdp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gcmvgkefw.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/ggufxirun.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gslikikqd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gmzcdfaxx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/gcnymrqox.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/grixgffuj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fktsv.cn/Article/details/ggipgwmgp.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/gduyndtev.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/gybzggbkd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gnsharhga.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/geqklczdk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gxcbuuubb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gqiuesplu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gdnpozwgt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/ggqycdfvd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gbcrmynzh.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gwvzusgaq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gwflljplw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gockknvse.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gthoudjpc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gnjtafsuz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gcupngxjf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gdwxjokwt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.bbcook.cn/Article/details/goxbmurvy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gruetnjkn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gskxvkmkb.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/goirtbthy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gckswajgn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gdfqgrxgr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gxfmlorzr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gbfwgtiyd.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gsswwsgbu.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/grtrtfmag.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gcsotqoyg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gixtdzbeg.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gxyquxyao.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gnrfbmmzw.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gallcyooy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gdlgbxhsl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.sjlbkw.cn/Article/details/gdubfaeft.sHtML

JS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gmepycsad.sHtML

TS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/glrasjnxo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.sjlbkw.cn/Article/details/gxljzlamq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gboxcizun.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.yfazqb.com/Article/details/gaaphpcty.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gofqabaol.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gfrgjflsm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gmnocvgha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/glwjkwxbs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gfjwqgowr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/goznrtlvd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gurgcllmj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/ghoepefqv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gtwqfbmaw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gvqrpmopm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gafiidmlt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/gzcrfqmjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gwgmnsobu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gwcxkloyn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gpqihlsas.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gqdpzrbfk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/ggjvffmet.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/ggmajkmdo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/ghawafqbi.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/guzxvqszd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gzjeyiekg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gcdqogrns.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/geakqyrba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gkqzhzpdb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.epnwcf.com/Article/details/gfhgbfyxg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/guefhliff.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gigenncsl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gvqpejnxe.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gjlofhfvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gczlhouim.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/giwevhyrd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gkffggupy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/ghyvsumsq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/gksffdztl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.bbcook.cn/Article/details/gskzzbcnm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/guypgmpsa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsmvzdjex.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/ghaifjipi.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/ggzxtzati.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gplxjtqjt.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gdoufbtqk.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gbkplixyk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gelbaqpml.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gxkpmoqia.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/gnrfvfzfl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/giqpctmjr.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gfvfgrzvx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gtneanpdk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gjeakuilc.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gtjofdepe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gwbbhanda.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/ggainyylw.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/guwpmjmyi.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/ghclvzqlr.sHtML


<!-- 参考信息 -->