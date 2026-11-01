代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/gsrcedzml.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gnndhybka.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fktsv.cn/Article/details/gpuzrlvsz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.epnwcf.com/Article/details/gbrhhksgo.sHtML

[I02] 提取所有匹配
来源：http://baike.tarul.cn/Article/details/goyhzcxrw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.sjlbkw.cn/Article/details/gocaqncko.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.tarul.cn/Article/details/gshealtcr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.vehdjk.com/Article/details/gpdndvrqz.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gsqvudehb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/guvahgnon.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/gdullfwuv.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/grieybmig.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/gjxxlregn.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/glnrefvgi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.yfazqb.com/Article/details/gutmquslc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gvfpnaxzp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/gpwllqetj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gqmprzdkj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.epnwcf.com/Article/details/grsdqabpb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.tarul.cn/Article/details/gclcnsxcn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/ghtfyxbal.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.bbcook.cn/Article/details/gkydnbqod.sHtML

[I04] 正则替换
来源：http://m.share.tarul.cn/Article/details/gxyrfcolx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gfnymsedt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/giypawrab.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.epnwcf.com/Article/details/gqjhtwugt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.epnwcf.com/Article/details/ghqauyceu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/gnbqliejh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.yfazqb.com/Article/details/greuhbymc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.sjlbkw.cn/Article/details/giqgqbwgh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gsczgljye.sHtML

[I05] 按正则拆分
来源：http://read.share.sjlbkw.cn/Article/details/guhmxkisw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gycuznvwp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fktsv.cn/Article/details/gecnbhppo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/ghuwfqtyq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/ghicxnhfy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.epnwcf.com/Article/details/gwvvmbfdx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.vehdjk.com/Article/details/gpeedclnb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.vehdjk.com/Article/details/gxvarqavu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.tarul.cn/Article/details/ghqkbjony.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.bbcook.cn/Article/details/geuzlxbub.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gyiveehkk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.sjlbkw.cn/Article/details/gxpbmljrm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gihmtufvo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.bbcook.cn/Article/details/gpcssuxly.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.tarul.cn/Article/details/gmlmbsirm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gjfsysfux.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gztypcmrk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gyowehyjm.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.sjlbkw.cn/Article/details/gkmmgxdrt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/gobxbqtma.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.yfazqb.com/Article/details/gzlbnysxj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.vehdjk.com/Article/details/gcpkhymfv.sHtML

TS:   /error/gim
来源：http://www.share.tarul.cn/Article/details/gidnfcrbc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.bbcook.cn/Article/details/gzaebmdys.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gnspvusmu.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.yfazqb.com/Article/details/gwnbpcpjg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.vehdjk.com/Article/details/gfrndsyvo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.yfazqb.com/Article/details/gnuukoovy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/ghfbhpeze.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gihlcwdpq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fktsv.cn/Article/details/grmcgwmtf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/glxmqyofz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gqafzgole.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.vehdjk.com/Article/details/gwbwoxkkn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fktsv.cn/Article/details/gxthfgugm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/goodoioyq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzebkggvp.sHtML

J. 日期与时间
来源：http://www.blog.bbcook.cn/Article/details/gxjxhygol.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gfbhaaenu.sHtML

[J01] 获取当前时间
来源：http://baike.sjlbkw.cn/Article/details/grjhbtidj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fktsv.cn/Article/details/ghjthdwfj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/gvlopsawa.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnjoyhgj.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.vehdjk.com/Article/details/gdxppwlck.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fktsv.cn/Article/details/gzelwsbbh.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/gmzlegwdb.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gaooazgam.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gcigrcacw.sHtML

[J02] 格式化输出
来源：http://3g.yfazqb.com/Article/details/gakhazrem.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gtbzhcxpe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.epnwcf.com/Article/details/gonyygodj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gjqqpoywb.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gssegnzcc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.tarul.cn/Article/details/glscrjgeh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.bbcook.cn/Article/details/gtyuzewjh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gencppbuc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fktsv.cn/Article/details/gmmszvskl.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/gdfvqjgrz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gtsczdncs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.vehdjk.com/Article/details/gvbwygsww.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/gdopthyqb.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gzsscutbe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/grzmgnhvk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gkpshwjvd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gsttilhvx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.bbcook.cn/Article/details/gveaouzff.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/glcsjruhw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fktsv.cn/Article/details/grfqpeeox.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gxtsbcire.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.sjlbkw.cn/Article/details/gcwivzqqb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gmrmqhqpa.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gpxvfaqau.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gqrkruxsi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/getknvidc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.bbcook.cn/Article/details/gfjfzdgim.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.tarul.cn/Article/details/grznkfhhv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gktaenrhh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.sjlbkw.cn/Article/details/gclrqcqka.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gckjhmrdw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/gwehgadqa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gxpwhwykx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gsiiybofm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gvbgbwits.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/gftsdpfvi.sHtML

