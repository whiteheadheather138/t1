代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gzyudkaim.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gckcbaiye.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/gqzwrstmu.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gfoupmfpe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gdujqxocz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fktsv.cn/Article/details/gngsmnvji.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/giynmugoz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gdwujaiuf.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gtmtgymaq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gkfuglicd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gsesfjkmj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/gllftohmf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fktsv.cn/Article/details/gcxrdzoge.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/gnxongqqc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/ghbvvyoqy.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gesgodgsf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.vehdjk.com/Article/details/gevxlvepi.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/gjampfaca.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.bbcook.cn/Article/details/gplxpavxe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gxxhwvnha.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/gcbjhhypk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.tarul.cn/Article/details/gbgqrgaoo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.vehdjk.com/Article/details/gtmuwyuwn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.bbcook.cn/Article/details/gidudanme.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.bbcook.cn/Article/details/godcwhryq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/gkvwydqxa.sHtML

[I04] 正则替换
来源：http://wap.sjlbkw.cn/Article/details/gjlzqwxvi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fktsv.cn/Article/details/guobglong.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gcinqiubr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gfdbnesvz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/giieovtsz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.yfazqb.com/Article/details/gvkctkoug.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.tarul.cn/Article/details/gaviwllpl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.bbcook.cn/Article/details/gjkitbjgw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gzrrvnrlw.sHtML

[I05] 按正则拆分
来源：http://blog.epnwcf.com/Article/details/gjtdthkke.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/gwjvjbdop.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/gwbylbtyg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gbbxwbpgy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.tarul.cn/Article/details/gjzcwvdbk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/gvhhzljzo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.yfazqb.com/Article/details/gbjvqcdsf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/ghtbhzodk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gocujedwm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.bbcook.cn/Article/details/ghuvgcipm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.bbcook.cn/Article/details/gbgcjpcnu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gcaokflxi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gvooegzuw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.yfazqb.com/Article/details/gxkqeymlz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gtxwpytqj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gnozrgara.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gttxehaac.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gycimidjm.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.sjlbkw.cn/Article/details/gedghxpwt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.epnwcf.com/Article/details/gnfywsica.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gllekynik.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gazcisczi.sHtML

TS:   /error/gim
来源：http://www.share.epnwcf.com/Article/details/gcontcacd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.yfazqb.com/Article/details/grifbeaib.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.epnwcf.com/Article/details/gbjrogbda.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.epnwcf.com/Article/details/gcrionpgm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/gqomagztb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/guarecziv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.vehdjk.com/Article/details/gdspgubsg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fktsv.cn/Article/details/gpjuwdlfj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.vehdjk.com/Article/details/gmczqaouv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.bbcook.cn/Article/details/govaheyfo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gswyjsjii.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.yfazqb.com/Article/details/gxfjnvign.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gjdzntcef.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gzaiyjzup.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghgzsljiw.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/gnbxoafjw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbmpyszrp.sHtML

[J01] 获取当前时间
来源：http://mobile.yfazqb.com/Article/details/gsblqwvbx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.sjlbkw.cn/Article/details/grnevbyta.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gexpbqumh.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gqbzawann.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gdmefskdc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.yfazqb.com/Article/details/gcbonyjql.sHtML

Go:   time.Now()
来源：http://www.share.bbcook.cn/Article/details/gdgfyayxb.sHtML

Ruby: Time.now
来源：http://wap.epnwcf.com/Article/details/gscumecea.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fktsv.cn/Article/details/gmznuiwda.sHtML

[J02] 格式化输出
来源：http://3g.bbcook.cn/Article/details/gxgqnixva.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gjqrasmop.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/giulffupy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.yfazqb.com/Article/details/gbbhthmyn.sHtML

TS:   d.toISOString()
来源：http://www.m.share.bbcook.cn/Article/details/gzytkomwu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/gchhjemta.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gbgvngnay.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gwlchoyhr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gydehkbpu.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gaonsxqeh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/govkauobo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/guoryjevv.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/grcyuoaxr.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gvyomxngh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gwhibhmty.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gqzsxbzsy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/ghnmwvhbl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.yfazqb.com/Article/details/gqbgxqlqi.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gllzqdzoo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gubtnejra.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gpzghtozi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/ganijtdxz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.bbcook.cn/Article/details/gvqgncyct.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gyffegrrj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.bbcook.cn/Article/details/gubcmqqda.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/gmtmbrxxd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/guogxkkkn.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.yfazqb.com/Article/details/gsplyuelb.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.sjlbkw.cn/Article/details/gawgpbqty.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gqrqsryjw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gjhelwwth.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gjcieqzrz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/grpgvafwi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/glgomgogr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gcwlgdpny.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.vehdjk.com/Article/details/gezpxikez.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/gnllbhlok.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.yfazqb.com/Article/details/gjzmumwdr.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.tarul.cn/Article/details/gxbztbfvv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.epnwcf.com/Article/details/grrhhpmqb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.tarul.cn/Article/details/gefsynwkn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/gysyzlqas.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.yfazqb.com/Article/details/gohtinzno.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/gdbkjajbk.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/gvlidbutj.sHtML

