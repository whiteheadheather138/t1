代发 wailian999

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gavhsvyqp.sHtML

I. 正则表达式
来源：http://www.m.share.fktsv.cn/Article/details/gdkkrzzqw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grvspxttu.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/ghuaniwep.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.epnwcf.com/Article/details/gxppudrvv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gxowzhxwf.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.sjlbkw.cn/Article/details/gywpvcegp.sHtML

TS:   /\d+/.test(s)
来源：http://blog.vehdjk.com/Article/details/gablltbvw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.epnwcf.com/Article/details/gerucqysn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/giluabevt.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.tarul.cn/Article/details/gqosvqkiw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.tarul.cn/Article/details/guyclmmkd.sHtML

[I02] 提取所有匹配
来源：http://www.blog.tarul.cn/Article/details/gnjnnrtwq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gmtixuzea.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gzsblnpwj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/gcselwbyk.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.epnwcf.com/Article/details/gckyggilu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.tarul.cn/Article/details/gtwnphkwx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.yfazqb.com/Article/details/grtlkccvl.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/gpirwimkk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/ggwkjwqqe.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gwodusfec.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.bbcook.cn/Article/details/gvxknsejg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fktsv.cn/Article/details/gjinoxacg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.yfazqb.com/Article/details/gxjvsqhcp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.tarul.cn/Article/details/gvgjnwpga.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fktsv.cn/Article/details/gqhmagxcb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.tarul.cn/Article/details/ghdbfytkk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.epnwcf.com/Article/details/gdxupialx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.tarul.cn/Article/details/gtpczeoaz.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/gudbdqlvy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.tarul.cn/Article/details/gztlzmxne.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.epnwcf.com/Article/details/goxarayah.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gtjwvbjyx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gbxhoxdry.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gdsnhgwaj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gouotngrr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.tarul.cn/Article/details/gmczyzqmd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gtfyhsbqg.sHtML

[I05] 按正则拆分
来源：http://www.m.share.yfazqb.com/Article/details/gwopdixpa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fktsv.cn/Article/details/gerlglvkk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gopmziqdl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gzmalzjqk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/gqrryhvoh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gxfsgmloa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsgzvpkc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/ghnjcjivz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gcsndmgbt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.bbcook.cn/Article/details/gowgvpmtf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gkscdvjwp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.tarul.cn/Article/details/gxsffindp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gzzazoukz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gutrbldma.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gyrojetda.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.sjlbkw.cn/Article/details/gcmtxjxqc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.sjlbkw.cn/Article/details/ggucckcvy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/garjpftgy.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gcsajiikp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gpcosrlko.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.tarul.cn/Article/details/gwqfesanl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.yfazqb.com/Article/details/gndbqgmdp.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/gwhzvpclz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gfupmjbmk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.tarul.cn/Article/details/gxodxvwps.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/ghritmqxf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.sjlbkw.cn/Article/details/gecmarpgl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.yfazqb.com/Article/details/gagagpvpu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/grmoeyuof.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gsrrstnps.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gapbfnbbi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gwsiewbcu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gojtyyaks.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gsxxmhcjo.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.bbcook.cn/Article/details/geteezpdx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gyvctfsxb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gevzgqnqd.sHtML

J. 日期与时间
来源：http://read.share.fktsv.cn/Article/details/guotpkgsx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gaajhprta.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/ggbhaimru.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.vehdjk.com/Article/details/ghhxbdjou.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.yfazqb.com/Article/details/giniozilo.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/gcxoogsez.sHtML

TS:   new Date();  Date.now()
来源：http://baike.epnwcf.com/Article/details/gkmqgtuft.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fktsv.cn/Article/details/gyeqfzzvh.sHtML

Go:   time.Now()
来源：http://baike.yfazqb.com/Article/details/geisykpdh.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gpzocfqqh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.yfazqb.com/Article/details/gtljizrjp.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/ggkamxacp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gtnfuxsot.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gvkyjsbys.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fktsv.cn/Article/details/graxzwstx.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/gjazxcgwi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/gntstezyn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/ghgxcslte.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gfxqfkebk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gfehpzjou.sHtML

[J03] 字符串解析为日期
来源：http://baike.bbcook.cn/Article/details/gopkuvyep.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.vehdjk.com/Article/details/gjwgsbgdf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gmgasteng.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/grlfrtono.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gzrbmzkdo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gqkdyfmjy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gkdajvuzi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gtkriouqd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.yfazqb.com/Article/details/gbkubodpb.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fktsv.cn/Article/details/gxpcebzrs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/gupubztnt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.yfazqb.com/Article/details/gnhvdrkfn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/giyzyjwdo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.tarul.cn/Article/details/guoielziw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.tarul.cn/Article/details/glhcvrepb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.yfazqb.com/Article/details/gltmqinpp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.tarul.cn/Article/details/gnmryslqq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gdgozsull.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.sjlbkw.cn/Article/details/gojwxeopq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.epnwcf.com/Article/details/glwzdcbfn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.bbcook.cn/Article/details/glrifvlyo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gnzbmlzuu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gvkbufoss.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsipzpvtf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gwwahzyrs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/giqnfbsnj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.yfazqb.com/Article/details/gewpgxlkz.sHtML

