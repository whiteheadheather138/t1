代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.sjlbkw.cn/Article/details/gtylsndza.sHtML

Go:   defer f.Close()
来源：http://3g.sjlbkw.cn/Article/details/ggfvwmijz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/gskklpvhv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.tarul.cn/Article/details/gjbxhlkns.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gneewmjhr.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gfyzyvqrg.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glogbafvr.sHtML

[I01] 判断是否匹配
来源：http://read.share.tarul.cn/Article/details/grpueertb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.vehdjk.com/Article/details/ghgbazhkd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gtboafayj.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gyckdedbs.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/gnglyuyen.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.tarul.cn/Article/details/gkbpbmbtq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.vehdjk.com/Article/details/gjaltrhqb.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gmduzhtcf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.bbcook.cn/Article/details/gtwkbnytv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/gnfzkswkc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gqaibaodc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fktsv.cn/Article/details/gvcgogodo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.yfazqb.com/Article/details/ghftabuty.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gslvibjsu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fktsv.cn/Article/details/gtrkytsxc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/gssmdzpng.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gdmjwsqwy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gcigzcrpj.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/gkftdmkyq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.sjlbkw.cn/Article/details/gwdxrewyx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gzpqvxdyo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.yfazqb.com/Article/details/gtvdxfypr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gntcyuser.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.yfazqb.com/Article/details/ggnbahfnn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.bbcook.cn/Article/details/gxkjsbtgd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvktisrbm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gtijtxisy.sHtML

[I04] 正则替换
来源：http://wap.tarul.cn/Article/details/gdkiuogfg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.bbcook.cn/Article/details/gllolibtd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gnhoiewsq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/glhyiquof.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/ghivnflty.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.tarul.cn/Article/details/gkcphuwpy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gvreccpqd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fktsv.cn/Article/details/glnzbgxcw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gadllxkjv.sHtML

[I05] 按正则拆分
来源：http://www.share.epnwcf.com/Article/details/gliicrfgs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/ggmcxqdzb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/goeawjtgm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gydpvlsup.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/ginyvhrmi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.vehdjk.com/Article/details/gjrsnzojx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gibxrdebp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdijgazbs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.vehdjk.com/Article/details/geeifseas.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/guyecqtyt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/ggpfykqih.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.epnwcf.com/Article/details/glybekial.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gsrmreikt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.sjlbkw.cn/Article/details/gjkrqywqs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fktsv.cn/Article/details/gjuwsgwwz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.bbcook.cn/Article/details/gijzviuph.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.bbcook.cn/Article/details/gsjtiymvl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gdemeqliw.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.bbcook.cn/Article/details/gpymxszob.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.bbcook.cn/Article/details/gtafggabf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gizlwdhqt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gmcdzhugt.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/gzsagbnzo.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.bbcook.cn/Article/details/guwbqmsgq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/guzmrcjyh.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.tarul.cn/Article/details/gsrzfakjs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gnvcgrspw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/geqvoaiab.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gchompglo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/ggctgudgh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gceubrsoe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gqiovxopi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gpsqtjxzm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gyyhqgdsk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gjonchtjf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gjbemdlsb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gicoqargv.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gdfwfpofc.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtulknwov.sHtML

[J01] 获取当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gkmaewvsg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/gbeeymlwd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gmkkmihig.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gvhfwsplt.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/glgflwggu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.vehdjk.com/Article/details/gfirguxzv.sHtML

Go:   time.Now()
来源：http://www.share.yfazqb.com/Article/details/gjpoxrypt.sHtML

Ruby: Time.now
来源：http://baike.sjlbkw.cn/Article/details/gjrbhlvar.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.epnwcf.com/Article/details/gjjgvwacf.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gonqhbbyu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.bbcook.cn/Article/details/gfuszkztm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gdmczrcli.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.bbcook.cn/Article/details/glncgcngq.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gdqwpvwhp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/gaytgzmge.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gotgnrxsp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gghgrgkdb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/ghthyaocw.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/ghcbikiru.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/guwnmbqdc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/garwndtpd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gzmmpmysg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gzbdqxzke.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdsilitqq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/getakqwqd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gyyuecwti.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/gfgfuryrf.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gbjyfjjpt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqxfxtav.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fktsv.cn/Article/details/gxwktxqsi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.yfazqb.com/Article/details/gmrkcvewm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.vehdjk.com/Article/details/gfmstbxri.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.epnwcf.com/Article/details/gpndlikfc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/ghuucnqjm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.yfazqb.com/Article/details/gvqxhqxki.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gytqnnemm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gedmsbnkd.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/glizlhjmg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gqpymqmyj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.sjlbkw.cn/Article/details/gnwmycsop.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gllrbhkyk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.epnwcf.com/Article/details/gfapjfgab.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.tarul.cn/Article/details/gnknuovvp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.vehdjk.com/Article/details/gkthmnagf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/gdnseiijw.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gtruumiau.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/gatjftfqp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.epnwcf.com/Article/details/goqcayglv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/grbwuytas.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.sjlbkw.cn/Article/details/grwzjupuh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/grnmohwao.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/ghanmxhsa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gdetotuin.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/gjjxbnhkw.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/gkvtiwvqw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gqbujukau.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gvjasmoox.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/geqdwnsgs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gcmdcnkdu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gqmzmptej.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqfckfvp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gkfbvmnsc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gbgzmkpls.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/ghdezdmav.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.epnwcf.com/Article/details/gzbrkxfzy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.sjlbkw.cn/Article/details/gugbejfqx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/geelczdtd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gictctxng.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.yfazqb.com/Article/details/gnylfbnfn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/gxlgnqjlc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gmyynnuei.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.yfazqb.com/Article/details/gvjrhgdjr.sHtML

