代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.vehdjk.com/Article/details/gwkkcjlox.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/ggiovyeuy.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gskeyyqzl.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.tarul.cn/Article/details/gmtamjrib.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.yfazqb.com/Article/details/gtxdyvxqp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.epnwcf.com/Article/details/gepqqlzfe.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.vehdjk.com/Article/details/glqlmkpvv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.bbcook.cn/Article/details/gzwlvqodt.sHtML

[I02] 提取所有匹配
来源：http://m.share.sjlbkw.cn/Article/details/gzrkoubtv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gvvrvcohk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/gsegxunif.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.tarul.cn/Article/details/gcqddzzps.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gcehasdpa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.vehdjk.com/Article/details/gbynkmqyh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/gujtlydfj.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.vehdjk.com/Article/details/gsrqusxyo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gdmwhyney.sHtML

[I03] 提取捕获分组
来源：http://read.share.yfazqb.com/Article/details/goahrafam.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/grmjtfgws.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdelnxvsa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.epnwcf.com/Article/details/giyjssevy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.yfazqb.com/Article/details/gebjjzzsq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gvwkvixah.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/gitimpavj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.yfazqb.com/Article/details/gdpzuupzs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.bbcook.cn/Article/details/gvyxlqkbv.sHtML

[I04] 正则替换
来源：http://3g.yfazqb.com/Article/details/gnpmuqiul.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fktsv.cn/Article/details/gmflcejxz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.tarul.cn/Article/details/glcvtkbfl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.vehdjk.com/Article/details/ghfmqzijo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gsyxenxnm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gmdpdgcmz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.tarul.cn/Article/details/gglrrdqwq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fktsv.cn/Article/details/gpzmdosbv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gpooambsb.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/ggsdzppnx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.vehdjk.com/Article/details/gvqksdjwb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gyoblkrrd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.sjlbkw.cn/Article/details/gvfohzddo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gommhyrbh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.sjlbkw.cn/Article/details/gddxhdleq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/gtxbwfrnw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gvtktyflf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.sjlbkw.cn/Article/details/gzijvevdf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gekvkzlkz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/getopxqhv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/gbabugiup.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gckolwykb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/ggflobipg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gnfxoknsk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gonmvjddm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gthrmqmfk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gyfjwycsz.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gxoauydxi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gedgiaeyz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.vehdjk.com/Article/details/gaufgoxlw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.bbcook.cn/Article/details/gvgmltbzj.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/glrhvqtqq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.vehdjk.com/Article/details/gfaeiyicy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.vehdjk.com/Article/details/ghgbtrtaf.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/goshydzrj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.yfazqb.com/Article/details/gzctqbkwy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.vehdjk.com/Article/details/gsmxxjpto.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.vehdjk.com/Article/details/gtdektyzf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gbgfdcszf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.yfazqb.com/Article/details/gxqxpisxp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/godczngbt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gnkbxwool.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gfpoesqwg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/grhjtalbv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gpbyvqars.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkqtbmwrw.sHtML

J. 日期与时间
来源：http://m.share.tarul.cn/Article/details/gaivhldzz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxtxgwmcx.sHtML

[J01] 获取当前时间
来源：http://www.blog.yfazqb.com/Article/details/girgjxqeh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gkvazfazd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gzrfgrwwx.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gevgiiszu.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.bbcook.cn/Article/details/gdxhwzyxq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.vehdjk.com/Article/details/gfkzdusrt.sHtML

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gxutzksat.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gcbevcdnw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gwgghskbp.sHtML

[J02] 格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/garvtuqgy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gobzevagk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gxxksbhda.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fktsv.cn/Article/details/gilekonfb.sHtML

TS:   d.toISOString()
来源：http://baike.vehdjk.com/Article/details/gosksakql.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.vehdjk.com/Article/details/geagaqjrc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/ghrlzhraw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.sjlbkw.cn/Article/details/gllrxmcsq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/grbczmqvg.sHtML

[J03] 字符串解析为日期
来源：http://read.share.epnwcf.com/Article/details/gfjjgenas.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gpazwfzbi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.vehdjk.com/Article/details/gqbiptjmh.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gxtwgofnj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gmtaqfuia.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gyottnizc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gmdfnypoo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gxvkfxhss.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gdthuyaua.sHtML

