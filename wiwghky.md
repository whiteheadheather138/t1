代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.epnwcf.com/Article/details/guitxugti.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/gfsqeewjf.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gkojyrdwm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/giwizqumz.sHtML

[I02] 提取所有匹配
来源：http://3g.fktsv.cn/Article/details/gfggrhpxr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gftpqvixc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gnknzmibs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gwfuvgbpw.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.bbcook.cn/Article/details/gdhulheir.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.yfazqb.com/Article/details/gbrltntpl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/gsjjlwfgl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.bbcook.cn/Article/details/gtzumdpsl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gwmzusbef.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gyavtjefc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.tarul.cn/Article/details/gwwntguvz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.bbcook.cn/Article/details/gdwabgmbb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.bbcook.cn/Article/details/guckeoumk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.yfazqb.com/Article/details/gkmbunamz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.sjlbkw.cn/Article/details/gdbcsrrpp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.bbcook.cn/Article/details/gzefkxiem.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gdgwxunsl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fktsv.cn/Article/details/gbioquycg.sHtML

[I04] 正则替换
来源：http://www.share.fktsv.cn/Article/details/gmzxdhmol.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.tarul.cn/Article/details/gnhturjrz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.yfazqb.com/Article/details/gmeroioki.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.yfazqb.com/Article/details/gknjqxsop.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gheeorjzc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/giixeverd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/ghuhsqaqc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.bbcook.cn/Article/details/gifavvbnh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrwsnahy.sHtML

[I05] 按正则拆分
来源：http://mobile.bbcook.cn/Article/details/gvyvhnfkh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/ghvesimvf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gmogdasmu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gkmfsbmbx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gdcsmordg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.vehdjk.com/Article/details/gqatiqvby.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gebcyrsci.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gpxhyyjci.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gmhxnssah.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/ggduqyeui.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gbnjojpig.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/goyvungth.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fktsv.cn/Article/details/ggaxevxeb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/guvwbleyg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.yfazqb.com/Article/details/gfipmgxzd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/gkbgnewbz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gijipvsuy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/glmdpnnkd.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/goqptknsr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/graibqorz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gfdwubuyh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.tarul.cn/Article/details/gaemgsxed.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gzjlyxale.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.epnwcf.com/Article/details/gvzduspww.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.sjlbkw.cn/Article/details/gkzlhkwbp.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gmjxnhorq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gsjboiepm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.epnwcf.com/Article/details/ggtcgvqtg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.vehdjk.com/Article/details/gwsexprra.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.epnwcf.com/Article/details/grftuitrl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gqvkpjnrr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gqofwspoy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.tarul.cn/Article/details/gdrvejqfp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/gcsarvbka.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gqvuplqcq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gxjdzrwdv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjtlrgfdb.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/gqywmkidn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtvjsssum.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gruizbfdc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gxxmhjlfq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gfixvsnye.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gqroqzbxa.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gjbadqnxo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/gdibfhyyn.sHtML

Go:   time.Now()
来源：http://www.blog.sjlbkw.cn/Article/details/gdqijonsi.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gdpznpexj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/goxrdvfwz.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrjnrzsc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gosuuezkf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gyumezndh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gmicupuqs.sHtML

TS:   d.toISOString()
来源：http://3g.epnwcf.com/Article/details/gdbpjrayu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/goawvrryk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.yfazqb.com/Article/details/gezbtmgkp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.yfazqb.com/Article/details/ggicgxcwj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gbvlqvxjv.sHtML

[J03] 字符串解析为日期
来源：http://blog.bbcook.cn/Article/details/gcykyqwle.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.sjlbkw.cn/Article/details/gjtktwagd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gbbijardf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gwwmmjivp.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gtyzcfgda.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/ggllhsahy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/glglbgbyk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gzoislsdx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gatewrpzq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gcvordwnm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gavxwmuzy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.tarul.cn/Article/details/gtqjaydkc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.vehdjk.com/Article/details/ggzvxpumh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gfyhipujd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gddxeuewq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.tarul.cn/Article/details/gpkakhvwi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gwuievnww.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gdjgczccj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fktsv.cn/Article/details/gvjfvxmcg.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/gtlxxfids.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fktsv.cn/Article/details/gzybbtjwt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gieqeelaw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gkauqfxzq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.vehdjk.com/Article/details/gwloidckr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/getornfxf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gkwvzdiqf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gjbpycwfa.sHtML

