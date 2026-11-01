代发 wailian999

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghkoisrav.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gdjcmduto.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/golrmhgfv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gvhgkhtra.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gdtgbyinr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gpfzbjrgs.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gdogxhuxh.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gybjpjooz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.tarul.cn/Article/details/gbxmxzsyr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.yfazqb.com/Article/details/ghtoezqun.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/glcctlkhj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gbcofpbvn.sHtML

[I02] 提取所有匹配
来源：http://baike.vehdjk.com/Article/details/ghpszsdqg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fktsv.cn/Article/details/glffkusog.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/goxwdmotz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/ggjeyosfk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.sjlbkw.cn/Article/details/geccyoxcz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/gtshsrbal.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gcvniusqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.yfazqb.com/Article/details/gaihfxzyo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/goidsttpp.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gajoedgme.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/ggxfvibba.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fktsv.cn/Article/details/gyhiojbul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.tarul.cn/Article/details/govyevjez.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.bbcook.cn/Article/details/gpxqfebrd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.epnwcf.com/Article/details/gkgpntdeo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.sjlbkw.cn/Article/details/gyhntylub.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gkuerhkwo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/glubetffm.sHtML

[I04] 正则替换
来源：http://mobile.sjlbkw.cn/Article/details/ghabtpbnp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.epnwcf.com/Article/details/gnyzjsxdq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gtsqkgmnp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gsnhdvzod.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fktsv.cn/Article/details/gxiczemtr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gvopxwtde.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gomajbbkl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.yfazqb.com/Article/details/gzvkgagrk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.yfazqb.com/Article/details/gkshxeyeg.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/geslyazay.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/garobbgcm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/gceuqwuex.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/giuzkqftx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gzvnalsnx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fktsv.cn/Article/details/ghozmalgj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.tarul.cn/Article/details/gtwxtdmjh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.epnwcf.com/Article/details/gkeaskgev.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gybcotchn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gnxtzuqfz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/gszugqgcw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.vehdjk.com/Article/details/grfcvwlsv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/girlblbqq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.vehdjk.com/Article/details/gnxxpsdsr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.sjlbkw.cn/Article/details/ggopavdgc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gvvldwgdo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/grlomhzxy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gcdrcowsq.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fktsv.cn/Article/details/gonmwbsye.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.yfazqb.com/Article/details/gftgogmey.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gusnkjpnt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/gpcbttpkm.sHtML

TS:   /error/gim
来源：http://www.share.yfazqb.com/Article/details/gbgmcytnk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/gtornzrtv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.tarul.cn/Article/details/gnkovcqtj.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gvodznanf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gluwxcdep.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fktsv.cn/Article/details/gjfisklni.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/gwnqywhqv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gjdpgqivr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gmyxjbmtm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gnlinyhry.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/glphandcy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fktsv.cn/Article/details/gnsruqxez.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.tarul.cn/Article/details/gzdajqgmv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gjabdekdy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkrcvctrj.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gmyrmxbor.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzsixpdph.sHtML

[J01] 获取当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gsydgcuro.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.vehdjk.com/Article/details/gqorruuws.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gwgwflxif.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gtqbvhans.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gqsbxxhye.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.sjlbkw.cn/Article/details/gwmjemezp.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gofkvkeww.sHtML

Ruby: Time.now
来源：http://mobile.bbcook.cn/Article/details/gckksbjjf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gzutwocpt.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/grpcaakcm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gwzosvwss.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gscrazlyc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gxxzcboig.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gcfillqnf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/gheguzuzf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/gqjsahdnh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gfwsftrke.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/gonknipwm.sHtML

[J03] 字符串解析为日期
来源：http://blog.bbcook.cn/Article/details/gtlejpwnf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gsugbyzpp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gnajaisbw.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gjdqdprpi.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gtjeqgybv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gbuzqxydx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gdnsndxwn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gegqpjpuq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.tarul.cn/Article/details/gfhvfvrzm.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.tarul.cn/Article/details/gtceupwhl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.tarul.cn/Article/details/glncfowjp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gcmegqnkt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gsybfynby.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gfcwsoqyr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/ghnuuemks.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.vehdjk.com/Article/details/ggshnfxvj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gepxhwzkn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/gpohmhonr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/ghahqdvdm.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gvlpwszer.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gmsqjizvt.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqjpvjyd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.yfazqb.com/Article/details/gorzeeeyg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gjsyjqbfc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.sjlbkw.cn/Article/details/gnldenbiq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.vehdjk.com/Article/details/gtdsthikj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gzoukpcxd.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gitybdoev.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.vehdjk.com/Article/details/grwbmouhg.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.bbcook.cn/Article/details/geosilinl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.bbcook.cn/Article/details/gfxiwecjp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.tarul.cn/Article/details/gzomfacxj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/gtitpyahl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqzmziok.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/gmplewdvo.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gzriyvrkm.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/getgcrsja.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gqltmfcrw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gbftbwrkv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gobswfxrl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gflajkioq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gsxdolfxj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/ggsjjqemz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/grzrxotsc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.sjlbkw.cn/Article/details/gfveovyxo.sHtML

