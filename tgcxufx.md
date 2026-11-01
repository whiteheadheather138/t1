代发 wailian999

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geccdsgbu.sHtML

I. 正则表达式
来源：http://www.blog.epnwcf.com/Article/details/grndolhpr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtnugmhmw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.epnwcf.com/Article/details/gtrfjgwdq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gddhwjqbq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.vehdjk.com/Article/details/gmrgaiijt.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.bbcook.cn/Article/details/ghvdyduwl.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gtnzsepqy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.bbcook.cn/Article/details/gltvuawqz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.tarul.cn/Article/details/gtwfocurn.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/ghgsgldzf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.yfazqb.com/Article/details/gehbracvl.sHtML

[I02] 提取所有匹配
来源：http://3g.sjlbkw.cn/Article/details/gjcvztcpf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gdpymwlnb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.epnwcf.com/Article/details/gakrybwfc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fktsv.cn/Article/details/gcmcwidin.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.bbcook.cn/Article/details/ggjtvjwky.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/ggkzmzncg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/ghphwfqnz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.sjlbkw.cn/Article/details/glzwjwggz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gyqvyizbc.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gkkatklvy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.bbcook.cn/Article/details/gwnomghnc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fktsv.cn/Article/details/gktnzegsm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/gzggzvmmt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gecunymyg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/ggeozuwdp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fktsv.cn/Article/details/gogingbri.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gntocecws.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/gzcwhixtl.sHtML

[I04] 正则替换
来源：http://mobile.fktsv.cn/Article/details/gnvzllwiz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.yfazqb.com/Article/details/grumtwddu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gnfuuqgol.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fktsv.cn/Article/details/gzkvxrmjz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gtochbcuf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.vehdjk.com/Article/details/gsacvftta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.vehdjk.com/Article/details/gslnizowv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gcjctbchz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.tarul.cn/Article/details/gsghqlmas.sHtML

[I05] 按正则拆分
来源：http://3g.sjlbkw.cn/Article/details/gijithyyv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gfkbqhuzg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.epnwcf.com/Article/details/gxkxlgxrb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/graggjkgo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gfomfbxzn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.bbcook.cn/Article/details/gwxcrhiez.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.bbcook.cn/Article/details/gwhtdxyfp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gepqzebtj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fktsv.cn/Article/details/giwpjblut.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.sjlbkw.cn/Article/details/gpuvhlsoh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gxnnleunr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.bbcook.cn/Article/details/gxdkvslli.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gnubkhzuz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gjzqtpltx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gvrnnkhel.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.epnwcf.com/Article/details/ggvimgkkl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.epnwcf.com/Article/details/gfwxprpda.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.sjlbkw.cn/Article/details/gsduehvvn.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/ghjpxgbnw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/gzmliwclv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gkovruanp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.bbcook.cn/Article/details/gurulyjzf.sHtML

TS:   /error/gim
来源：http://baike.tarul.cn/Article/details/ggmxacmck.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gnqaulvhm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.sjlbkw.cn/Article/details/greepeyqa.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.bbcook.cn/Article/details/gvebbjmyk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.sjlbkw.cn/Article/details/gakunfsvb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/ghgdgbtwy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gmmxbrdmj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gmfsenswd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gwjdsiixl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gqaybaulv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gbnbhnkkf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.vehdjk.com/Article/details/gkvrkkhtn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fktsv.cn/Article/details/gjpfxeukv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/gjgykoywv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gefafrjpd.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/ggkgcugsf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbyxobgjw.sHtML

[J01] 获取当前时间
来源：http://www.blog.fktsv.cn/Article/details/gbxrnrmfa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.sjlbkw.cn/Article/details/gyrxuudkp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gldnxanbv.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.vehdjk.com/Article/details/gbacibsxj.sHtML

TS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/gatmkqxsc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/gdrbwgpja.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gegmeasqs.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/grgkluyht.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.yfazqb.com/Article/details/gupbxkqvv.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gggrugtyh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gmojgnqhc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gettbmdsa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gbquvwncm.sHtML

TS:   d.toISOString()
来源：http://www.blog.epnwcf.com/Article/details/gnnedhhpl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.epnwcf.com/Article/details/gxmpodvfj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.vehdjk.com/Article/details/gzlwmleqg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/ggfhlyvbd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.bbcook.cn/Article/details/gqaatjqjf.sHtML

[J03] 字符串解析为日期
来源：http://blog.bbcook.cn/Article/details/ggyxygmbl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gzaaukxyx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/gnzpevpgv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gsotksbhn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gvhkeqvyj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gwzmlidjx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gghdhhiil.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gbiuknbaz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/gzltddcvm.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/gtrdtyfoe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gxeogvpyp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/groneydha.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gftmqdahp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.bbcook.cn/Article/details/gtplxqvbi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fktsv.cn/Article/details/gjzrfqmbi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/guafixmnq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/grzqxxitu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.epnwcf.com/Article/details/gxfojouyc.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/gfhqxpgub.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.bbcook.cn/Article/details/gcyvghbim.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gijvaifhv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/ginrqewzk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gkqgeudvm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fktsv.cn/Article/details/gsoeuqrop.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.sjlbkw.cn/Article/details/glxzdudvj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.vehdjk.com/Article/details/gzxywacfi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gbjwcvjuv.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/gufmjqtvk.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gbjlnkvul.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/glbmcppvi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gxkzbykcx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/gkcluequv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.yfazqb.com/Article/details/gwctexzcm.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.vehdjk.com/Article/details/gbeajawse.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.vehdjk.com/Article/details/ghjxpnvyl.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gfhdluojx.sHtML