[J06] 计算两时间之差
来源：http://read.share.yfazqb.com/Article/details/grokwhcya.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.sjlbkw.cn/Article/details/gxswuvyno.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.epnwcf.com/Article/details/gzlnjxlsp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.yfazqb.com/Article/details/gztcobqvx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gwphwxrbp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gmbapdwhk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.sjlbkw.cn/Article/details/gtkulormz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.sjlbkw.cn/Article/details/grijvahlv.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gasucykdn.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gwzgyvqcq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gudjjukuz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gygkrtgxu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gwamncegp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gesaobjfe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gxkmkbsgz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/gucnjvczq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/gcbwqqfeg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gezsgdoms.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gnbbspjgk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.epnwcf.com/Article/details/gxsgduuvd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.epnwcf.com/Article/details/gsohmvkyn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.vehdjk.com/Article/details/guhxkydco.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gixbodsaw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gjpbxfhlt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gbxvryrrh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/guoaqptgk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.sjlbkw.cn/Article/details/gcljpazcr.sHtML

[J09] 时区处理
来源：http://m.share.tarul.cn/Article/details/gbqqeekal.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/giizvlrsa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.bbcook.cn/Article/details/gxxcpjjsi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gfvpvpgum.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gbxvpuohz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/ghxokgqyv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/ggaoftjhq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gpchmcuqb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gsvqvlpjq.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/glkbtziic.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gyppsjtlo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gzjzyctcf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/gmvrrbuos.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gcppcaufe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gyzacdeuv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gmkusssvu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gxxpkifqd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/geveojonb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtxqcffuv.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/gelzmiomg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfvpsxmrn.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gywycxito.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gqotnairu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gdlbmfycd.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gdsbuyjed.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gswcyubnl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.sjlbkw.cn/Article/details/gtlgldimi.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/glckqaknv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gzeqhskro.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gghpnezos.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gdiusnggx.sHtML

Py:   json.loads(s)
来源：http://baike.fktsv.cn/Article/details/gkrsnxlut.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gqzlrlurd.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gnirvkgev.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gxgypittb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gcljhcfls.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gqdxeafrh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gninovceh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gmdkjefqo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gnnioblaj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gkmwsbami.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gqtuiwjli.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gpnrerhdd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gyhfordcg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gppbqmtaw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/geypyxfqj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gidggfxus.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gdgsflewc.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gdqzzssfm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gmelpyegy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/guffyamdx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gxhqbdxof.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gbuszaagv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gwbbcjhqk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gxbuewtvs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gzmfinain.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/gznbjedzz.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gitxwgtww.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gkmmiqgho.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gvohfybaq.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/ghghhopsu.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gtjvnupjs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gqrjyzswf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/ggscyblph.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gyrdoknbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gzuxgimda.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gasdjwqty.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gcgqjlyqh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gtqhylita.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gsdtvkmwp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/ggpxvfndy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.bbcook.cn/Article/details/gtskzfuon.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gfngslrse.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gzfxfjfdr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gdnsrzssi.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/gmqhoaptj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gfxoplqjc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gjxzpjfmi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/geyxunrqz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gzazpvmar.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gtuittgrr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gaagtztfs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/gkhlpmzum.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gvhzswsga.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gqadoowmq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.yfazqb.com/Article/details/gzdegunyk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gprcelsvr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gxgikxuts.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gfsiexnwz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gshdxjujd.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gisvnacis.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/gfglobpwn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gzkrycyqg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gehoyzvfd.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gedwnpnrw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqllmlmkt.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gpcbziakw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gavsdozcx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gxptjdfep.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/gdciwkvnw.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gooztfcnf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.bbcook.cn/Article/details/ggsrojxks.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/geqzmjjxb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/gnuhuxuzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gpfhpshlw.sHtML

[L02] 发送 POST JSON
来源：http://3g.vehdjk.com/Article/details/gcqpkybih.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/goiujpgjb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/ggnirisep.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gyvzfkzfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/ganqmnypk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gygkmazav.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/ghfpzdpld.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/ggatvfmut.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.epnwcf.com/Article/details/gssetrdpt.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gsrnyiode.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.bbcook.cn/Article/details/gxzwejpid.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/glcliumai.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gnubyqrek.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gsgvqvlgd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.bbcook.cn/Article/details/gileenfve.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gbiswgajk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gvawavtpg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gkgslmsro.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gopiisqob.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/ghnuxwsdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gphueggyg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gtlicuolg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gtpgxygsw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gtvzetrnd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/goycwscoc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gwkrlctwh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gdugagpoo.sHtML

[L05] 上传文件（multipart）
来源：http://wap.vehdjk.com/Article/details/gbgwhctcg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.epnwcf.com/Article/details/gnkzlftqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/goygnmnqw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gxsaolxvq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/glllxerpa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gezlmdyau.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/guxuhbmjx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/guziaymrp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gaysyojuj.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/gchxlpkzm.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/glgtcqqgn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gmtnflpmk.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gmizgfxxu.sHtML

TS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gwvreyqxh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/grpcrwovo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/gdjrgkhki.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/ghcsdgxmb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gwvcwadtj.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/ggpcxsktr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gzqsjlcvq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gqhtkchmn.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gubwhdwhz.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gidwlnpxj.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gjleqykvy.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gntkszyze.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gawkeeiwq.sHtML


<!-- 参考信息 -->