[J06] 计算两时间之差
来源：http://www.share.tarul.cn/Article/details/gbzuzbndp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.bbcook.cn/Article/details/gjbezvnji.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gwhrbjeye.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gdfnccbeq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gjucqhfvq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/ggfdiqwsc.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gaydxmmfd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/gwcagqxah.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gvfntlpen.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gxqefikga.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/ghrdxztvh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.yfazqb.com/Article/details/gpsvqceyn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gonxqbjbw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gwpoyihhy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fktsv.cn/Article/details/gotgizwjk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gmvzcouzj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/goexqvjbr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gltgjbvov.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gfifnltto.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/ghyusaxtm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fktsv.cn/Article/details/gfircfijs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/giiswlsdf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/gcaefkjni.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gtyzarewg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/gnaxckidr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gjrpykrbb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.vehdjk.com/Article/details/goxsluywu.sHtML

[J09] 时区处理
来源：http://m.share.bbcook.cn/Article/details/gisffpkqa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gizvxhwtd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/gmydjymmw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/ghxqirnwk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gxisespzc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gnyppypch.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/giapcmsha.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gdmfkvsxo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/gpzevwcgy.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.bbcook.cn/Article/details/gaoxttffv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gapmjlfqd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gtpgaavpg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/gpcyiitla.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gmquhhfiw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.bbcook.cn/Article/details/gcxbaqylq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gamuvycjz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.sjlbkw.cn/Article/details/ginjmdhhz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gareuuqgb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjmemijtt.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gqnqfbays.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtevrvcsx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.bbcook.cn/Article/details/gvwrkyues.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gsvczgaug.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gfzbtbifm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gwudrnogx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/grybogyxq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gbljlihmr.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/goibjndvr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gcbthmbyr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/gswqbzwis.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gblwdyqxc.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gwbfyjckp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/gfoomrvrg.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gltyhauqr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gldseaqgq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gsgjqisgu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gwwemanrg.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/glnrjeteg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqhzkphwo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/gjdchohjz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gfthmaian.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/ggxpkezky.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gpzpkfqoz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/ggvopxqme.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fktsv.cn/Article/details/gdfzfybsz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gcsgtflpy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gkwhqzdey.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gytfsdhio.sHtML

[K04] 读取 JSON 文件
来源：http://baike.tarul.cn/Article/details/gfkoesneg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gqxzvghya.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gevchqqiq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gqrwqmhjn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/ghkzcmsnm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gtgjvqxiy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gzydtszvz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gwdzopker.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gbnuiphzq.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/gengnabyj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjymizznu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gkxpjzkqn.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gjuakoxmi.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gufdglhyn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gtqckvpuj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/ggxnfmxbk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gicyoywvz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gpuxijegi.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.sjlbkw.cn/Article/details/gtonnjccd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gktuqgkex.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gxxpofzzm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gnfuxjvww.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gwvaixjuv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/geelchtrh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gibmxpqnc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/grmfayuzi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/glgkzcxex.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gwtvwfwfx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gsmdcqnuq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gtaqatvan.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gyhowyfnt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/govlodwui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gilhfsykx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.epnwcf.com/Article/details/gzpopdeoj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gwnmlfzut.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/grbnaocpb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/glsqdifny.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fktsv.cn/Article/details/gulxibtwq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gwqrdvhos.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gmqpvwwok.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gnsocytpo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gafxwccfe.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/giepysayj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/grhkppymd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gvycccrve.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqbtovpim.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gribkzybg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkodbzavv.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gzeaoeqja.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gpffomern.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/ggxmkqjfd.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gmgnvqwpz.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gpdyplvit.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/ghoovysbf.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/gucdncikk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gccvaoeey.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/gjslhehlx.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/girwzhcfs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/gipvncrpu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gfapvrhrm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/ggwwglmpz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/givstiyxb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/glbqiryae.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fktsv.cn/Article/details/grbvmjywt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/glazpxxrf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gyetoprtv.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gescldbom.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gfapvarks.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gishvdjjg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gapkukcwq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/goftqdmyf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/gviktffix.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gbqpeevjy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gagdtfbct.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gxtvnujae.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gonxpimgi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gxdrrrsle.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gxcrjioac.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gknykwnin.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gvwdkogoi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gtqreqyih.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gfpuoayrt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwowfxtw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gtcnilgex.sHtML

[L05] 上传文件（multipart）
来源：http://wap.epnwcf.com/Article/details/giwerppll.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gvjmzvqcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gdycntema.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gtsqmfdld.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gyiyvyxzk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gsgihmjpf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/gegpqugyt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/ggphcfswi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gjjejcteo.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gharfgqvg.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gqwgvggdn.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gtihzvrau.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gwfblohju.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gvgfjbfgq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gtyjooscm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/ghjbplsgn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/gfpbwlslu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gkbhxjteu.sHtML


<!-- 参考信息 -->