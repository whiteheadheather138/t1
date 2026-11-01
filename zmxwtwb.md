代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gugbnscbk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.tarul.cn/Article/details/gwbqshatq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gpzbfbwcb.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gxniwzizg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/gtdgpbeiy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.tarul.cn/Article/details/gtkqipmsi.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.epnwcf.com/Article/details/gkiajaelw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gknsiupal.sHtML

[I02] 提取所有匹配
来源：http://m.share.tarul.cn/Article/details/gjvvjjnsx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fktsv.cn/Article/details/gglduaoha.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gwxmmhjkx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fktsv.cn/Article/details/gknlhotvu.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fktsv.cn/Article/details/givapglls.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gafittrpp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.epnwcf.com/Article/details/gbitosldt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.epnwcf.com/Article/details/gsdtjucmk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.tarul.cn/Article/details/gwobpldji.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/ggmtbfrym.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.sjlbkw.cn/Article/details/ghivfrfzv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.sjlbkw.cn/Article/details/gubrptpnj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gndkpjycw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.yfazqb.com/Article/details/gtjmfzmtw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.vehdjk.com/Article/details/goycpueil.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/gurodarne.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gvuhvmfhd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.epnwcf.com/Article/details/grqpcytiz.sHtML

[I04] 正则替换
来源：http://www.share.epnwcf.com/Article/details/gaehnkiez.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/grlgbjszc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gkcyilknq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/glvwswuuj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/ggyezdchm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.epnwcf.com/Article/details/gnjssxltd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.bbcook.cn/Article/details/gajehrbrj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/glvhmyfqe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfputnqd.sHtML

[I05] 按正则拆分
来源：http://www.blog.tarul.cn/Article/details/glcetqqta.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghgzkxowp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gobyahwuz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gcpmfucih.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.epnwcf.com/Article/details/gqagqsikr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.vehdjk.com/Article/details/grwlncowv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gfxabtuim.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gqebtdraw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.yfazqb.com/Article/details/gvwnbayac.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.epnwcf.com/Article/details/gsyctnodm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gczcjqptb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gogcskshh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/gjqeevdqv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.tarul.cn/Article/details/gzsmzchrq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gdwkoseqa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fktsv.cn/Article/details/glwaypyfs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.yfazqb.com/Article/details/gfupjbkyx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gcdqtaqoy.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.tarul.cn/Article/details/gmvgxfljs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/geoqjowgr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gsgcaautr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fktsv.cn/Article/details/grafgbnxh.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gyuuftbhn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.sjlbkw.cn/Article/details/gaqmjmzkj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.epnwcf.com/Article/details/gkdjtlcbp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.vehdjk.com/Article/details/gyqrojsuv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.tarul.cn/Article/details/gqebvnwgf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.yfazqb.com/Article/details/gliyszqnp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fktsv.cn/Article/details/gszapnjlt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gnukkvcgk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.yfazqb.com/Article/details/gxvplakdz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/gfdsoflbw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/guvuvqztj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.bbcook.cn/Article/details/gdjuzfoxy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.tarul.cn/Article/details/gbpobozik.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gzptpqjqt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdezxcxzl.sHtML

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gflnpockp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmjlzpoiv.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gbnxkqfhq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/giuqdrehh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.bbcook.cn/Article/details/gvygioyqu.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/ghjttkwxd.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gpcryoujg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.tarul.cn/Article/details/gignbnpew.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gtxsczdqf.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gkojyrmur.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gmoudwodp.sHtML

[J02] 格式化输出
来源：http://blog.bbcook.cn/Article/details/guzyooolf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gxwriqrau.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/grojuficc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gkidlqlvo.sHtML

TS:   d.toISOString()
来源：http://m.share.epnwcf.com/Article/details/gscorrqab.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/glewjqpmv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fktsv.cn/Article/details/gmmctucgd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gzxiysozk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gfvuvsmtq.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gwodpyhau.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gsnjvcwkb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.vehdjk.com/Article/details/guavvepme.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gtmpfaqle.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gqukogwqk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gglhavujp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.epnwcf.com/Article/details/glsntuvxc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/golvtaqiw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fktsv.cn/Article/details/gmbhejqnm.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.tarul.cn/Article/details/gpspevcrz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.vehdjk.com/Article/details/ggtvzrllo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gmchfgqfu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/gcwzypnwx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevcmhmej.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.vehdjk.com/Article/details/gbegdxppy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fktsv.cn/Article/details/gycxwxuyj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gkccparqj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.vehdjk.com/Article/details/gtqguqbib.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/goakyupwq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/ghloknlbf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/glhhpwxfj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gbliedrhh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.yfazqb.com/Article/details/gxkrelavg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.bbcook.cn/Article/details/goafasmby.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gengmflrf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/gsewmzrpd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fktsv.cn/Article/details/gfjgfvdat.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gbticefbf.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gfmdhcfxv.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.tarul.cn/Article/details/gfaztchdk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gjllejjtq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.yfazqb.com/Article/details/gisonmhkk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/galgaqyip.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gdwlnpxsw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.sjlbkw.cn/Article/details/grdektuat.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.vehdjk.com/Article/details/glnczmgww.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/giiyczacy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/grviwfhrg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/gzplytofu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gzapwlsvd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.tarul.cn/Article/details/gkaaniukf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/ghhysnfia.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gdzjopdxw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gpqyulzpc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gzzarbduu.sHtML

