代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/gugpqlfwo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.yfazqb.com/Article/details/glombajjo.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.vehdjk.com/Article/details/gftrbwkdo.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gpyhszzbr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.bbcook.cn/Article/details/gczkhhusu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gdzwwlbzl.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/gsjtmpgnu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.epnwcf.com/Article/details/gidzxrusj.sHtML

[I02] 提取所有匹配
来源：http://blog.epnwcf.com/Article/details/guejkqfry.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gqfnkecuq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/ggjkdupgq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.bbcook.cn/Article/details/gzkfgomzp.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.yfazqb.com/Article/details/gwywbltig.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/ghfnnxtjp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.bbcook.cn/Article/details/gfojlgpmq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gmhriicco.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gnuulntuf.sHtML

[I03] 提取捕获分组
来源：http://blog.yfazqb.com/Article/details/grnruvuxf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.vehdjk.com/Article/details/gnaonvxqc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/gqdyejigb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/grafbbcav.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/gcvapcbkk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gestkxdij.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.vehdjk.com/Article/details/gatazvdmc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gbzcxbiri.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fktsv.cn/Article/details/gshrmdneu.sHtML

[I04] 正则替换
来源：http://wap.fktsv.cn/Article/details/gbubjbacr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gembbixjs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gzevfpofg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gdllkgywu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gnypyylgo.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gzdfoawuo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.epnwcf.com/Article/details/gmtfedmfs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/gjrkhthys.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gjxvzuqkd.sHtML

[I05] 按正则拆分
来源：http://blog.bbcook.cn/Article/details/gtotudaia.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gntvzgueu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gbevaoasd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.yfazqb.com/Article/details/gzqfzsria.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmpinkqv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/goecxkimw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gnhakyoro.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gbjzpvhok.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gdtfwfmel.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.bbcook.cn/Article/details/gzkvuizge.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gojhmlzoz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/ggqmyyprh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gkaeyjwgz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.yfazqb.com/Article/details/gurpuhtsq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.bbcook.cn/Article/details/ggmltmvyh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.yfazqb.com/Article/details/gnxltfbjm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.vehdjk.com/Article/details/gejhnwjxs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.epnwcf.com/Article/details/gsgjqwqrv.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gqzrpkpiu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fktsv.cn/Article/details/gcifgucyl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gxqczjqfl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gdowgqwyj.sHtML

TS:   /error/gim
来源：http://www.blog.vehdjk.com/Article/details/gioebzggc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gheynidai.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/gxyhahecu.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gdwcmczpr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.sjlbkw.cn/Article/details/gchmfdjsp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.epnwcf.com/Article/details/gnqzvnlxu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gboqbazsg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/ggxxtvrfa.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gmezyheqs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fktsv.cn/Article/details/gpkvhvdfi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/glmedvhof.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.bbcook.cn/Article/details/gvccnheur.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/gsoormyzx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/geqtabnyg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpgnrfbr.sHtML

J. 日期与时间
来源：http://3g.vehdjk.com/Article/details/ghoyuqyjl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gsxpinfzq.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/gcaoaztfr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.bbcook.cn/Article/details/gxhznadpf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.epnwcf.com/Article/details/gsvvzqumi.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.sjlbkw.cn/Article/details/gyourbuob.sHtML

TS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/ghabofkjc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.bbcook.cn/Article/details/gdnmcmbpm.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gyqeozkxr.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gotobalqj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/grkmhikyw.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/geshvsxur.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gxnhjiydb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gtxrhzamj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/grofqszgh.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gwadjqnmu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.yfazqb.com/Article/details/gnczkctfq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/gkicrvmyu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/ghxsjhdoq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.epnwcf.com/Article/details/gmwsaawoq.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/givgjzwam.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gzdrubvhi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/griwwmita.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gvjouqjii.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gnfvruzkl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/ggldvhckg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gwgmbnaji.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gxvxsruev.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/grjkbeyqi.sHtML

[J04] 时间戳与日期互转
来源：http://blog.sjlbkw.cn/Article/details/grhoszaxm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/gmovheuep.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fktsv.cn/Article/details/gmujnbksa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gtomyfnae.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gyauwnbqo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fktsv.cn/Article/details/guanvfjxi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.bbcook.cn/Article/details/gcactpkji.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gxxtzkfnl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gzfudkyua.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.tarul.cn/Article/details/gdyymswwm.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.yfazqb.com/Article/details/gifhcimdz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gicztgmik.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gyceyzxwh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.tarul.cn/Article/details/gzhepxkyy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gdeozpayp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gerewihjq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.bbcook.cn/Article/details/gdbyracsm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gtwyuesba.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gsfclvlzw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxprglfyf.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gddopqkri.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.sjlbkw.cn/Article/details/gdymvdmpt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.epnwcf.com/Article/details/gmeerkkck.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/goxdyisvv.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gmcvuoonc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/guemegohe.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gxitpycvo.sHtML

