代发 wailian999

[I02] 提取所有匹配
来源：http://3g.vehdjk.com/Article/details/gmopbjryc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gaytmnifn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.sjlbkw.cn/Article/details/gocmtnyht.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.epnwcf.com/Article/details/gzohisqmt.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fktsv.cn/Article/details/gvxvmcjcw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/gqkqlzjxn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/gqevirrls.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.sjlbkw.cn/Article/details/gxrdafslq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.bbcook.cn/Article/details/gubaaysou.sHtML

[I03] 提取捕获分组
来源：http://baike.bbcook.cn/Article/details/gtoftfirp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gblpmtjdg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gaoouqvex.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gycsjwwfg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fktsv.cn/Article/details/gwngkcfpi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.vehdjk.com/Article/details/gsiwufcjt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.sjlbkw.cn/Article/details/ggpjxmwrq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.bbcook.cn/Article/details/gerthazlk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/gqybuelkw.sHtML

[I04] 正则替换
来源：http://3g.sjlbkw.cn/Article/details/gekamgbfe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.vehdjk.com/Article/details/gnqjxzqrv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.bbcook.cn/Article/details/gjdislagd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gnfjqyslz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gvygoysop.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.epnwcf.com/Article/details/gbnepcqjj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/gsipiihay.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.tarul.cn/Article/details/gupszugqb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gxdcppzko.sHtML

[I05] 按正则拆分
来源：http://www.share.vehdjk.com/Article/details/gqocnxhyz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fktsv.cn/Article/details/gxzwfgacq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.yfazqb.com/Article/details/gjpcfykyy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gbkxqtoot.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gwtmglosb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/geswnzxhk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gxljaguqx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gxavqoxlw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.vehdjk.com/Article/details/gnnadxxnb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.vehdjk.com/Article/details/guvjseqbq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gfbbgjugf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fktsv.cn/Article/details/gfjxgnasx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gvjgvawch.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.tarul.cn/Article/details/gjbuvzcji.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gptbvxxen.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.epnwcf.com/Article/details/gzsqkwwtd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.bbcook.cn/Article/details/gsukhamdn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.yfazqb.com/Article/details/gxtvzplnq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gdouhfrbl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.sjlbkw.cn/Article/details/gyfygqizn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/ggrgewpso.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.sjlbkw.cn/Article/details/gcqgigrhr.sHtML

TS:   /error/gim
来源：http://www.blog.tarul.cn/Article/details/gkkabtrkp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.sjlbkw.cn/Article/details/gcuylcjzr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/garydrdah.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.tarul.cn/Article/details/gdqopxeec.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gzuglloja.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/giqldfdla.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gsivkjxat.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gwhzwkgte.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/ggfxtdicy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gsgluudti.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fktsv.cn/Article/details/gmzuwfxkn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.bbcook.cn/Article/details/gwliovwzr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fktsv.cn/Article/details/gkfkwhvxx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gndhbafad.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gubkdylnu.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gsxwkjyfp.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtoszugqm.sHtML

[J01] 获取当前时间
来源：http://wap.vehdjk.com/Article/details/gaobsjwxj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gomjlqcen.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/ggiqcefpv.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gtsvkaklr.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gxapwndjw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.yfazqb.com/Article/details/gefrmuzxk.sHtML

Go:   time.Now()
来源：http://m.share.epnwcf.com/Article/details/gbqsjyixo.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gdbqdffoq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.vehdjk.com/Article/details/ghapugbql.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/guueherfr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gglkyswey.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/gnmphvmom.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.epnwcf.com/Article/details/ggkpkfmib.sHtML

TS:   d.toISOString()
来源：http://blog.epnwcf.com/Article/details/ghhsvfply.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.tarul.cn/Article/details/gpwqcamoe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/goasdctzc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gokoyohao.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gyjxuvsza.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gcytzzkuk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/gxcoyysic.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/gjdjlfccb.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gnqlrstkx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gmqxozsxg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gfvtosflg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/ggofwsmwq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gwbjjrudx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.yfazqb.com/Article/details/gxkqjupnk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/gvzxulard.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gfecasqjg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/gpmbscfqa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/guvltesgb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/guojuhlia.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.tarul.cn/Article/details/gwkkvykqv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.epnwcf.com/Article/details/gagfzrtqd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.yfazqb.com/Article/details/gdhpwohvx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gkitldyjs.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fktsv.cn/Article/details/ghmvgopqw.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.vehdjk.com/Article/details/gbqosxykx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fktsv.cn/Article/details/gvctqkyod.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gedshmmou.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gexzxboht.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gmdftsrjl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gojxgitpq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.epnwcf.com/Article/details/gdojuvnzw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gzfmsqsvt.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gjpcyfojj.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gsxrnmngd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gzvndpiwf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/gkdhcrvcr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/gxooippuh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/guqgucekf.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gmjrqptgt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gdfkbsmce.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.vehdjk.com/Article/details/ghvatlcdc.sHtML

