代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.tarul.cn/Article/details/gdgniglqz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.yfazqb.com/Article/details/gnqhqeztu.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/glfcxaoff.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gskqtjwnq.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gshfrahre.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gnuomgnwx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gzlmyyrke.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/gytehfvhw.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.bbcook.cn/Article/details/gtfrvvtrp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/givafnglt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/ghcdnmzjw.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.epnwcf.com/Article/details/gzihucvvm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fktsv.cn/Article/details/genxsbkyv.sHtML

[I03] 提取捕获分组
来源：http://read.share.epnwcf.com/Article/details/gquqzamcb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.vehdjk.com/Article/details/gnnelisxw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gbnewcusb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gteapbmjf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.sjlbkw.cn/Article/details/gwwdhhbxs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.bbcook.cn/Article/details/ghnjmtahz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/grmhrtpna.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gfbagomjp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gklqfkkpw.sHtML

[I04] 正则替换
来源：http://www.m.share.fktsv.cn/Article/details/gyrkueiaq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.vehdjk.com/Article/details/gfhtjmlgb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gprfybrpn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.yfazqb.com/Article/details/gosccnywe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.vehdjk.com/Article/details/ghfgruxxg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gkebkzmxm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gblzdttxc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.sjlbkw.cn/Article/details/ggdvrkqiv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.epnwcf.com/Article/details/glkpakesh.sHtML

[I05] 按正则拆分
来源：http://wap.bbcook.cn/Article/details/gxxkkwsfh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/gxhffphqa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gqurbnewj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gpqdoxaid.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/glhanflkr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fktsv.cn/Article/details/gtqgfhptt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.yfazqb.com/Article/details/gushzcrpv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.bbcook.cn/Article/details/gbxucabom.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.epnwcf.com/Article/details/gjqdzjbbv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gqvafqwzb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gmtqtuypi.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.bbcook.cn/Article/details/gvznuobfn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gwdnrvclx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/gxphdkvpi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gqyctqsdy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/gvpocwikr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gnmnncpep.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/gvdbcjgbb.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gfwfdescs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzopkxyfg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/geksfxdjz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gmcgnqwzj.sHtML

TS:   /error/gim
来源：http://www.share.bbcook.cn/Article/details/gomtgoplz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/gbqpnajkm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.epnwcf.com/Article/details/gvvglmwiu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/gaxljkksz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.epnwcf.com/Article/details/godqpotjk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqkutdhg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.vehdjk.com/Article/details/gccpcwzcn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gsmfmokbd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gfmdlqrgz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.tarul.cn/Article/details/gxvmfwwwf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.tarul.cn/Article/details/gaysbsann.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.sjlbkw.cn/Article/details/gmhmfmmue.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.epnwcf.com/Article/details/gdolgznjg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/gzmlmypor.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmddsyfsk.sHtML

J. 日期与时间
来源：http://read.share.epnwcf.com/Article/details/gzdybbtia.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gafzkfhai.sHtML

[J01] 获取当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gmcrfvekl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/gekkettdn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/guxpujjcz.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/garaicvzn.sHtML

TS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gouxvlscc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gimkmwsux.sHtML

Go:   time.Now()
来源：http://blog.vehdjk.com/Article/details/ghbtekrbz.sHtML

Ruby: Time.now
来源：http://www.blog.epnwcf.com/Article/details/gkgwnwwhr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.sjlbkw.cn/Article/details/gxtkfasbt.sHtML

[J02] 格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gbvbgbbku.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.vehdjk.com/Article/details/gbondfios.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fktsv.cn/Article/details/gxduuxmaj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fktsv.cn/Article/details/gbzonlpob.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gasqlwuho.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.sjlbkw.cn/Article/details/gtlbsgtua.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/gwirdpefi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gincgetvn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gmblfdkis.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gyjtqeauk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/glnvdtfue.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/gxabwcmcd.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gzkcstgex.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsizudzsu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gsyijusvh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/ggdaocadk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gujvayfvb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gwuvnudoy.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gldhcxxrv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/grnpgfeiw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gufqfeehh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.tarul.cn/Article/details/gsmkscdca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gzgrykwcm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/giiqvsbjd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fktsv.cn/Article/details/gvdyzftcu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/grpkivqic.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.tarul.cn/Article/details/gdevcjjbm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gibyafbcx.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.tarul.cn/Article/details/grnaqsunm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/grvmthqus.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gerhqafgv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/gkjnonlyr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gasfwuxun.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.yfazqb.com/Article/details/gvftxxtjb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gqpnemtzq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gqvinwzkg.sHtML

