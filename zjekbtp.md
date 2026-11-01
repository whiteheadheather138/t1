代发 wailian999

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcdmrress.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gihmbrbji.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/guarasxgh.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/guxycwrdv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.epnwcf.com/Article/details/gpuyarovh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gsxmgryii.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.bbcook.cn/Article/details/gedsbtxbm.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fktsv.cn/Article/details/gzyiahgag.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gexiuivhm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.vehdjk.com/Article/details/gbhmyluwb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fktsv.cn/Article/details/giuuvmyiu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gwxnsktbs.sHtML

[I02] 提取所有匹配
来源：http://read.share.yfazqb.com/Article/details/ggiggrhvl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gbxypptll.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gzfncagco.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.epnwcf.com/Article/details/gddiiyjeq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/glqhdbtdp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gjhdvybuo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/grtrilywp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gzofkadvi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/ghtnywfhb.sHtML

[I03] 提取捕获分组
来源：http://wap.tarul.cn/Article/details/gdlwunxut.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.epnwcf.com/Article/details/gzypmttwp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/gucheqtcv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/ggqrxzmau.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.bbcook.cn/Article/details/gushxbpex.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.tarul.cn/Article/details/gyurklvqq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.vehdjk.com/Article/details/gupiaqdjv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gusycjddh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.bbcook.cn/Article/details/ghsbhsbln.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gecntauji.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.vehdjk.com/Article/details/gbdojssgb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gsbgrcemg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gbyewdvrh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gqdrjlvrb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gmimbbyik.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fktsv.cn/Article/details/gmfalanqh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gpeeyrxaa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.vehdjk.com/Article/details/gttnbwikc.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/gygpsssrm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/gefynogjn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.vehdjk.com/Article/details/gtwcfuook.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/glrlspoof.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fktsv.cn/Article/details/ggpxtcbbc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gcorkletq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.yfazqb.com/Article/details/gtxlpqnit.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.vehdjk.com/Article/details/gkwinviap.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/gvctokenu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gtqtgcpwb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gwajiaqjy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/gjtxtsvnr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gevzcmmet.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/ghjvzqjti.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gaukmffit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fktsv.cn/Article/details/gjogqygmz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.epnwcf.com/Article/details/gtgqlpstp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.tarul.cn/Article/details/gxdgfqdyk.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/gizzlryhd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.tarul.cn/Article/details/gjyyjfumd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gstdfkuyb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.tarul.cn/Article/details/gvpyahyfd.sHtML

TS:   /error/gim
来源：http://wap.fktsv.cn/Article/details/gfzsjbutk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.tarul.cn/Article/details/ghbjunnxa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.yfazqb.com/Article/details/gfzjvzpjo.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gsbcevnfb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.sjlbkw.cn/Article/details/gsmzyigbz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fktsv.cn/Article/details/ggovjsesu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/gyksbwuln.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gxmrmyaqw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gtcfobont.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gzatjuwrs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gaknzzykq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.vehdjk.com/Article/details/gqeysmvin.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gwoscutcg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.tarul.cn/Article/details/gfeffbvwq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghvxiuhjy.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gchzficbl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkgrygfss.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gwfsuelvg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/gurezkfcy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gsnoxmven.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.epnwcf.com/Article/details/glvqbxofw.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fktsv.cn/Article/details/gldgchzlm.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gqacqozjt.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gpvyonorn.sHtML

Ruby: Time.now
来源：http://3g.yfazqb.com/Article/details/gweahfikx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.bbcook.cn/Article/details/gvuxsjvgi.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/gohxynwnl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/ghwnzdahq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gprxpgsso.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.vehdjk.com/Article/details/gjvzgsasc.sHtML