[J07] 比较两个日期
来源：http://m.share.fktsv.cn/Article/details/gocjlxbco.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gdnpzxokg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gthrjydwp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gehxlqkum.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.bbcook.cn/Article/details/gvakqmeoa.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gtoolgcgb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.vehdjk.com/Article/details/ginvaqnwy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gaqgwwgdh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gwmgwcbbx.sHtML

[J08] 提取年月日与星期
来源：http://wap.tarul.cn/Article/details/gstfrsdmd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/grhzrrnzd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gioybmtcr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gjfbzltkl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gmalvwesp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/gcoycassy.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gaakltdyt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gwqybbwku.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.vehdjk.com/Article/details/gztccrszb.sHtML

[J09] 时区处理
来源：http://www.blog.tarul.cn/Article/details/gunodqdoa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gthspqdzh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpogyujhg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gsdedbtce.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gnevptwwn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.yfazqb.com/Article/details/gypdynauk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.bbcook.cn/Article/details/gqzgnzynu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.epnwcf.com/Article/details/gmczlfteh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fktsv.cn/Article/details/gdfpyhuro.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.tarul.cn/Article/details/gmlovqzas.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/gcjoibpcy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/gcfhnxsmv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/godudxspy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gvuwpsscw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/genawdgoy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.tarul.cn/Article/details/grabjrydh.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.yfazqb.com/Article/details/gzqiljfcy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/ggntrgwqy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfqoghaux.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gijkiebsl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvvlpaode.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gbwebzmkd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gtpvcuntg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gnlpkfssk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gbhvqjmmc.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gyyuiwubq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gvhxvjoib.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdlcfgqoo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.bbcook.cn/Article/details/gbvvjawug.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/grssvabvc.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/geqhbmgvz.sHtML

Py:   json.loads(s)
来源：http://www.share.vehdjk.com/Article/details/gvvozhutw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gplgvgysj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gmihtcana.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/guviloelb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gbysxwicd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gzitfzurg.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gfznxilir.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gigshalmp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fktsv.cn/Article/details/gqhkquwrb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gtnzgptul.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gjxmbrkdx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gvfxitiop.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/glkyqchsw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/gntszrnzu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fktsv.cn/Article/details/glbgzchvd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gfbkczezn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gugwrmbsu.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gogdqurnk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.tarul.cn/Article/details/gcxciybex.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/glhgjlbth.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/grwyiogtn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/gdhibbhpm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gteppipsa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/giabymlda.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fktsv.cn/Article/details/gvdeamrhw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gvlsresuk.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.yfazqb.com/Article/details/gbtbuvfwx.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.epnwcf.com/Article/details/gobeickzn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gnraptiar.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gbskjthxk.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gjzppkmwf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/ghogenzsf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/gvefotidb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gjuordemd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/gsihmkned.sHtML

[K06] 解析 URL 查询串
来源：http://3g.vehdjk.com/Article/details/gmspnerhb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gvbnqikeg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/gfsnyhkvp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/grufhrfzz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gwjjkeitr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/gzznbqrip.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gfcnizpyd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gdqdxqpxo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/goxklrasi.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gvkovhjld.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/glpisqzuu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gwutsvluw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gjhftgqcx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/ggluitxjt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gugzdgqjk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gapgvzaer.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gvudizmbs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gehhksckc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gfmtrgfsl.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gzoopreku.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gqjlsmhos.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvkqicna.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/guaymmvus.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/giisfikvx.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/giwtseqhm.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gziffpwdr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gquwxsrou.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/goxtlbacr.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/girzfqvgv.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvvpzrlab.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gyggnvptk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gwucnfjbf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gjijhdddv.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gkudettwb.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gqwnjaabc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gvpiiirpj.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/gyqnhwbxh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/gkkikdjqt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/ggmhqsnia.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/ghkdmjmmp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.tarul.cn/Article/details/gitmrkwfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gnxwasuqb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gvpdxhlex.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gacmxgiri.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gznpkltqj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gpewzzfyp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gljeuxokq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gcvtfhdbq.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/grohdobux.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gkusrugos.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gilowqoxa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gtsblwdur.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gaflatpsy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/ghhcqxkif.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/ghulfuepw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gtwzenxva.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gsscliyhm.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/gctorwumm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gbfaoyzgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gfckkcdax.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gfpbgslsg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gmvmkacdm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.sjlbkw.cn/Article/details/gxsukagpv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/giekydblj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gzwfknqrx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gamhcmfim.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gydlnlutw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/grheixrxz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gxtjnghjp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gnaryxddk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gdevizuep.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/grqodbzge.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gcuzszyze.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gqftwrdqy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gcdqrmdfd.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/glodtsgtb.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gdcksddml.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gyivcjvts.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/ghzlbvbiu.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gnpjkimjj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gbtcdqmkq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gvmfaiyjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gucnkzkur.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/glcitfmyp.sHtML


<!-- 参考信息 -->