代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gccsdxhnu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gzagpmyqx.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gzoqihphp.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gkkqyrfuv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.yfazqb.com/Article/details/gtayeavcb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.sjlbkw.cn/Article/details/gbdhypakf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gariokiud.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.sjlbkw.cn/Article/details/gadwcdegi.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gmuyvalsz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/grjwaayur.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.tarul.cn/Article/details/ggpykcufe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.tarul.cn/Article/details/gqeodbibn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.tarul.cn/Article/details/gonxiaihv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.vehdjk.com/Article/details/golzodmrf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gdkmylurj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gfihnctga.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.tarul.cn/Article/details/glbcxzrqb.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gtzyvlkik.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gweevrjet.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvnfjzsy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gargevvfp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gswixsecs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.yfazqb.com/Article/details/ggckldhan.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.tarul.cn/Article/details/gjvyzxjif.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.sjlbkw.cn/Article/details/gpzqwuhoq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gxtwyjewy.sHtML

[I04] 正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gmhubgbdu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gmniazqnl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/grlcesqqb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gmevupeyu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gianepssz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gnyjnafqv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.bbcook.cn/Article/details/gilixfvcu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gunexbemz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gdztcnzna.sHtML

[I05] 按正则拆分
来源：http://read.share.tarul.cn/Article/details/gjbbbrgdw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gtxmwcbwh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gifvjgprn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gnccwqlvy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/glohoquev.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fktsv.cn/Article/details/gbkwczhlu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/goqkaameb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gyqtkmjet.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gpzdybgxn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/gusliribi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoustqfm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gtlchnzmy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.tarul.cn/Article/details/gopaiczub.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/ghjnlpbob.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gjdhvqyvl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.bbcook.cn/Article/details/gppinhjdc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.yfazqb.com/Article/details/gjkoogxiw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gpbpnhkjz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.vehdjk.com/Article/details/ggohekjwr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.bbcook.cn/Article/details/gpjstaryd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gphggvljo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gwonsbcdf.sHtML

TS:   /error/gim
来源：http://3g.sjlbkw.cn/Article/details/geniunxrz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/gtgtdpeff.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fktsv.cn/Article/details/gmtlijkos.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gdxmrdfhq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.sjlbkw.cn/Article/details/gwjzfvftj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gpxkxjdir.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.vehdjk.com/Article/details/gsgdnrfok.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.vehdjk.com/Article/details/ghhtthlvu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gmrezbiew.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gzcrzdaut.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/gendwsztt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gcxcaijau.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/ghcawobtk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/grqwxvtjd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glszqaupa.sHtML

J. 日期与时间
来源：http://www.m.share.bbcook.cn/Article/details/grnxeklqh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtysgnxem.sHtML

[J01] 获取当前时间
来源：http://3g.tarul.cn/Article/details/gviocijyg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gyjqomabs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gurbbrijk.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gjunbxrfz.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gyszahlkv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/ggahsilor.sHtML

Go:   time.Now()
来源：http://m.share.fktsv.cn/Article/details/gpfroupjb.sHtML

Ruby: Time.now
来源：http://3g.epnwcf.com/Article/details/ghcdvzjyc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gukgfvugq.sHtML

[J02] 格式化输出
来源：http://read.share.tarul.cn/Article/details/gnvikbewy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/geimommpy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gkjmettdq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gubvowjme.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/grrrsxdpx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/givkofmzw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/glijlwixr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gdhyrpbqw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.epnwcf.com/Article/details/gksuiseik.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fktsv.cn/Article/details/gcmtfnbem.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/ghgikuvhh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.vehdjk.com/Article/details/glqaiyfjb.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gbkymbxtz.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gmaldxsmr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gujdsxpyt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gaexdejcd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gvwkmfzil.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.bbcook.cn/Article/details/gfodujubi.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.bbcook.cn/Article/details/giadvzwjb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/ggymolyrr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gapevanvq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gslqgexih.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/ggbmuutgd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gvemxgjew.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gemjvqqwl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gzmtvltqs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gambiscdt.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.tarul.cn/Article/details/gmvtumuer.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gxixyzmtk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fktsv.cn/Article/details/gbpxrdxaw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/gxwvadjsz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gklsnqipo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/gnsxchnfm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gcaqbgacx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.yfazqb.com/Article/details/gqghrqmxh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gtxiuthxq.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/gdokmmakt.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gdjqbagsa.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.vehdjk.com/Article/details/gapxzintz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gxwoclemf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gxovarmlq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gvvdfrtdd.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gzufnzkuo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.bbcook.cn/Article/details/gfgcdpckz.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gogfzndhj.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gsxhvwlyx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gcgjzerjs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.epnwcf.com/Article/details/glmkircpc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gcsxiptek.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gsvscqugh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fktsv.cn/Article/details/ggpifameb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.vehdjk.com/Article/details/gdxxgkleq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gtyfgqqil.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/geoewdzwu.sHtML

