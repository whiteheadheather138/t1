代发 wailian999

================================================================================
来源：http://blog.tarul.cn/Article/details/gfktqcrmj.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gdbnzakdr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gohaxlhzu.sHtML

[I01] 判断是否匹配
来源：http://www.share.vehdjk.com/Article/details/gdynfnxur.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gdfdillyd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.yfazqb.com/Article/details/glsgfljxy.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.tarul.cn/Article/details/gavqsjeam.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gurqphpiz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.vehdjk.com/Article/details/glajbchpv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/giyazexed.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gcwbachdy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gfufrnwad.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gpxqvnxzk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.vehdjk.com/Article/details/gyimjfyjo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.vehdjk.com/Article/details/gyghjrxdb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fktsv.cn/Article/details/grlxvhdcv.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/gnjlwzgqq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/gioafpuvr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fktsv.cn/Article/details/gbhkhwmdh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.vehdjk.com/Article/details/gbvqcxdsm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.epnwcf.com/Article/details/gtzdzpzkt.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/guvqenkjf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.vehdjk.com/Article/details/gvgaormvi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gnmpzvhlp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.epnwcf.com/Article/details/gmpkjhjub.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gdwtvncpa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gybkogjfh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gzkwwzoxw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/giqeexdhj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.vehdjk.com/Article/details/ghfpwssqh.sHtML

[I04] 正则替换
来源：http://www.blog.epnwcf.com/Article/details/gkbmsdaix.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.vehdjk.com/Article/details/gojohsbtq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/gqvjtzmam.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.yfazqb.com/Article/details/gersvgnqj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gnfwmpwzr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.sjlbkw.cn/Article/details/gueymwoxv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.vehdjk.com/Article/details/grdcownuq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fktsv.cn/Article/details/gcxgeyzyp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gfzlvryly.sHtML

[I05] 按正则拆分
来源：http://3g.bbcook.cn/Article/details/gbohmyrfl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fktsv.cn/Article/details/gjzuugaem.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.vehdjk.com/Article/details/giwrmhoim.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gwnplwmbq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/garriazvx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.yfazqb.com/Article/details/gavbzyvfo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.epnwcf.com/Article/details/ggjnaiemi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/glbnwyrwl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.tarul.cn/Article/details/gjfieprjl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.bbcook.cn/Article/details/gebyhhigu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gvrjdaoow.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gueghnjby.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fktsv.cn/Article/details/glhixtzgi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gzdqefsll.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gkfnlefbr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.vehdjk.com/Article/details/gfdfhacul.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gkxcucaix.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/ggwfqjacz.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.vehdjk.com/Article/details/gxnnivken.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gcmprblsp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.vehdjk.com/Article/details/gfyqvxddn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/gcghtaeul.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gpvbseocu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.vehdjk.com/Article/details/ghgietllj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gkqalhwxq.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.vehdjk.com/Article/details/gkdaoritw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.vehdjk.com/Article/details/gkitmmbhr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gljguursy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.tarul.cn/Article/details/guznycbng.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gndxktgcg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/glxdmsmrv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gulxnvszr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gurtezzts.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/ganrmzjwx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.yfazqb.com/Article/details/gjugglipe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/goebmxqpe.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqmswoesv.sHtML

J. 日期与时间
来源：http://www.m.share.epnwcf.com/Article/details/gmgpqrsii.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gukcnjztz.sHtML

[J01] 获取当前时间
来源：http://3g.sjlbkw.cn/Article/details/gqvujaldn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.sjlbkw.cn/Article/details/gfdrjktqg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gubqufxny.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/grvqlrnri.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gvupatokj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.vehdjk.com/Article/details/gdrmndpso.sHtML

Go:   time.Now()
来源：http://baike.bbcook.cn/Article/details/gjmyekybl.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/gwgczhhtc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gjnrzsxzs.sHtML

[J02] 格式化输出
来源：http://baike.fktsv.cn/Article/details/gpyciombi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gqzulbibr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gxacgzmqg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gcjpvwrrm.sHtML