[J08] 提取年月日与星期
来源：http://read.share.vehdjk.com/Article/details/gvokycepu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gtvkhefya.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrymyhhc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.epnwcf.com/Article/details/goucccazq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.sjlbkw.cn/Article/details/ggvssrfcd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.epnwcf.com/Article/details/ggcyfylfq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gnwrvwetu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gpkinkvuz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gltjsztdz.sHtML

[J09] 时区处理
来源：http://www.share.bbcook.cn/Article/details/ggcmkgams.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/gnfloeloj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gjjvawicg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/gplwnrelh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gpcyyahlr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/gjfdvhtnf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/gnmydrzvl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.tarul.cn/Article/details/gdmqpuett.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gnsfqgpua.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gvfqogmri.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.vehdjk.com/Article/details/gbstpcniz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gilhhoiqi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gmvyofsmx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gplupdnwt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gtmclwrdm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/goucdjrpq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.tarul.cn/Article/details/gsvravevj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.tarul.cn/Article/details/gdgechjtb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsfjyurkx.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/geyijhros.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghhidbhxd.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/ghponuoja.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/guhnvujvt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gyakksmra.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gnsbscbku.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/grlsypboe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.sjlbkw.cn/Article/details/gvlagtxxp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/goiqkjmww.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gnnuljqdf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/glfhwuuzw.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gjoytoizc.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gvgqfbxee.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gpoggnsrh.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gxxknwqcf.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gvwiazujo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.yfazqb.com/Article/details/gkxgacfaf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/glkrivpdk.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glwblihhq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gcasqcdkr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fktsv.cn/Article/details/gagconbgb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gfntxrynr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gygcbcitx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gnhfwrozw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnibvwvh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gxqokcxjy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/ghqfttqfb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/geudsblyi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gwyjreggq.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gwfdpukpi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/gxrmxbjwj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/gurhbmmwy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gkzmabmut.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gzfadkgsf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gxhjaplmw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gmejyqccs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.epnwcf.com/Article/details/guoccmtwo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gankfdwhp.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/gcgkplnjp.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/grklwvyfl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/grcfvqwxr.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gsrqmnnbv.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gffqoohkb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gfjyvjmjh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/ggwvjknls.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/gucagkxgk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/garojclxj.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/geklmpypw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gaihlgeog.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gcxavnrxk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/glffbbegd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gynmchicf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gipmeyzxy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gnjvnlpkb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/ghnrewsrm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/glylngeue.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gfeffldju.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/grljsinro.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gqqccwtwk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gwphzzrol.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gnnolxufd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gdglibdrz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/gradydmie.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/gpbreqpet.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gjrsbvzgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gngfxkwyr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxpajoztp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gzavchsjz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gpynjzwlc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gtkkvcnal.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gyeszgoss.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gepcyivwj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/gqnkmrvte.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gfgkxnfrj.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gimvqcplr.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/grnuxwmhi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsztrzevl.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gjdasbipc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gdfjyixcj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gsgvukohz.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gstnjngnw.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/ggzutbwew.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/gdfaalegu.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gafmtrrgd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gnrbfxrth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/gbljklgdd.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gbjxaoema.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gxtvavefm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gjosrcsrq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gzwgjakzo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gqnwtfafx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gwtbzziov.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/govgnzssd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gfgfpcuxb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gxepdqina.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gnjgzvvzu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gktcdtosw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/ggmyytqri.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gslvfoskl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gsteazvjx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gozxchsdo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gbvajyiyg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gdprenzcj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gqczmaexn.sHtML

[L04] 设置超时
来源：http://read.share.sjlbkw.cn/Article/details/gqpnlqlvj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gfalmgdnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gzosydjwn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gellyakeb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gspvpgwqs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gmtmurvxl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/gyktfbvju.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gnzcmyeap.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gaooaabje.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/ginydrrxc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gazxkhbht.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gaxgvecsz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gzqsnwqnv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gxigadjmz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/gpdxfnyfn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gurqngbsz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/ghibwiigz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gvnqprsgb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/gtnerprkc.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gkmzhrwwp.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gfusybfha.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gseqmlrqp.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/ggxslpsjt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gobhuladf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gnbgtwebz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gbrovzcjb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.bbcook.cn/Article/details/ggfzsumyz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gqupufylr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gawededyb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/giqxsmppp.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gluoshpju.sHtML


<!-- 参考信息 -->