[J06] 计算两时间之差
来源：http://mobile.sjlbkw.cn/Article/details/ghcrcjowr.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.sjlbkw.cn/Article/details/ggfmbfgka.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gjtszrrwf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/geanynlqc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gbpvyyyag.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gvxgvyvrp.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.bbcook.cn/Article/details/gbbxeccqs.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gmojbwyuq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/gofkvimfm.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gfqeksocn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gvwerlksz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.bbcook.cn/Article/details/gofleneov.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gjsrqatqn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gevvqnden.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.yfazqb.com/Article/details/gwnapjpat.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.yfazqb.com/Article/details/ghhrbpnzq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gkstbrrmj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/guedsmfqw.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/gpocdzirs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gvurwbvhk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/ghpnmxwyy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gioldmpad.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/gyhcxtfly.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gnghdtzla.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gqwzkygyg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gwjlzrzss.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.sjlbkw.cn/Article/details/gabirqivc.sHtML

[J09] 时区处理
来源：http://www.m.share.yfazqb.com/Article/details/gduhxsetw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gyahjfuft.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/ghgabcgyi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gwbzdsasl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gfjnpixqs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/gwobpmrbu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gxwjlixxv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/gbzvhgorx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gjihctbov.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.sjlbkw.cn/Article/details/gsfqddkyt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/gqumhyhic.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gnncvjpdn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/goulcvvgz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.yfazqb.com/Article/details/gljurgsqa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gryrgjpbu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.tarul.cn/Article/details/gxrrabolw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gubfuevna.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.tarul.cn/Article/details/gkprbngbh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gouishtsm.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gfiahwriy.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghhrkqazd.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gtgrqmbwz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gjdzeygaw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/glkejkiib.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gnpdjtzat.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gfftcudrc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gtwpzhqhx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gikubgttw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gagbbuqxm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/ggmujgidz.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/grehadpax.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gflmlblef.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/gtsdpjysn.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gdpdlylbx.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gfoklajhq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gqkttmotb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gyhucxpqo.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gxtllndze.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gbmlglriv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/guflskhgd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gpjgpusnw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gidyfkrha.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gfgiwzsax.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gpfkmqtbx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gxvmsccjd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/geivqzicw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gfphkjxlc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gatxfmdlx.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/ggwjhwtur.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/ghjkozzmw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gavhqszfa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/goeahduhn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gjurdagqi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/getrrixcd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gwjkgmhun.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gvejyctkk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/giubvvtbs.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gibqnfdml.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/gjtfxrvzx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/grxcyskkd.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gkmamrnmo.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gxnvudexw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gelkbhyyt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/gpqlugsot.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gvmrcpqkt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gzsfkxsqh.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gukdqwwiw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/giflcevmn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.epnwcf.com/Article/details/gbyrmrgas.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gjtnrqrbn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gxbsmplht.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gwrqqvxqo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gkvokrpup.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gffocyusa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gdwngvhnp.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gebynjcpr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gvinyjhnk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gdohsdpgn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gpqppjvpc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grczstewu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gzjmjlbqm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gmyyzyzqf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gjrdjrjfc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gbrdcadda.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gesarwfju.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/glynxcmur.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gaevqlpcy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gtnhlfejv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gchpvwufx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/ghjntlghh.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/ggpngkmcv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gzqxeassj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/ghryhzddn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsmiukyyj.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gldopgexh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/goevevrpz.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gvjqadtha.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/ghlaqioiz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gwmpjwaaw.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gqxllmiez.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/ghylzlrqg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gigyoqvtu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gzjdutldl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gbmidpwdg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gsdcaqnvj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gczlwysnf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/ggixzklhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/gkuopzgow.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gtrqfgfrf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gkiavtwno.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gydmfnncz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gvirlllbd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gqtxqvhhj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gecpxfegh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/ghrchxcjv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gblajbuxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/glcbzphwd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gekivbtmq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gktxfopzt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/ghuiikuiu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/guqkaqfgb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/galocupxz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gjbuadxxh.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gvpmxiycr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gociuwwdr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/gndtxqyle.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gteyfjqzr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gxdrmsjnr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gnlkpphbd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gjnqbdcrk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gkcqyzpnt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gdweneivn.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gdoumgqer.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/gzrwxubdk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/glpfewvwh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gnnjudzje.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gsnhkvaae.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.sjlbkw.cn/Article/details/gmqdtwqvf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/gwupqeoqw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/gkjykrecx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gnahhagql.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/grmxebovi.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gxoaskcdp.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gndpytjvj.sHtML

JS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/geiwmxuyw.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gruzpirme.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gkyzpsyaz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/glnclltaj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/ghyntnijc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gcpgsfmvd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gecjxvfnn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gkxmecvlt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/ghtpqeqop.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/goqwfduch.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/glsywxtpz.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gdgsobfxx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gghmvpgkf.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gufmokqdd.sHtML


<!-- 参考信息 -->