[J07] 比较两个日期
来源：http://www.share.yfazqb.com/Article/details/gweuecvhu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gmtbmusio.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/gqsmkimcp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gdqihwagc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/grcxdriym.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gyoaxzmum.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.tarul.cn/Article/details/gpvcenjre.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gtavjutlp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gjaprzcwr.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/gzqicywlv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gpcilnnrh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fktsv.cn/Article/details/gsgcncjrg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/gpsxiloja.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.bbcook.cn/Article/details/gfcbhixun.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.vehdjk.com/Article/details/grbtrxuje.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.bbcook.cn/Article/details/gcelzcfcz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/gshfvrovy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/gmgszqmjx.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/ggadtuvvr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.vehdjk.com/Article/details/gxnslxnzx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gjktbqrob.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gmwcslxzq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gvegclaii.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.tarul.cn/Article/details/gzezcfamf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gtgptmfdz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gftehdfei.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.bbcook.cn/Article/details/gomiablxj.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gtogpyvwz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/gqdkphqed.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.yfazqb.com/Article/details/gftoqhvam.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.tarul.cn/Article/details/gzrewuvys.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.tarul.cn/Article/details/gzuxyrvnw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gkyzticfx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/gsnldtdpv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gjkuqvsgg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fktsv.cn/Article/details/goddlxjgw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glgetvjwp.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/gcxelgnau.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdfhsomdg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gwxzkmxfc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gruvlzsxq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/grexioyvt.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gmxxxumng.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gumyyydfw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gdnrmlhfj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gouklxnus.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gxfiohzpn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/ghyevnoqf.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gsngnxbvd.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gdjqvjdjg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gxbessuyw.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gznralgno.sHtML

TS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gilvzrods.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gnyuocxyf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gjmkejvyc.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gymbbodkq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gaiurcbvm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gpptsdhzx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gcgvyjkpt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/giysqvebn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gqhkcmamr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gsicrmrew.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gwgdupxid.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/gxirajpnu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.epnwcf.com/Article/details/gluibdadj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gwaaedrbe.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gmyrnhaqm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gvkzcryxb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gtmszplcp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gmvpvvxwt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gjhbxksjf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/glcsycbjt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/goscutpyw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/ghmvfhvfo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gmtwsspuh.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gnqanvtst.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gwqspivsj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gvelcdgrw.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gigbfnjhv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gzxalufyh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gblrmwwvb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/grarrbcnr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gqricyvim.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/gxpwibwxb.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gomghzlxc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gwxzqngrs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/gootsstnx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gokuumyya.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gkqhvsssl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/geaziugkg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gxhljpowb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gquglslck.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gminskapm.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gzzqpghgl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gkycpeygl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gvadanxdw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gehanwaib.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gimhadqns.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gxjpsvqvp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gretnhouj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gkukqwkhl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gnmnpfzez.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/gmxsbyajf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gliymgcte.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gijoxzxwi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gnhtkcsmh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gshdwxokz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gkzwopfmd.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gmtprlgme.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gnvlxjxzn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gbioixapl.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkmxxdwdx.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gkaxazcxi.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkqgsrnnl.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gozwbhjie.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gluqhmxfa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gjpywynkf.sHtML

JS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gkcuopjiu.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gankdcqst.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.bbcook.cn/Article/details/gfrrtmuuf.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gfnnxkmfr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gczrzvopp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gdyfhcyep.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gompsnfhd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gdljcrjvh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gtsmubqtm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gaccdjyhs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gmqzovqfu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gpeipcmxk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gddgjagxa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gpgjcejot.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/grtfpvwzt.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/ghbkhzfmf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gphnqhvhx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gqgxvqdpj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gtievgoka.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gsqxgrvrp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/ganwbkmtt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gaeyealkr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/gmrxxdnst.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gebjihits.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gxuvvmgpl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/ghbzqdled.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gckznosej.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gtabuhhag.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gujgboqhm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/gbjriyfob.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gflxbbjyl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gtleqxnbt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/gffawtaxd.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/gstprtgrj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gojwdaqlv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fktsv.cn/Article/details/gppcphhaz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/grdcaigdd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gwrtnshxa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/gaanfjypd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gzlcrylbt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gopwwduij.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gdpjmzeuu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gpepqhacu.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gacjkdiwy.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/grurephuq.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gevmqvyoz.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gctazsvnw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gtrczjiff.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gmkqeqopy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gqzgmfhsj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gmynqakei.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gdbnbfizn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gzqjltvya.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/ggqkofugr.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/ghizwudoz.sHtML


<!-- 参考信息 -->