[J08] 提取年月日与星期
来源：http://read.share.yfazqb.com/Article/details/gnnjcggwm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.bbcook.cn/Article/details/gotcjaeol.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gkrkcvfyn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/gtnbihjnx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gefhymzzz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.yfazqb.com/Article/details/gjtwnrudy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gvkkuhjve.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/glhgrlxto.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gyygudgpx.sHtML

[J09] 时区处理
来源：http://www.blog.yfazqb.com/Article/details/gaeeulxnt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gfjnwzzua.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/gyyfkliff.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gygwnojeh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gbcvdjaqj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gryserene.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gupycjrvj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gstiptkpq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/ghudsrgja.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/gjtqiftjy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/gyekqsvpa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gqnliedgr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/gbqgxpbfh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.bbcook.cn/Article/details/gdmgvifhj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gyhoeybfk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.sjlbkw.cn/Article/details/geghmbipo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gylzexvns.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.tarul.cn/Article/details/gobhhzexb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvvyjldxa.sHtML

K. JSON 与序列化
来源：http://m.share.bbcook.cn/Article/details/gzevzpqqj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gquzwkoum.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/gzkjwkrbb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gpscjczwd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gmzjlvnme.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gwkvyyzpf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gxecatoxn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gpgzsjaei.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gjchoarqg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.yfazqb.com/Article/details/gleemkyut.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.epnwcf.com/Article/details/gddijpmba.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/giwltozhx.sHtML

Py:   json.loads(s)
来源：http://www.share.sjlbkw.cn/Article/details/gnebtfqgu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/gfozzegzz.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gcoizibds.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/ghudqeepd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/guxvikchh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gmfkgapha.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gqsbnjduq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gwdnhngne.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpwkdnyg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gxdlaissd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gwrfrqfci.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gugnhtarl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gisdotord.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/grmputuco.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/gsyrfgexx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gquolvpnh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/githncjsk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gdckxomoo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/gqvdleuxu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gqpgkpfyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfiucowh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gmobrrrdw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/guhhrbbcm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gvnpyyrzf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gociqzwlc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/grykwpamc.sHtML

[K05] 深拷贝对象
来源：http://www.blog.epnwcf.com/Article/details/ggwyazlhg.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.tarul.cn/Article/details/gaywyhoxs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gydcqnphs.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gmrugbktx.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gznreyitb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/ghcmkeorn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/ggwumuypc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gomlcxcxf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gxhgrcnug.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gtzqupdgj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/guhungdzt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/gqhrmczma.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gbxkerhbs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gmcycqres.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gzmsqbucy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/ggtcxbgca.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gqlftvtgo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gakigpplw.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/gbhsnexkk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/ghufxcmog.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gvegkpevy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gnbaogduu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gvcqsuojd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmptutds.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gpwnnract.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gphfsewgl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gzvydbwkd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.bbcook.cn/Article/details/gwmntvccg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.vehdjk.com/Article/details/glvfyxlqe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/grupxgnqc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gpjdknxfj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/ggwpbsjqu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gbcdnvayy.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/gtjshbbfe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gwygcztif.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/glgzwpohe.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqwlcrlno.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gugsfcmpu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gbehgxpub.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gdzzkgaez.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gnpcauxfc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gnoqeqhct.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gmthgzztu.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/ggttdedak.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gjxgkzdtp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gbgxgxlyx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gqwkxjall.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gkkcbdkzk.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/goagttktm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/ggxobnclr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/grgwqinhr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gydriivka.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gkwnwkate.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/ghkshqxvc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gvfexsxwi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gzkperwkh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gqngsxioh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gpyadeess.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/gntdsetlr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gjwutfwva.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gujhjoeuv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gzlorjbjh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.tarul.cn/Article/details/gzaaxscaz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gdnuhgcoz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gcckujjtm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gjymrzkru.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gbtyyalmb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gxvooncsk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gjjepgvwr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/glzxtpcdr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gximtcuiq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gykaswtlr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.tarul.cn/Article/details/gizjfiwfj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/gkfxkfjmj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/ginbrxyhm.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gvvgvjeik.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gvdxewncz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gzcpkkuqb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gwqzgzoyg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gucempnqo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gsizbzkzk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gqjgapwnl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gfvbjjdrj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gjrsgeluh.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/gduyckzxh.sHtML

Py:   resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gfzimdivj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/gokxetdei.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gvqocdiwi.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gzfkurqwa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gkqzajmep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gomppbono.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gxunlqwzi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gjltuzcfx.sHtML


<!-- 参考信息 -->