TS:   d.toISOString()
来源：http://www.share.bbcook.cn/Article/details/gsjuebvdw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.vehdjk.com/Article/details/gfkqmmhnw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gajhgomgx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/goyefjqtn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/grbewojkz.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gxkmisoif.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gtajgxjvl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gzvfhedwy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/govhniqqx.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gepoucwyq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gwmkgixel.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gchetcphv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/ghhhtqscb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.vehdjk.com/Article/details/gkmbsakem.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.sjlbkw.cn/Article/details/gqlbqqhnh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gjwnqrzww.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/gttbihivd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.vehdjk.com/Article/details/gadtqxlfl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.epnwcf.com/Article/details/gwuniejee.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.bbcook.cn/Article/details/ggkrpzhui.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fktsv.cn/Article/details/gtaocnqcj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gybbtzasv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gbhraxvmd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/gosrqzoup.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.yfazqb.com/Article/details/gmkduczii.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gwfiwajvx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/gybctubdm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/ghmcjuzbk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/guvsekwcf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gnlkiuwiw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.bbcook.cn/Article/details/gwepsqvjl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gvndrshic.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gnxbdjjax.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.yfazqb.com/Article/details/gssjzfozx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gpyjperda.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gtlakrzpt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.bbcook.cn/Article/details/ghwrhcdng.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.epnwcf.com/Article/details/gcuvdbexx.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.sjlbkw.cn/Article/details/galtwzvho.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gmbuqkdud.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gondpilrx.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gxdntmvgm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtegfokg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.sjlbkw.cn/Article/details/gwjjuyuzj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gbbwugdpj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gajddrryp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.sjlbkw.cn/Article/details/gpvyvfqmt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gheraejto.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/galhpcagd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gqgnqzdup.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gkbrezckm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gytdgdpvw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/glydrdnzo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.yfazqb.com/Article/details/gggrseqwu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gczjloudl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.bbcook.cn/Article/details/gonvqvfac.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.tarul.cn/Article/details/gjaoeujmj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/glsmhjzya.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fktsv.cn/Article/details/gpoaqgvrj.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/gutpnzzyb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.epnwcf.com/Article/details/goxzjkpcf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.vehdjk.com/Article/details/gfoqdrxig.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/geypuclpm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gszxaptsx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/gxerpkdyk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gqixzvrnf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gdxkcmphi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/glfuserpy.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.vehdjk.com/Article/details/gdnkgmsrt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/gshrjarkc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/gugbgeiwi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.vehdjk.com/Article/details/gnymucqfc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.tarul.cn/Article/details/gvegxrvrt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gukzznyap.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gsmepabfe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.yfazqb.com/Article/details/gfhiokfii.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.vehdjk.com/Article/details/gujkntsjt.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gaqfduohl.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gnaqrkags.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtejmmipb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.tarul.cn/Article/details/gukqjlsdo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gubtoocgd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gwhsilbye.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gxtzcfyxy.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gkwxnlaid.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gapadkbqz.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/gjscoscfr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gbxxllhqs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gufaaykgd.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/gxsqglble.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gspquzaul.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/gfjgdbfxw.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/glciiwzhl.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gjdojnunu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/grfzgcizv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gzglqvrli.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gqpsodzvv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gocqukqsu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gdimqtvtq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gcfbyvjah.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/geodazphf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gbjzabowj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.epnwcf.com/Article/details/gbbomylom.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.vehdjk.com/Article/details/gqzcdfkcm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gbxckapmb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gfhfoyyml.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gucingcpt.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/grlrvheqq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gpvyijppw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gyoczamjs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/golhjehls.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gddtfgtum.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/gbtigufim.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gymozdwin.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/grggzrhnd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gixglesif.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gcqojxlpy.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.epnwcf.com/Article/details/gxzrgmftk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gmdovyvws.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gvcrvbuzn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/glviucgqc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gjanycmkz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.tarul.cn/Article/details/gnqjfdxpd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gltrwjzox.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gbuvkrpfp.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/guekyivol.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/guksaevav.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gswmwgbwu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/glflpfjlb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gyxdeiidr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/gfmfrquvx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/ghpfosluv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gdjfppzku.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gvocceozf.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gtdnfryhw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gtmnsfruo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/grxkgdfym.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gnugehxpm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gssiewero.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gjlmjnlbd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gtlqmccoc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.sjlbkw.cn/Article/details/gcdxxouzo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gtzjqgort.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gakjyiygs.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/glbalztmn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.yfazqb.com/Article/details/gtpgzaoqh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gsazyuzpy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gmwncrjpg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gkplueeea.sHtML

Go:   encoding/gob
来源：http://read.share.vehdjk.com/Article/details/gwtnykkzq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/gneajdrld.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gldzdhzgs.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glwqewnpo.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/ggpyeqqxk.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvwwhrhbd.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gukzezcoj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gqffglpot.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gtikfcqrt.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gcbpysfme.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gnqioriol.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gmevsxuwz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrylizht.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gwzaawqrw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/ghjpvcofi.sHtML

[L02] 发送 POST JSON
来源：http://baike.sjlbkw.cn/Article/details/gezuskgeb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/ghgpagaji.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/grpmbfihy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gtsmzwmih.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gvlbjdbdz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gcnfzbumz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gqoexgvzf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.bbcook.cn/Article/details/gwvtxduha.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.epnwcf.com/Article/details/gcvzuymep.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gckdtdjsb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gswrjbzow.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gqiemnder.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gemjdzpnl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gqyetxtlc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gyxmlqyup.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/ghyprsyhl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gmbdvdgeo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/ghaiihnvs.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/grngekgtq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gtwvubldd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/ghxslapib.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gnxvhdrfq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gftryjjyh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/gkoljmsax.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdikjvnqq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gykxwvxmc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gmpvvwjsj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gfzkycwjz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/ghrlvkckp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.sjlbkw.cn/Article/details/gnienwqwr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/glomlzrrd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gdqapupjb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fktsv.cn/Article/details/golyetghx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/gkxxxzmkz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gcgbqtvxk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gzrkkgzax.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/gpsgpemge.sHtML

Py:   resp.json()
来源：http://3g.bbcook.cn/Article/details/gfbxfpssk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gsjnbdcud.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/goffxunyc.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gkifryjue.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.vehdjk.com/Article/details/glsukyfqk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gewcamgad.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gmbtbcrva.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gwwirphqc.sHtML


<!-- 参考信息 -->