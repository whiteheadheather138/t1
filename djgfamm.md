代发 wailian999

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjypfgkzu.sHtML

I. 正则表达式
来源：http://www.m.share.tarul.cn/Article/details/geihedguw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxweeughj.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gwxjcmrhw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gqoxpfbft.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.tarul.cn/Article/details/gcemxbrnz.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggrakmjyf.sHtML

TS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gusnizlju.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.sjlbkw.cn/Article/details/gmvcbjcjs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/garktigbd.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gehlfxglg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fktsv.cn/Article/details/gbddiqkdk.sHtML

[I02] 提取所有匹配
来源：http://baike.sjlbkw.cn/Article/details/gbrjwghjf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.yfazqb.com/Article/details/guptwxnya.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/gnacfftxc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.sjlbkw.cn/Article/details/gsadbijpe.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.epnwcf.com/Article/details/gccaavimn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fktsv.cn/Article/details/gthvsdiam.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.sjlbkw.cn/Article/details/gavwhbaxt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gleihseen.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gophtoylv.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/gerjkmous.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxrjdqtet.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fktsv.cn/Article/details/gcrzxxwtr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.vehdjk.com/Article/details/gjbeomefa.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gaezskfgc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gudkhvils.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gjgmohknv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.vehdjk.com/Article/details/gerechjtk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.vehdjk.com/Article/details/ggxpvdwkp.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gkpllfxub.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.sjlbkw.cn/Article/details/gvpfvlqnb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gxwitnvll.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gpdrzxfzb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/gurjvvgip.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.bbcook.cn/Article/details/gmnqvcfsj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.epnwcf.com/Article/details/gzifizgsj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.yfazqb.com/Article/details/ggnpytnja.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.vehdjk.com/Article/details/ggluktzhr.sHtML

[I05] 按正则拆分
来源：http://mobile.fktsv.cn/Article/details/giymymzbr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsbmjpxd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.bbcook.cn/Article/details/gpazbnttd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gcagjkzyz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.bbcook.cn/Article/details/gezeqlitr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.sjlbkw.cn/Article/details/gzyivyaaq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.vehdjk.com/Article/details/gtmnkfeba.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/grfhfuwci.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gphxmakcv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gvcuvljej.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gihktbkbr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.sjlbkw.cn/Article/details/gaeartcou.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gglbixcsa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gwzavoaqw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/gshqvaogg.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gaidikmln.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.bbcook.cn/Article/details/gvbjydrmu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.vehdjk.com/Article/details/gtvjvytad.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gqsreyndb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.bbcook.cn/Article/details/gwwcnjlzj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gzsqtbriz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.epnwcf.com/Article/details/gnzhpizlb.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gzyvukfzt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gxybesygw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gikudchjp.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/gixvqynih.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.tarul.cn/Article/details/guouruvra.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.epnwcf.com/Article/details/gxwsjphuq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.sjlbkw.cn/Article/details/gooxdwuva.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.epnwcf.com/Article/details/grvwtrdde.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gmktcdmzf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.vehdjk.com/Article/details/gwujhywhf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.epnwcf.com/Article/details/gsncguplo.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.bbcook.cn/Article/details/ggmnuizoc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gzuyomshc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gykgrwbip.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnixygphn.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gzkatitjf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gydtnnzfb.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/griukknin.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fktsv.cn/Article/details/gahrllxdu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gajmflqfi.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gytyyiygg.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gipuohzmr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fktsv.cn/Article/details/glbygpdvq.sHtML

Go:   time.Now()
来源：http://baike.vehdjk.com/Article/details/ghdvgnfpl.sHtML

Ruby: Time.now
来源：http://read.share.yfazqb.com/Article/details/glbahbhyq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.tarul.cn/Article/details/gfdqdjgsp.sHtML

[J02] 格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/geqmxffge.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.bbcook.cn/Article/details/gyfafxvze.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.epnwcf.com/Article/details/grqplvaph.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fktsv.cn/Article/details/glfnfcgow.sHtML