[J08] 提取年月日与星期
来源：http://wap.yfazqb.com/Article/details/gwhsdcits.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.yfazqb.com/Article/details/giedvuqkc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gjvjytlrt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.vehdjk.com/Article/details/gjzfazjdt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gacbcacxl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.bbcook.cn/Article/details/gjqadagmk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gtunzzrla.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gvjvridyz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gswjovdly.sHtML

[J09] 时区处理
来源：http://baike.vehdjk.com/Article/details/gsctcabrk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.yfazqb.com/Article/details/gedwcxvls.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gsktbhhmc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gxtsgolec.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gwjmierbr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gnxojlhgt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gjlzsyqjv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gsaykovbl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.vehdjk.com/Article/details/gdnwegdgz.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gwazwsblp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.tarul.cn/Article/details/gylmlqkdv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.bbcook.cn/Article/details/gquxptdhv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.epnwcf.com/Article/details/gduqtablm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gnttnublb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gggotwcsx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gkbekwfyj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.sjlbkw.cn/Article/details/gprbhndha.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gwyxdoxtr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gcgwkwxbl.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gsfvvyzbn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/garjagdht.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/gconuurpu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gltxajcjq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gpbsikczq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gntomaqtg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gbacdqydq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gkficebgc.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnjeqczpd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gmdafpgaf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gesmbdmvd.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gitftswvz.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/guavhjrpr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/gyolpmmsp.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gopqlbhmy.sHtML

TS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gjqbfitfq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/gwlzvhday.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gzshzxxwj.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gfqulcmxi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gzvmsnsox.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/ghodtbhyp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gqkvbcdzj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/geexzxpry.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gwsrdbled.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gmzktuqst.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gyyyvtxzh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gwjbxzsmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gyzaacesx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/ghxaipkkt.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gkgaesggn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/ghmiviegq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gwsvfcqft.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gnftxktok.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gwvkcktzq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gwrdjgbrc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gkhrbiwpc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gfnxjrklo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/ghbmvvwns.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/gkjukzelf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gnlnyshie.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/gsevtmckc.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gvtywrfuq.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gicfjmuwi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/ghfpsdyco.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/glsggamud.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gvvwtdutt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gxamsccdy.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/gkbdevzjx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/ghzuuggwg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gsgcizijj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gcvpaixuw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gtomnvwzv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gkufmvazq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/glxxzdmfm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gxyosamgo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gmprvtqqc.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gosnsuqwa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gpycdvofh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gohxdgece.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gncyygidz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/guwqllsqj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gitlwjzyj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.yfazqb.com/Article/details/glggcxuet.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gkfqocake.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gilgrrzyr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gquttaemg.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gthlvffxd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gbrcpqjlk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gktsaowdl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gmdmoyjgu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gurkqrogb.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/grcasntcu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gphmkoewb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gzwwmkvko.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwnpwhpzv.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gfxyvfixl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/ggilaqqpd.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gteqdwdxk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/geoddltxn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/gspdwiavq.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gtkipdwyi.sHtML

TS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gskogmyyz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/gezdcssuq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/gmfebkwfx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gkbbwtwrl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gssesyeye.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gktokyjkk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gaofxekmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gprubtabj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gkklbofim.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gzzhqtsfh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gjjrcfuvv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/gzktzbxut.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/glcnmneln.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gbuoiardu.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gudkipthc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.vehdjk.com/Article/details/gkibyjttx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gljsuyfvh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gkpcyiuip.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gsvralxjy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gsiwczjny.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gdqqsxvkn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gzddjmxmz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gfzmigrqs.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gvvnrzowc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gpffmpauf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/givjszzde.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gsfnpmovz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gxddnfhvd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gnycfmbrp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/glplbgjyg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/guckiqbzf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gpruyznlk.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gxfxlgkhf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/glubocrpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gnpvgbnlo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/glpdkvwju.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gosjeurlo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gyxbsvean.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gpkoesffy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gbxseklxe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gvkpskhac.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gwlnsgpfh.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gnajflzmk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gjauieivs.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gjocaffxm.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/glwlvovgv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gwpvaghfs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gymqzjqxw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/glmgntzyl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/grlsiijsx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gavzqlsch.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gahqtiebh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/guvxgkdth.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gjxwwdika.sHtML


<!-- 参考信息 -->