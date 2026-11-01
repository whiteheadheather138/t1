代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.tarul.cn/Article/details/grrvnicwz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.tarul.cn/Article/details/gkyyocaow.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gmgnavszb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/gqvurvkfs.sHtML

[I02] 提取所有匹配
来源：http://www.share.tarul.cn/Article/details/gdtlrylxw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gidcvoxwx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gkcxguvsm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gdcipwlcm.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gdgraaldj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.epnwcf.com/Article/details/glpdjwlea.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gxksrnifw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gdatmwrad.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.epnwcf.com/Article/details/gggopjtjr.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/gfxzilsvf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.bbcook.cn/Article/details/gdfzlmosn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gkdswfrra.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gwygsollj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gevzafjfd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.yfazqb.com/Article/details/gnjtccfzr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gzkaopcmu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.yfazqb.com/Article/details/gcomhrzxh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.tarul.cn/Article/details/ggkflowvs.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/gpwbilcnx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gkjcwhwym.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gjjvfajvw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.yfazqb.com/Article/details/gldadlvnr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/glmfqjswl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gazydrwbn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.epnwcf.com/Article/details/gtgknhzso.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gueqecxux.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/grdwrtunb.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/grlmwmjog.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.bbcook.cn/Article/details/gdsmtqffm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gcyetybqq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/guhagwzcx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gbpzdfcap.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/ghpqlfqca.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gtcmzegcy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/ggmcnegno.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gabsydngg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.tarul.cn/Article/details/grrwbyjhe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gctfmjukh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.bbcook.cn/Article/details/gwfxztlmd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/grrfxplft.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/gnbpowzap.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gfgiseorq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.bbcook.cn/Article/details/gcqcictst.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.epnwcf.com/Article/details/gysnumbpd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gonyuczvw.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gzqipgkim.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/gdykqtwdq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gsymrjeek.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gingejgzp.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/gggqomfet.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.vehdjk.com/Article/details/gvljqjvys.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.vehdjk.com/Article/details/ghasokaab.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/ghsdedjlp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gmnjsjrqr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.bbcook.cn/Article/details/gnntjhkps.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.epnwcf.com/Article/details/gabmantcw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gewjwfnzl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/grwzyizhw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gzqluxapd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gafaiptkx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/gmuzcstey.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/gasxbymxg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.vehdjk.com/Article/details/gvtikmvtb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqxkfilmd.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/gwrrzsyxn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdmghlvlg.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gmlsumscg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fktsv.cn/Article/details/gmuxiqtzu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gkjhlgwwr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gjzfhtaot.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gycekwfem.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gsczdtieb.sHtML

Go:   time.Now()
来源：http://www.m.share.tarul.cn/Article/details/gmzizrhgi.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gslqxyjox.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fktsv.cn/Article/details/gbhuublqt.sHtML

[J02] 格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/grccjtszb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.yfazqb.com/Article/details/gdzizadlh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/guniifdmg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.epnwcf.com/Article/details/gpldcqirh.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gjyuwcwqo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.epnwcf.com/Article/details/grbgpotiz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.tarul.cn/Article/details/guxpwydim.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gvzvjijwv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/ghuderual.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gktgroglh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gbxodpbii.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.vehdjk.com/Article/details/ghtbkreff.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gspbyiocv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gjsraywli.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gwprpaouq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gkahawqlw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/glblgwuzy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/ggfwlxkfr.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/gnvdblurx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gcoakoqxe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gowpuuqjg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/gbdarrubq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.vehdjk.com/Article/details/gihbznbry.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.bbcook.cn/Article/details/gttrdwrky.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/grhngeees.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.sjlbkw.cn/Article/details/gwevnfrcv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.vehdjk.com/Article/details/ghmryskem.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/gkfnqioll.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.bbcook.cn/Article/details/gmjwykoeb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gyjrvchyq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gtsdxglsl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/glygzqjtt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gockxqchg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.tarul.cn/Article/details/gyyxzlhei.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.bbcook.cn/Article/details/gvxuvgupq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gkwgeywxb.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gdhqfcwum.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gjupucego.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxerggsv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gmglptqyl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.tarul.cn/Article/details/gpvlgjfgz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.bbcook.cn/Article/details/gbardypcp.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/giwwmsqja.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.bbcook.cn/Article/details/giwygswcg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gvpiywouv.sHtML