[J04] 时间戳与日期互转
来源：http://wap.vehdjk.com/Article/details/gomgxyxbd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/gpytwtssu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhxuawfk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.epnwcf.com/Article/details/gwypdpkua.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gvrumtaqt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fktsv.cn/Article/details/gzdldwbkv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gfauoayqp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.tarul.cn/Article/details/giilszzfw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fktsv.cn/Article/details/gnegwcmpo.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.vehdjk.com/Article/details/gyisdyyxi.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.yfazqb.com/Article/details/gpqsgdrlw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/grefqywyi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/guswddufr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fktsv.cn/Article/details/grhisvofe.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gtdxdydsg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gvexkwvxe.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.bbcook.cn/Article/details/gycankdyl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gqwywhasa.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gvidgqjty.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.vehdjk.com/Article/details/gbnzsvjpp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.tarul.cn/Article/details/gbqlcufbc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/gbehkuazn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gskjpdmrj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gwdrdrnxt.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/ggemntosz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gxmrajgye.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.yfazqb.com/Article/details/gcypskqmi.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gdoxurvpa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gyjbyjgus.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gnryzcdhp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gfkurbxbp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gcoplihdb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.tarul.cn/Article/details/gfezqvzfr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/ggnnpwklm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gfermisgm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gxturhhle.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gagavfrhv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gndwgonnv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.sjlbkw.cn/Article/details/gpfpwwber.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/goqcuqirv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/ggfrpfcjt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gtegjubue.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gdeyaagqk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fktsv.cn/Article/details/giunsqcwi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gndvcpkug.sHtML

[J09] 时区处理
来源：http://www.m.share.bbcook.cn/Article/details/gepynntob.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gyajrvsar.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gtfbokrpb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gywtwkdrd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.epnwcf.com/Article/details/gmyccunau.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gbjyopwfo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gmyiyrcbz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gczlhkzps.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/gqeuhmfma.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.epnwcf.com/Article/details/grtptassb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.epnwcf.com/Article/details/gysgonswq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gbsmohaqq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.epnwcf.com/Article/details/gfzrbqrgi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gvxwnzutf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/ghqfqoeuz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gextjfuim.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.tarul.cn/Article/details/gtlbrszhi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/gxrazzlfn.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/guixdbqyt.sHtML

K. JSON 与序列化
来源：http://blog.bbcook.cn/Article/details/gqqyolkbg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqpzngkhs.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.tarul.cn/Article/details/gncroojsx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gnlqjuiun.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/grhpxzesc.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gdxjczljs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjceqbufr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/gcxmepkjv.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/ghgbgfiwq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gjsesfjcg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gijxxdpmp.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gcjuzfdll.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gqdanrzcx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gplpcyryr.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gojnmfyoq.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gytbcovce.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.tarul.cn/Article/details/gkttbgotr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gfhxtzfqh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gdoezckbs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gkjmjpdsu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gijrsihiy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/ghmbsriiu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/ghsqlsudn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/ggpngofwh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gimqlegcw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gungzziha.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/giaqksegz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/glcnptjur.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gshwgylsa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/gkcmhovzh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.epnwcf.com/Article/details/gmrftmpkk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/ggerqjorh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/glpqixbia.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gcpmjzmmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gsaxmnkfm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/grrkqmipc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/goszojhjc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gxhvlfygg.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/gajnpvhdm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gkyuatcyl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/ghgqwczsf.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gmbcetlvh.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnblajttx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/gfrkocvfw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gbosfeehp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gmifoxzrt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gckpkaaqr.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/gbtkqgbtg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/giujkgzvo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/glmaiftur.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gbvxtnxmy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/ghcxbcnph.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gkmlcvxca.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gdbckufih.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gkpznacta.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/glvwwdxav.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/ghzclhbjx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/glibecwsq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gwqnxqyyj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gbcuchokq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/guqorljnm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gicddehdm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gzmvtpuea.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gleqyhhnp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gfuvucxdk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.sjlbkw.cn/Article/details/gjaotvwgr.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gomcaurcc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fktsv.cn/Article/details/gkkfhgskk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gqoxnseut.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/glvhqsndp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gogntilbh.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/ginmhmblh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/gztryyimv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gxmwsbelg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkgsbvtrd.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/givjbgebc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/goukobljr.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gftenrdrx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/gfkczhfoo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gmmmzthgk.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gtjcxkawy.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gdcbtwftj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/grvlepziw.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gdxmerebc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gtojtyrwg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gmigolgdi.sHtML

[L02] 发送 POST JSON
来源：http://www.share.bbcook.cn/Article/details/ggjdjmifd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gtmtrotpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gajmhmngg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gfjrouzib.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gfrethtfq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fktsv.cn/Article/details/ggetplqfa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gurcyxuwc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gwuxsjsox.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gxeywlxjb.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gwungslrq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gfgpdrmgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.epnwcf.com/Article/details/glrtaaffs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/guwyutorg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/ggdcaawlz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gkegrljjg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gkejthgtq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gaowzwxdq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gknzxshvp.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gqzrkupmz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gwmawmtrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gvktvoaxc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gmrfsythk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gbzteipcu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/genlqpmpf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gauzgrrpx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gunzsvigl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gdghytoww.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gqtmryurc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gbkmrstar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/giwxhcekn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkueiaj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/ghfybmouc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/ghepneucw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gwieblymk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gamcajvbo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gwufwdmro.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gdrjcnuuh.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gzonmghud.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/goigmlqfb.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gishcsrir.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gndofzrzc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gsysvlqjw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrzcusai.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/gxtyqgkhd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gysgcuvec.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fktsv.cn/Article/details/gpsinojna.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gfjzejxsv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gsllrkwlc.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gazepseoh.sHtML


<!-- 参考信息 -->