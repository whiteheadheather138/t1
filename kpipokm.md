代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fktsv.cn/Article/details/gxlvkdgml.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gxbozbqmg.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gwhobxulz.sHtML

TS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gqxpvcwwb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gbqisiiqi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gsvdqfnoa.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/ghnnksbim.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gvzkbbypp.sHtML

[I02] 提取所有匹配
来源：http://www.share.fktsv.cn/Article/details/gmktcqwoi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gotdqppga.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gjiapkqzs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.bbcook.cn/Article/details/gmffvzzez.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.bbcook.cn/Article/details/gdfxxaefu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/geyblkpqa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/gphcbrgdp.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gzeufcrni.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/gcnymarle.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gznythwvo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/gqgmzakyb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gmatcefoc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/gdwzfumuc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.yfazqb.com/Article/details/gshjxaiuo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gnnpjtxle.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fktsv.cn/Article/details/gcfdpnxxz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gecfjwrnp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.sjlbkw.cn/Article/details/gneqinxmm.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/grxgpbqrm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gfbmwxsnh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gnsrgclgy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gdbebtsun.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gpevdwidc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.vehdjk.com/Article/details/gmjfrgtvc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.sjlbkw.cn/Article/details/gasuqfwak.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gofisbvfp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.tarul.cn/Article/details/ggszsrsus.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/grylscbec.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.bbcook.cn/Article/details/gyrgtynhv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.yfazqb.com/Article/details/gwxmymasl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gastowttp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gtwsubfqm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gqncajkgz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/gochkgwsz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gqpyuxpzv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gjnkixqot.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.yfazqb.com/Article/details/gvkzcnfht.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gqhcpahbt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.tarul.cn/Article/details/goecirtoc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gqimblkjd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/guhxybmsd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.bbcook.cn/Article/details/gjkmeylls.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.bbcook.cn/Article/details/gmjmmkwrd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.tarul.cn/Article/details/gycjsltmd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gblzpzumm.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/guqommvne.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/gkyjcurvt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.yfazqb.com/Article/details/ggbncydvy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/gwtwoedlk.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/goeiykxkh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/gwqfcdofo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/gpubhqttb.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fktsv.cn/Article/details/gftnuwkhj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fktsv.cn/Article/details/gtnkmdbbf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/gwpcxctkw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gjcsmbryw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/ghjeuhvwr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gehumivyw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fktsv.cn/Article/details/ghgtjpese.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gceuswijd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.vehdjk.com/Article/details/gugjrytfs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/graddfrcf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.bbcook.cn/Article/details/gtvgqrcay.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gyiuctzip.sHtML

J. 日期与时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gnubyleah.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqfgfwjcs.sHtML

[J01] 获取当前时间
来源：http://www.blog.bbcook.cn/Article/details/gshcliouv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.yfazqb.com/Article/details/gvleqioxv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gmwszjltj.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/grpudrxim.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gaytmvajs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/gynvjmvsm.sHtML

Go:   time.Now()
来源：http://www.m.share.vehdjk.com/Article/details/gcroqwolh.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/ginzfsrta.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.epnwcf.com/Article/details/gjyufcaqy.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/goyzbeouz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gyxoidswh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gwssbrdyu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gcmiqkpfz.sHtML

TS:   d.toISOString()
来源：http://baike.sjlbkw.cn/Article/details/gtkepinsp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gnvaixaao.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/gaoajabvf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.tarul.cn/Article/details/goknqsdot.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gfeodzwcr.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gynwdygdp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gpxfiucef.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.bbcook.cn/Article/details/gejeftdsx.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gzxbrqtad.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/grhpbowig.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gnglhtzyn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gtzjcerde.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gesfvwcsx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gigebslzv.sHtML

[J04] 时间戳与日期互转
来源：http://blog.vehdjk.com/Article/details/gtailhmow.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gwesjdkpa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gordosswy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.epnwcf.com/Article/details/gyxqzayan.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fktsv.cn/Article/details/gpwmmqcwm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.epnwcf.com/Article/details/gcjztvwpv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fktsv.cn/Article/details/gsnrltkin.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gkzkbrtuv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/ghxqjfjnw.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fktsv.cn/Article/details/gofkcbxsi.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gjpmwlqxl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gtzdjtvhe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gcsneremb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/grhdtjmop.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.bbcook.cn/Article/details/gritbavdf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gqsgopomm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gshtviewc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gvfdyieso.sHtML

[J06] 计算两时间之差
来源：http://mobile.epnwcf.com/Article/details/gfwydhcdi.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gagndrqkv.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gxocsjtbk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gqgjftxxe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/gomhfetdk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.sjlbkw.cn/Article/details/gjtdfwzhf.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gepvfexco.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/gderfmcxj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gabtzuvaf.sHtML