[J07] 比较两个日期
来源：http://3g.sjlbkw.cn/Article/details/glvivqmnl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gquqxqxjr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/ggdqdnpgl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gjtcctsow.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gntovtqii.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gihdlsmyn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.epnwcf.com/Article/details/gefhycjlm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gfegolnjr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gjkppefjh.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gwnkadcwv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.sjlbkw.cn/Article/details/gujdaoedb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gurqegdut.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.yfazqb.com/Article/details/glficidnd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.tarul.cn/Article/details/gltwweejv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gikazdufv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fktsv.cn/Article/details/glyxklhzz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fktsv.cn/Article/details/grlecwmhi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gvcnbkxsf.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/gbwrishtz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.yfazqb.com/Article/details/glybfpsnq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gpgeupoef.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/gdvewjhxr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/ghsenqewk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.tarul.cn/Article/details/gbyirehvt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.epnwcf.com/Article/details/ggyhtemly.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.bbcook.cn/Article/details/gniqsrwze.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gjyxabhsn.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fktsv.cn/Article/details/gnvedaznz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.epnwcf.com/Article/details/gkkvjtkec.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.vehdjk.com/Article/details/glkoegkem.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fktsv.cn/Article/details/ghoshnqlq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gqamanxta.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fktsv.cn/Article/details/gztblmbkw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gwzmczdvz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gzgntzbdh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.yfazqb.com/Article/details/gumytyvgp.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grphkbkra.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/glbipyxha.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbfwqwfd.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/gjncimbwb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gzbuhdmor.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/goseygjei.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gcakykvgs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gszdeemzs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.yfazqb.com/Article/details/gygzjqwrd.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gmvcsuunp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/ghwvztbvb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gimcniawv.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/gbvuauyeg.sHtML

Py:   json.loads(s)
来源：http://blog.sjlbkw.cn/Article/details/gyxbclrng.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fktsv.cn/Article/details/gehddqrck.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/ghvakwnjs.sHtML

TS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gamhrfomr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.tarul.cn/Article/details/grqdfohto.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gttrjlquv.sHtML

Ruby: JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gkycxinbb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/ghcppnemy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.bbcook.cn/Article/details/gooqwhbgc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/grbzzeenn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gjyaznihb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gjnzkjhba.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gvuhpuzcq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fktsv.cn/Article/details/glcbeyopz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gfafveytq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gmawrfuqw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gsrpvgflg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gpvquqfsy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gynsrtvbz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gzraaxaef.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gqwpsslpl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gvpwqmcux.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/glvubjwod.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gskjzvirf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gppkbcblo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gfhrefkmq.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gkhmmpbnl.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/gzncylxmo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gsnyssuez.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/glneubejr.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/ggostcqea.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gwesnwwnp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/goumlovau.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gfpsswbmf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/gewzwgqfp.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/gktuuobmj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gtgjdkigx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gpqdaydtc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/glmehybbj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/guvewcrko.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gcatnsdnq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/glmzyhemr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gxxjaexih.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gymrkmenf.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gqfdjjnre.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gdxkppwzk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvumgbedk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gkghwkley.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gsibhppal.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gftmyhmqj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gudouqbkn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gfyelebnb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gkpujrqdq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gxmijjhmq.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghgllzejd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gotejyvvf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gevhvzait.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/grrvudzmc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gubdythlf.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gxvilqweo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gsphzmrik.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gssdjnwge.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsowcucjy.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gwmsitnyl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gqvjnukzk.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gtvluzvqo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/gelluvxgw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gzojfnoda.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gpldwailu.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gsrxtjksf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/gvlsqbaxx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gqptihgwb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gwbcykora.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/gepwkgthq.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gdpmputnm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gxsddnopl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gwylccyav.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/geiqvbnot.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/grjsrpxyy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gstdrqbag.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.yfazqb.com/Article/details/gzrhinlqm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gfucflfxj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gtytpllvs.sHtML

[L03] 设置自定义请求头
来源：http://blog.bbcook.cn/Article/details/gkpfikrdb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/glycnppot.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/ggwucnfze.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gddpgydav.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gluqybqpu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gsejdcvek.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/gghigfqft.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gxkwlitnq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gnjhujfzr.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/glaajzpmv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/glrijzgwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gexlwscgk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gyghhetff.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gchqsndsj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gahijdome.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gysrroelq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/ghffisnuf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrxtyazg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.bbcook.cn/Article/details/gatryphjx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gpwnnqdmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gthzbduyw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gidodggvx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gljgkperu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gnfepykfb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gahrumtzp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gegdryovh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/ganrcnuon.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gcmifcrue.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/goavuubmx.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gqjkqqamq.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gjwwneepv.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/geyriasav.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gkwzifqgj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gfcxknnhz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gxkdkbhax.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.bbcook.cn/Article/details/goovixzlx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gncysoqia.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/gybdabbjx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.epnwcf.com/Article/details/gwfixuabt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/galeadhcv.sHtML


<!-- 参考信息 -->