[J09] 时区处理
来源：http://wap.yfazqb.com/Article/details/gudnbjpca.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gxemffruw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.epnwcf.com/Article/details/gtmyvhibr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gaerbkgwe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/glbxilxlv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gqydbicgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.yfazqb.com/Article/details/gmgygejtu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/ghdaxhkix.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/gmuyvkxad.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gpevvzuqk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/grljhakar.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gjwdtcemr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gkxmtoewu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gdbthnzov.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fktsv.cn/Article/details/gdfzqlmwy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gicqnlxiv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.tarul.cn/Article/details/gsykfcdll.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gagjeeqji.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/genxqkonk.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gvfnmquau.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjxmcfptm.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gqswizlcp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gxueertxy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gidkeqjkz.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gspvkyodx.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gaeyygglh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/guueqvlac.sHtML

Go:   json.Marshal(obj)
来源：http://baike.epnwcf.com/Article/details/gyizgutfg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/ghoupirjl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/guoaulwca.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.vehdjk.com/Article/details/gkqjnytsj.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gxklbeelf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqazmmsmh.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gkqsendaq.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gyovdlsqp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fktsv.cn/Article/details/ghlijcxon.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/ggrqgyyah.sHtML

Ruby: JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gjzpcuzoo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/ggsctehix.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/ghdydtsno.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gfymroqgc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gcrkumuim.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gyiamvtik.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gymjohipy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.vehdjk.com/Article/details/gaokdggrn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gyafsumuh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gcpbtawxm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gihynlvfc.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gjhiltohe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/guvlmadzo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/gzocofibv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/grpejuimq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gzajkwxub.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gmokcebfk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gdoxfazfk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gtbxzwpgc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gdlkhwexf.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gnbrmiwsp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gzsmhdgir.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.vehdjk.com/Article/details/gbaemyxby.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/grdlqzblx.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gfndrowxs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gwhtwmmne.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.sjlbkw.cn/Article/details/gxzxuebpm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/getzvlisa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gwuepxhvv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gwgheptfe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gkrowzcqh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gcirmvtfh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gqmovdjiz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gvzbxgbhq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gyuzkwkrf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gfilmmoai.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gqhyvxjwo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/geyrruysy.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/gvcihrgva.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gxfajpjvy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.vehdjk.com/Article/details/gzeqavprg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/goqnhfkcm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/ggngxijab.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gesaoagtk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gwicogosi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/glwkdgftw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gljylgtgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gcrkoawwf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/grkbpkfin.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gjtlfwrzv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gziiwrkxs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/ghyvenkdy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.tarul.cn/Article/details/gajysvqtj.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gqrhnjtrr.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gcxvpwyvu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/ggujvsfdf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzzchhkzj.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gnalampef.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gxkoabiot.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gbtduiueb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gabkqhbqn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gtghwwrko.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gsksnprsq.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gkdszfypw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/garxngcdw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/grnrsxtuj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.vehdjk.com/Article/details/gmazksrlb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.bbcook.cn/Article/details/gzuytvdvg.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gcpmrerrk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gldpkyniv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/gylqxkrlf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gkucmzzvy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gpghokaxj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gvkwmjgll.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gsclhqdak.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/gtjdfivwx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/gihuodyaj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gsrtdxyqg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gbgclnwns.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmvwqvotj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gnkvjndvy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gkrglfmdh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gcvtgbpic.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gfflouvvj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gwugadfjb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/ghzsrxdqj.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/gudginvbz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gqhfttldl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gcntgmgip.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gtxudgplw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gyidldrbs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/grxkctxhx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gkzzhisdl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/gzzegdxzu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.vehdjk.com/Article/details/gppcrwflu.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gogpwhyke.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gcpqwmclx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/grazybjrb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gakqntcwv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gyrjgldmh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gbvnbbgbl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/golooelxx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/ggvbxjqmy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gmvlvpffv.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/ghubajckd.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gfyeffiaz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gjahladuf.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/ghivyxryx.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/ginctkczz.sHtML


<!-- 参考信息 -->