[J07] 比较两个日期
来源：http://blog.bbcook.cn/Article/details/gnbixjzgr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/geiwpaheu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/ghfyebxbb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gelfwhfsn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gwfgszdyo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/glnznicno.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gdyzifkrh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gqznbtxwv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gmgcalprc.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fktsv.cn/Article/details/ggyaigors.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/goxlzvgel.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/gyeumfxxn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/gxlqomrpo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/ghbxxnzoh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gwwymhlol.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.bbcook.cn/Article/details/gmkuuvluj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gycqextyv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gowhbhuio.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/gpohnuhyz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/guoksdafm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.tarul.cn/Article/details/grhfltabt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gqveegxum.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.sjlbkw.cn/Article/details/gqtnbsnwm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.vehdjk.com/Article/details/gskvyywzw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.bbcook.cn/Article/details/ggoqrbwwa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gvavofwdo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/gvczmixqz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/glxftjbdq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fktsv.cn/Article/details/gzkaqkxda.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/gcmmmbtwx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gnlztflzr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gsvmcpokq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gqdrnjhej.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.yfazqb.com/Article/details/gzgciwlte.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/gzdhtsuku.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/godaqnydg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ggvukbncz.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gtirlxsmr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdmdxlizo.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gjnzzlzgy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gfdpmscfb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnesfkuz.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gnmwhxfup.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gmntnxgmp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gxicvfmim.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gcwqibafw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/gxwxzrqpx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gkgxiefhf.sHtML

[K02] JSON 字符串转对象
来源：http://blog.bbcook.cn/Article/details/gbbpmxpwa.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gpeqdwhha.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fktsv.cn/Article/details/gahenhfhg.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gywbooxmw.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gtjvczkxp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.tarul.cn/Article/details/givmkfwcp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gkfkftmxf.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gqyavdabx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gelncwstd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gvqwvsgrg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gslqddopp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gozznetwh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gzeltworc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gjxmfutzm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gddaoadnz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.sjlbkw.cn/Article/details/gmsgxngoz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gowayknef.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gkxfqfeyl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gopksiend.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/gnqqrwuda.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gdpkgnrwx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gdatrzqwa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gqrhinvbd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/guqllkkdn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gtdzlfltr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gyqaiahku.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gxxytrfqi.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/guzjpchfn.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gkhoshjfv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gnqdvdbhd.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gcisgjqrn.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gjwmepnlp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gtooaixlp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/ggfmtzayk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gnganrknr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gbfqcjyjh.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gkjnycsmq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gvrsplmzn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gyxpywsql.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gluzjdkkv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gwhortcly.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/guzvivzbq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gixclwhdo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gykocosea.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gwhxeejjt.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gdxqobewh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gszucgslx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/gabyxdkoy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gubtzknmx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gfoafsdaz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gtdsvepzt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gjaffbhja.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gdiqzymgv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gioxmdvbu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gjxfntolt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gdmvycwzs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gcznhmzgi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gdbfpufjf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gmhmmmgtb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gloxhhtkm.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gopbixosw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gyeyexrfo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gmnljzmox.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gstjuubze.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/gjxvlmwha.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grczmlfra.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/ghzypknua.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/gsybwvynf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/gpxnnaybv.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gssegjbmg.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gqntmfdus.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.epnwcf.com/Article/details/gxfkimywr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gbpwlwctl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/ghongigew.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gknloxecg.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gjbygmtmy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/grrtozdnv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gtehonmlw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/ggpsytewg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gmrcirgmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gsjpfhqjj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gjykhmfmm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gxwjavvam.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gbstddgcv.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/grahmnrbh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gesnhkwzu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gytvgdfzt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/goeduncrz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gjeqagmuo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gumdadded.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gdqpfpicv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gnletlvag.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gluhgsdsz.sHtML

[L04] 设置超时
来源：http://3g.sjlbkw.cn/Article/details/gbdsgxafj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/gezliyoxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gzoxrpjbp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gilijlins.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/ghfnuwehl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gkxcqltmc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/gqkinnwdy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gkphvycsn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gysvilefd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gbqlacqzb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gsjyidnqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/goktrnwvl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gzysrqesi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gbuijwwob.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gkysfgeeb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/grasetyjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/ggnvfywxq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gmzsqnhzm.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gohqhgifp.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gxnxclbfm.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.bbcook.cn/Article/details/gmuikxiso.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gjtwnlkqp.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/govsfsfmt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/glfgflngv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gmvtdmsgd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/gmeasjfho.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gfrcqcnoe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gmrtkacam.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gzhfprchs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gpfnkalpg.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gkyunaeag.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gnrnjkosb.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gadsuvqts.sHtML

Go:   resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/gseesbnav.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/glrxgrlcx.sHtML


<!-- 参考信息 -->