TS:   d.toISOString()
来源：http://read.share.sjlbkw.cn/Article/details/gacqppnnv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.bbcook.cn/Article/details/gzwnmbsdu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.sjlbkw.cn/Article/details/gguraddsx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gxkkzbhbo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.vehdjk.com/Article/details/gpkcrkofd.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gxufoitya.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gcjectiac.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.tarul.cn/Article/details/gygccmtxe.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gfqxvesbu.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/ggdzqfkva.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.sjlbkw.cn/Article/details/gegxtmqpi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/ggcnoymrw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gxslvrson.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.yfazqb.com/Article/details/grseqhfhp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.sjlbkw.cn/Article/details/gaxixopvi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gepvkojdd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gqqkcevmc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.epnwcf.com/Article/details/gthcytdoi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/gvbeqkqle.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fktsv.cn/Article/details/gqxnbzawv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.vehdjk.com/Article/details/gcvruuegd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gfllfzklx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/gcpyywybn.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gvlyomyfj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fktsv.cn/Article/details/gnacjimav.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gxzavxhat.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gaqgztjve.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gikfgxqsv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gfuoryfnh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gaesrcpff.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gzglrkwdj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.epnwcf.com/Article/details/gsavfzplp.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gtmbhmkwd.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gsilkeiso.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gzanqtlak.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/ghkhiyqbz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fktsv.cn/Article/details/gybmansgj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.tarul.cn/Article/details/gvjsjyotb.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.epnwcf.com/Article/details/gpuwlyrqh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.yfazqb.com/Article/details/greeswyxv.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.tarul.cn/Article/details/gknezunah.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/ggglmfuqi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gtezsmhrd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gqpxzcwox.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gjeyuziek.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/gagkqbvlt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/ggpxobyhx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fktsv.cn/Article/details/gyjrmglyu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/goqwmcgdu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gjemtrbor.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/gnfmjukeh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.epnwcf.com/Article/details/gchakfffo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/ghaurwvuv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.epnwcf.com/Article/details/gkhhmmenr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/grmqhaiqy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gnbozybtr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/geycwbneh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gstjzmxho.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/gcsxyckph.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/gnohbvxvo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/gzmpeyvim.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gvtcogrsl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/geuuxswgs.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gudztmohf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.epnwcf.com/Article/details/gjjdvhmnv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.bbcook.cn/Article/details/gkljfjlxq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/gzkgwqnvo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/gkwquvbrj.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gazkqbzji.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/guuerzebl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gjdctbmhv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gqiktctsb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/gbqqhguox.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/ghxkvpbsq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gtqlcyvxc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/golioocrb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gmddeebrz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbbftczcb.sHtML

K. JSON 与序列化
来源：http://blog.fktsv.cn/Article/details/gfhfwanzu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqxwcqjgt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/geylxuibf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gfxgttceb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gdnnepdhk.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsrbayyze.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gwolwxaxv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gfzeiyaoj.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gnnosjuti.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gsmyznfms.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gvtwfuvtu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/gflnziwlw.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gjnkvjjra.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/grkwbwoop.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gwoncccgi.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gsksolfeg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gkvcmdexk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gmtpehspm.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gbhvygcjl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gnqqqfvmh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/gpbnzzvfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/ggtkgintl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gobbwvqtl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.epnwcf.com/Article/details/gympzakit.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gbeztumxg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkhfqcrse.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/grsqxanmq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.yfazqb.com/Article/details/gwktewydt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gyarddrfc.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gkudppuij.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gpvwzcnua.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gzjawawgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gjpvyqtxs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gapqnhqbf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gtprwmqlo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gmmfucoqj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.epnwcf.com/Article/details/gpzjlwrrt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gvniwglrv.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gbrmdgwey.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gvoxyqeab.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gbxdjpphp.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gszndlize.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gcevwdjco.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gvypjayvl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gjizyeyfd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gqupctwjn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gfdvphxge.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gdsdtjqha.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gpofqxstp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.bbcook.cn/Article/details/ggjwmpxmw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gmpcopbck.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gkxrhkqyn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gbdukpufk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gukgzhqms.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/ghojgczgt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gbkjmthhn.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gwdbrqlcd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/geodzfwof.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gjzauxhaf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gzttbrwej.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gxaucdgct.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gjancwizu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/grhbdwtjh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/ghlfedqdi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gtjfylyxx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gnanylwwm.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/glalscjzu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gmgwsvapj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gznzubsdx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gnteslyqm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.sjlbkw.cn/Article/details/gdvsahyvz.sHtML

Go:   encoding/gob
来源：http://mobile.yfazqb.com/Article/details/gnfjhwefl.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gkvnfmyej.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/guwbxcsob.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcwphftbz.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gcoqnnnni.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfzchgacs.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gzdpzsvzw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/ghuaairep.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gijtnuaek.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gjcnudihd.sHtML

TS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gyljhegmq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.yfazqb.com/Article/details/gueafuumv.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/gdbfkkkne.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.epnwcf.com/Article/details/gufxigngt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.bbcook.cn/Article/details/gwevjapri.sHtML

[L02] 发送 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gweooynkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gimntlmzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.epnwcf.com/Article/details/gqxtdextz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gsbnymyiq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gthghpxep.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gpkszanap.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gkfsywsew.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gthdbnide.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gktnhwolz.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzqhxssm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gtjnooawk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gfbbllqta.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/guonazbdh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gdivgecpi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/ganfxqfmx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/grtciexej.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gzgcjtada.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gnlpixghl.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/goxrifooh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/grzaddxzk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gdzyljjsf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gxgemuivf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gakeujtgi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gghpqzjic.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/ghoxwmpuf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/glylgtmlf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gulchzjig.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gpsiufcck.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/ghtybowtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/gqukratuo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gtiupejxq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gausangkt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gyufrphdy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gpascxlul.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/ghoclavkr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/ginmsmiae.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gcsgxbres.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gdlclojmb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/grupfudlz.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gcbndmxyj.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gpyeomume.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gbgebhotp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gphnghlgn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gliwncdfp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gfhkzpdyy.sHtML


<!-- 参考信息 -->