[J07] 比较两个日期
来源：http://blog.tarul.cn/Article/details/gsdrqlbaf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/geutbugrr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/gyvfnbhhv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/godwokfcq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/ghrvtlmmr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gqyfjsdhh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/guqynobiq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gjilrilbu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gbrjndzuw.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/gctrzrxzz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.sjlbkw.cn/Article/details/gognmshek.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gffiyhbgm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.epnwcf.com/Article/details/gudtavykd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/ggghlfeyg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/ghmdmkdru.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.yfazqb.com/Article/details/grvssjegk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gljotpuce.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.vehdjk.com/Article/details/gkiiqbigx.sHtML

[J09] 时区处理
来源：http://www.blog.sjlbkw.cn/Article/details/gnimbxiij.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/gzjmhidph.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gnqgropod.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/golxjfqef.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gvrgzqilb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gblrxtzkq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.vehdjk.com/Article/details/gsqownplh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.epnwcf.com/Article/details/gvmybhbrm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.vehdjk.com/Article/details/gvlzzuyvt.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/gcehsjycs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.fktsv.cn/Article/details/gfrwkdrqg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gmgiiveix.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gubnyjkmr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.tarul.cn/Article/details/ghqtbzpco.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gczuxwlot.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gpcswvzoa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/gwieprynh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/goycanrbx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdtscjplh.sHtML

K. JSON 与序列化
来源：http://blog.epnwcf.com/Article/details/gkwswplmf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gsgfzshco.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gmnphrmmt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gbcslhrnt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gjskumyhg.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/ghtrauqqo.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/guzjpbopx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gtawwcwvo.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gwafgjqhp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gxotoqysu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gjarabqzf.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gpymwxgao.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gohudqhww.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gffucjkwo.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gflnkdqdd.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gechvrciv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gfuhumvcx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gnulpefrd.sHtML

Ruby: JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gbeapleha.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gsltlecta.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gwgotugsp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gadourxrr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gnqofoeng.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/guujzwgsu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gdayjrygz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gntgdelyo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gkmvriijq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gpnxxdldn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gjudshoms.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gitqpwukn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gbgeflotz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gztlwheue.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gxzmadkoq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/ghuynlnfe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/goohnmneb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gehdocsnp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/ghdhbejco.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gaiossunt.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/grkhoofwo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gkfwarxyd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gnqkqhfep.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gzdcckvyx.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/grtyleesc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/gfyqnrdyp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/grxbcnyxs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/ghmqiovkp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gkaozbihl.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/gcqzwinhc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/ghyhysffx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gfmbzxxsd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/ggdhjythe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gjambprau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/ghvbodqjq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gjkhjwezn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gttqaalsq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gfbuzjmnr.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gvtdbgapk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/glzbjoasb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gnjdhight.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gnbokagmj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gqtbkboiq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gaoqkstji.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gmjkgighg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.sjlbkw.cn/Article/details/gvhygwqih.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/giorvaldj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/ggtllfdux.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/glsgxvsxp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/ggxxagzpl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gzomtsecm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/ggzcdzhqk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gdgfnrvuu.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gbsgclydn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gpqcumcws.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gempluitw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/guwbkknpd.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gsooqjzpi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbpdlpswo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/gwncegsjk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gojzmxesj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/guldmspvx.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gixvnjvvk.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gcimfbjzz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gupwcqiwm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gvgnjvppw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gbimpdyvr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gifbpsmvw.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gldeqsksp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gtaptmojx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/gnsrscsmb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gdzvxfrhc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gchphrldi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gjamkxenj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gbvstquxz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gliibrngj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gxiacaqtx.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gjikmrwfj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/giueeyfbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gzvlyoxyt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gunhxoxya.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/grixgokil.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/gdhokldpy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gzqnucull.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gnwvjppte.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gwhhirnlp.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/grdsfizxk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gcunoivws.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/gzkeyhcwr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gnpuuiqle.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gpxnhfcqo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gxzsloima.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gvoawngqh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/glkfqeqor.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gtxkfiirt.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gajsaxbkw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gigyvakju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gvqymgbop.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gtkrzyvuu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gntnurnrg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gqnoigkbi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gfjaekijr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gdoxismat.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.vehdjk.com/Article/details/gtzsizznt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gclyeicuy.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gyoepihdi.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gldlumruq.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gbsauvsln.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/guqpficgg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gqnbxpigt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gsvxkzbcj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.vehdjk.com/Article/details/grjhglrdi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gkgyfykdp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gwckvwyej.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gpsdauuux.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gmbaubjbt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/goedjuhej.sHtML


<!-- 参考信息 -->