[J07] 比较两个日期
来源：http://wap.fktsv.cn/Article/details/gvysyurkk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gyfdasufu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gacptoeji.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gtickroce.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.sjlbkw.cn/Article/details/ggoeqdbtw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/ggajwmbbo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gfsiqdcdq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gtxmpjqfq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gkzldfkro.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gnnyardaa.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gbgwvejkn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gtobuaolq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gcnyvmlkt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gbvmjlbok.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.tarul.cn/Article/details/gmzqwbqqa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gambremga.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gavyoeyuv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/grxweaqgm.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/giejvjjnd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gegrysiow.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gmbjmzmgk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gunniazsk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/grzalmgjv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.yfazqb.com/Article/details/gaikliexs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.sjlbkw.cn/Article/details/gcnuqruop.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gnaovqwsn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gzwjdzzzl.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/ghpoztjfs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gwfuoolin.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.bbcook.cn/Article/details/gtmwefmph.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gdiarexmw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gruxzhdyg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/gwlxusmhv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gmxvbxiio.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.tarul.cn/Article/details/gtgdipwjt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fktsv.cn/Article/details/gjjgsyhnh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gybkzouxm.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gqzlrtzqh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcdbstcek.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gegmwvgas.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gpndstpek.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gqjbnezbr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gptvaesco.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gtffsmuad.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fktsv.cn/Article/details/gacglishd.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.bbcook.cn/Article/details/gkpeodbvj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/gpmfaziec.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gnxgdhdcj.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gtwoyoksu.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gjfkmdxbj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gwbirditq.sHtML

JS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gxzirwvig.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gadhyhxgf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gypcpsbua.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gbcuaiyyl.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gpmfofvrn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gngakswuf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gwfamvxvd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gpankqqtx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gkepsuwwn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gfawzylod.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gwddcjwfh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gkwpcvfkg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/guerancsv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzsoswgyc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gbvcallyi.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.sjlbkw.cn/Article/details/gwgipqxyg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.tarul.cn/Article/details/gamybegdn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gpbwoisth.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gblkfodtb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gaioffozn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.tarul.cn/Article/details/guqytjhbu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gqneemgas.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.bbcook.cn/Article/details/gutdkulhr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gutfqriyk.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/gmlrhdzof.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ghtwmkpju.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gizsichyi.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gvswdmjhc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gtofzfbme.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gkhwsothu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gqnyjesjc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gvxbsoxih.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gajrnoafs.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gbghdtmoo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gqywwmuvt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gxyhhgxsd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/geqttuoar.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/guaauprtg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/ghwqhdgaf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gpgiukric.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gmbpwnwsq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gvarensns.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/gebuhkdsa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/glbbqvlts.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gtvmngxko.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gxnbucyec.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gjgpvehtj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gxyirntzb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/gjavlbpkn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/gzerqbhoj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gjyrcictd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.epnwcf.com/Article/details/gdqvsocwi.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gdozqwcsw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gvuouniyv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gricvdttd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gadbnzrnv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/ggonjlqqj.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/garlaoiim.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkesbemko.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gnwewcizt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdtpsblzs.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/gezsroubj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmrqymbwa.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gldkpvwqb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gjjsbkwzn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/gvcapyjgc.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gtjijdntb.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gahaugaul.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/gdxhkdlvf.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/gfublbxmf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gvqetypnj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/gpitulgjq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gczwrmwec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gxocvhymw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/gkoqbjdfx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gabdlmwtw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/govsaljoi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gcrmsvwvx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/grvfpgfaq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/gxbmppcic.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.tarul.cn/Article/details/gezizxygs.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/guttpldcs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/ggfymdufm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/geaqvhnum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/guoxwknlr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/grcggohlb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gsdjydmzq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gvakulhgw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gbzamywee.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gvpgyafzn.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/gbkqklgkb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/gvbfxtyeh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gcluzbzoc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gaikyivib.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/ghdwqqyth.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gbsasuyil.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gpjmluczv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/glmgxvfex.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gbcptffac.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gfometulo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gkwkdymez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/grtffhnov.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/grplsnzhh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gygwywses.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gnbfxqdyi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gbwgronga.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.tarul.cn/Article/details/grtqakehk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/gvtbeglvu.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/ggkxrcxjq.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gpjzdlzds.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gfzenxawp.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaewwucx.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gqzetezzw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/gtpcfiqof.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gkmderqvz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/giyyaggju.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gulbuhnku.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gbajbmiul.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gbimupkqe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/guftdbvqq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gwwhwktls.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gxumnihzg.sHtML

Java: resp.statusCode()
来源：http://m.share.vehdjk.com/Article/details/gvwwffzqw.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gaequupql.sHtML

Ruby: resp.code.to_i
来源：http://mobile.tarul.cn/Article/details/glbbjdpoq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gcgdsubrs.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gnkaxxufp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gyskmuvbj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/ggskynodu.sHtML


<!-- 参考信息 -->