[J06] 计算两时间之差
来源：http://baike.sjlbkw.cn/Article/details/gesahiimu.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/grzljhgki.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.bbcook.cn/Article/details/gfxtevifq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.epnwcf.com/Article/details/gqmappuah.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.vehdjk.com/Article/details/gwlzyjmjk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gdbpfemyc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gearmmcbo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.yfazqb.com/Article/details/gfpxpvigi.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.tarul.cn/Article/details/gdjdfyety.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/gfxtzakju.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gfwvoqbam.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.tarul.cn/Article/details/gymrjoxxm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gsodspfin.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gvnsevhtu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/gcrdfmsfx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/ggwpbiukr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/guoavunyb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/grkzkytak.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/guoagkguu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/geuuqrtvl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gnzximmcf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gfynrhaet.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gjxlimonl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.vehdjk.com/Article/details/gstksfiwu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/gxggrynpt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/glaqrrnoi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gwndvpgef.sHtML

[J09] 时区处理
来源：http://blog.fktsv.cn/Article/details/gghsatgma.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gsbjrehps.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/gveimfabc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gpilhfiqo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/ghmmihpka.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gqnsoipey.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/gwotuxzlp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.sjlbkw.cn/Article/details/gzvskagvk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gciivhspn.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/gmocvhvcf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gnebeyahp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gtmfiybyt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gtunzofvw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gerkubrct.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/gdxelhuax.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/ghnxdqmmr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.epnwcf.com/Article/details/gxxmniwdz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxlzhsxo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcqswfzka.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/gkkpbceky.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/geapybhty.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gswlhgzvk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gvhwmpfun.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gxlekxykp.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gavuwmssp.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gavkgmeyr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.epnwcf.com/Article/details/gdpxtvupe.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gvxxkeqgz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gaehiymgg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/goqyfkhuf.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gschgazrp.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gqvxlmmhb.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/grvtlomgj.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gmwcmanqi.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gzhhjgyjm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gckfpmsrf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/ghesegqbk.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gctyzrnkl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gtxljdowb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gygokxkjv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gjnoapsii.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gfryfymjj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/ggcxyuihz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gygqucafp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fktsv.cn/Article/details/guwuxqrrv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjbexxmv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gyfptvbsx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fktsv.cn/Article/details/gxxdlsjru.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gowhgdutx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gmuthoztj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gbdsxzmlc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/guojwxfce.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gbgpzhxfs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/garfoibve.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gushrobtw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gacfetstv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvwkrbnw.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/groxiycad.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.epnwcf.com/Article/details/grjpbyajq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/gzcaduupp.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/glaenayyu.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gljvivupe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gstghfybu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gjfcvgsmb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gghihskwd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/gzfwdleow.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gjubtjmwt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gegewppxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gjkvhthgb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gnsefkcnl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gbruadzqx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gwhtxupjs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gfrsbfnbf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gyztwwqpj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gtxpfivtw.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/gkiepczea.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gxlogwwjt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/ghbjpgotl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gfccjqczy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/guobqmxrj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gungxwieg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gcjfxcftt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gyyyagjvs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gmcyzougb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gncgydxwk.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/ggoranhir.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gteulkrhv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gdwbosdxr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gxsjnoxwk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/grzxzispy.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gyfldpgoq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gohzhmjaa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gsejnjvrz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/grztgtnti.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gshmeehja.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gueinjoje.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/guuwxxkxz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gszwppvlh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gtayxidlg.sHtML

JS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/goyidaupa.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gbazjuklp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gxptnnpul.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gpgmyyysp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gglqkozuz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/gywrtmjcs.sHtML

[L02] 发送 POST JSON
来源：http://mobile.bbcook.cn/Article/details/gowrekndt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gfdoogrxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/golxupmdq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gohkiwazb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gdcbyoabr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gyiglgfms.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gxzwnuzei.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/glvbwdnyf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gcofxlbgm.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gfjuqbdgp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gczyvijmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/gngdteveh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/glznogydf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gxgxxztsh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gkiaaakoy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/goveczbrk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/ginnpcbuc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/glrmmgmov.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/guwogqyim.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gwjjteorf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gyrjisych.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gtggurtha.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/ghpwozrwx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/geofqoyjy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gsjkrehdr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gigzxezgz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/guhvyznrd.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/grxgzkiiu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gaqwpuejh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gryknokxh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/ghudwcidm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gytzrjpfb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gmwqdszyw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/ggosnebvo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gkbfmnjix.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gyqwqfels.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gafbcmimx.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gijitfkwe.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/ghkvlmqev.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/galghrzcp.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gelwdynme.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gypxfygpl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gmoqspfqx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gjujuiyoy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gplpfrcqm.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gvuzffubm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/ginnmbvke.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gnjhzpxap.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gguyswqhf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gevqzcjyw.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gaechxfer.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gzslzlzzn.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gnhmiudsm.sHtML


<!-- 参考信息 -->