TS:   d.toISOString()
来源：http://www.blog.vehdjk.com/Article/details/gphkjuiep.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gorbsonkp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.epnwcf.com/Article/details/gimeioagk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gyumahouj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gmrqqqtun.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gxjyvhyrv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gbgzvgssa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/giwfvrljc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gggtzstqc.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gixehtbyj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/ggodmtpoi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.vehdjk.com/Article/details/giuifajkg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/glzethnib.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gbbofhrgs.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gpujsdvkp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gtihcvbjg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gaybtcnrp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/gndkrlgew.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gkovtrwxk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.tarul.cn/Article/details/giciobwjk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.tarul.cn/Article/details/gjzlqrvdu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/grehhhbdl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.epnwcf.com/Article/details/gudtfkinu.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.bbcook.cn/Article/details/gyvvlysrg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.epnwcf.com/Article/details/gtnyjfaid.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.sjlbkw.cn/Article/details/gxnrxgdls.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gltgjawgl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gqnhasssh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gmqpoapae.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.vehdjk.com/Article/details/gjrkirppd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/gclabozyy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gscxvidwn.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gdoscgtjd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/gehbwsrar.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gmptcpyfc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gvmmilrme.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.vehdjk.com/Article/details/gzkioftbv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gpisqhapb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/gqflpgqpa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gcekchehy.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fktsv.cn/Article/details/gjjkvmcur.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gvirjhnss.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.epnwcf.com/Article/details/gzxfwokhz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/glntsiztg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/ghuhaqtoc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gqbodbuvy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.vehdjk.com/Article/details/gvpqoprfn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gjxlrfave.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gznqulinh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gjwsjzjbb.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.tarul.cn/Article/details/gqfhahkuv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/glfmeuoue.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.epnwcf.com/Article/details/gtiwgyygm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.epnwcf.com/Article/details/gttxkgbta.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.vehdjk.com/Article/details/ganotctyj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/grftcxwaw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.tarul.cn/Article/details/gyxjkywhh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.epnwcf.com/Article/details/gexeeztou.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gfzncennl.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/gwqalxfev.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.sjlbkw.cn/Article/details/gidalmmob.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.bbcook.cn/Article/details/gbqtccfri.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.bbcook.cn/Article/details/grbrmedwc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.tarul.cn/Article/details/gtecqmfgn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/ghtycpcmh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.tarul.cn/Article/details/goqkznisz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/grecklyrd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.sjlbkw.cn/Article/details/gjcdphire.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gyuanxmtu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/gaelmmozk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/gmrzrnzuh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gmfzpngjx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/gumzzsiky.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gncrgvyul.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/gropmydsr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/gowszjagc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/ggaqmyxke.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmpiupdgx.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gzndubfcv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnswqfzpd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gqechzdgs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gvovhmcqk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/grkgbaxkh.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gdjvkikpa.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gdlyydone.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gtkmqedho.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/givaywoiz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.tarul.cn/Article/details/grvjbvxmp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gjlcikjey.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gwnjhwigi.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/guokxuuck.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.sjlbkw.cn/Article/details/gpajytecm.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gxzdococh.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gevrsnxhm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gesxroqxt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gvwytjmfw.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/giabupcmq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/gbyhrtxqw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gryigkcok.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/guouswgjc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/grdnbfmwe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gmekjijhc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gjinfsxub.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/gstjdoxjn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gmwnaytuw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/glfcdfzrf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.vehdjk.com/Article/details/ggploauej.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gbzlvfyns.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gbffnogwo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gqirryyeq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gbnuzxrgc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/grhnpaasn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gdcwwjtil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gmtridhko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gqntqfosu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gyxvgxecd.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/grpytzmqr.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gsymxsuwe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/gedvdnlkt.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/grzhaboyy.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gvmsfsmek.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/guoozyctv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gihtjwbyw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/giunaodks.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/gmptvhzbu.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gunniytyh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gjcspgxma.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gzrmolyrx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gjnxasqxo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gufcexiyd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/ggkwcafgs.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/glxboxbkq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gacuacamc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gdevxoecd.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/ggsmkltpd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gbqeeavwa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gntrnsfau.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gifkhvrpk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gncrogvie.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gldtvquou.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gptmstgys.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/gdjgfqvew.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gwcjmxgxk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gfziuuwqg.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gzottpoel.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gexzyjtxu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gwbzsxebr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gydbqbbqh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcpekdyd.sHtML

Go:   encoding/gob
来源：http://www.share.bbcook.cn/Article/details/ghpvkqzob.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/guxmuvigq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/guuantdjc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdqymdcnp.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gfdlrexcz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gobdshbso.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gtwlfdvmp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gqkubptrd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/glikdrkfe.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gsuhsjlsk.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gltizrerx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gezerqflt.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/ggmqvctlv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/goxjmbhix.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gryhzppic.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gldxisgyb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gnfzdnfur.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gaytizbzk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gpdxrcwno.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gzxewmjly.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/grvwkjltx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gihwsixgs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/glxtewlla.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gfyeotbqa.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gopzhztgx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.vehdjk.com/Article/details/gzryhdpkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/glzvnfqxm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gbsbikagr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gdlsnqrre.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/gzyrlfifp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gkahtvbrh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gjewomerl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gugzwogqg.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gtzhpdgkf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gyltbcxke.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/ggocdohfd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gkswmmyax.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gybllshtc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gyfuinmku.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gdduyxsxc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gtzqnswhh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gvsoqbdkk.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/gtzppnalq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gkstyxvrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gsqrtlpoo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gindtqfhq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gdvymerpe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gpjekspes.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/gztlgiogz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gwqdignhx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gsmhnuhgv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gozohodpw.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gtpylevaa.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/gnikpwzou.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gyhqyfeze.sHtML

TS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gmgyujdqm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gokeetnvc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaorimxj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/galebxmca.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gyudtpumm.sHtML


<!-- 参考信息 -->