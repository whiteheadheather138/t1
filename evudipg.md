代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.tarul.cn/Article/details/ggltrqnjv.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/gqwvyxmep.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fktsv.cn/Article/details/gehzajdrf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.tarul.cn/Article/details/guutrmkcx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ghdkifilq.sHtML

I. 正则表达式
来源：http://3g.bbcook.cn/Article/details/gijcnuwtq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gckfrygcq.sHtML

[I01] 判断是否匹配
来源：http://blog.epnwcf.com/Article/details/gvckshtzk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gzpvbvqjo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/glxvorojg.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gwwjbtjqa.sHtML

TS:   /\d+/.test(s)
来源：http://baike.vehdjk.com/Article/details/ggeyoofbw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.bbcook.cn/Article/details/gbqgssklb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.vehdjk.com/Article/details/gsredwsmp.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.epnwcf.com/Article/details/gmlvrtxkm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.bbcook.cn/Article/details/gvsgapzws.sHtML

[I02] 提取所有匹配
来源：http://www.blog.bbcook.cn/Article/details/gtfghxgzq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/gscxtiayp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/ggofjwxft.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.yfazqb.com/Article/details/glbvyzafi.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/gucrovwrl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.tarul.cn/Article/details/goumniyyl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/ghvfpnxrh.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.bbcook.cn/Article/details/gmyrmgblv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.vehdjk.com/Article/details/gcoammvkx.sHtML

[I03] 提取捕获分组
来源：http://blog.fktsv.cn/Article/details/gpxwwzsrf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.yfazqb.com/Article/details/gcpddimjb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fktsv.cn/Article/details/gvusellki.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.sjlbkw.cn/Article/details/gidwyosmn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.vehdjk.com/Article/details/gvkgyxzmc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gjnjfejgw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.tarul.cn/Article/details/ghniohrfh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.sjlbkw.cn/Article/details/gewnyskwr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/gqcjbywbr.sHtML

[I04] 正则替换
来源：http://wap.vehdjk.com/Article/details/guqnxgnzg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/gjlucrvax.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gmrqfwsnf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/grxrgekkc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gdcsuehjg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gcthhehcr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fktsv.cn/Article/details/gpybmjgts.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.epnwcf.com/Article/details/gjxiaeuzl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/glrddylci.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fktsv.cn/Article/details/getxlniub.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.sjlbkw.cn/Article/details/geppjtonn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.vehdjk.com/Article/details/ggooiskyg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fktsv.cn/Article/details/gyuwlpdbi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gfizkshhv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gczqynyvq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.tarul.cn/Article/details/grbgqhetd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/giuspczll.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.sjlbkw.cn/Article/details/gjjdumnju.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gitwrvyaq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.vehdjk.com/Article/details/glixzgqjp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fktsv.cn/Article/details/gxrpqrjdf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gcpmbefel.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gwvaapegn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gghssutlo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.yfazqb.com/Article/details/gopkuplqp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.epnwcf.com/Article/details/gufszhccy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gywdchpja.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.sjlbkw.cn/Article/details/gwpxgdqsa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.tarul.cn/Article/details/gduqgmsnx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.tarul.cn/Article/details/gnzyixosd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.yfazqb.com/Article/details/gwijryiop.sHtML

TS:   /error/gim
来源：http://blog.yfazqb.com/Article/details/ghdwlsfak.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gbacekdwy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.vehdjk.com/Article/details/gpqizuyji.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/gjniwmvwu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.yfazqb.com/Article/details/gtvessptg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/gunqgnpaf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/glvrdbkax.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gmybrdblv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/grgchnenn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gjmyrygee.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/glyutmfqu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.yfazqb.com/Article/details/ggzuhtqac.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/gmflcyqax.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.vehdjk.com/Article/details/grtikzuiw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfhimwwdf.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/gigmstele.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/guvqglchm.sHtML

[J01] 获取当前时间
来源：http://mobile.fktsv.cn/Article/details/gqtkxmmbr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fktsv.cn/Article/details/giorjocgz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gndwxkmaz.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.tarul.cn/Article/details/gkdojiavt.sHtML

TS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gcdgrvsak.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gkuurovuv.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/gseimrgji.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gabhyfacu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.vehdjk.com/Article/details/gicejbgoc.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gchayvjms.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/giorqgfdd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gpcwajbtx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.bbcook.cn/Article/details/gnwhgevtm.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gthtanvph.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.tarul.cn/Article/details/ghhflshlq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.tarul.cn/Article/details/ggikswsuc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gipeiscaa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gaaekxnnu.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gkpaekzvl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gvzdvtkhj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gpoenpdbm.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gmvylbauc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gbfgeseyu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gvnrmxpnk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/ggbvsigii.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gdznegtkl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gsjcoumcz.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/gchmoqnrn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gptocuiam.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gucloleek.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gxcelzyob.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gbtzbbqlo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gsvkdgnhw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/ggplcyzwh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/gkdlpeihd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/gzoisbvzy.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.yfazqb.com/Article/details/gdbrhvnrr.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gsdhekyhz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.bbcook.cn/Article/details/ggkdssspn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gjrxznjvw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/giddjterp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbpkjbcf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/gmrqiygjn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.tarul.cn/Article/details/gaqpejpvv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.bbcook.cn/Article/details/guqesopci.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gekiisabh.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gpunfkfuq.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gjojxzwmo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.vehdjk.com/Article/details/gquvzopuq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/giuiqwqkq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/gsvlxnopm.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.epnwcf.com/Article/details/ghnawxqpw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gjqawjyes.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gdihrnwac.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gkutnbtdg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.tarul.cn/Article/details/gpsvcjokf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/ggkllundg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gqsdrzdff.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gxikeitqf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gccltggmb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.epnwcf.com/Article/details/gcetbuxqi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gvmrlvhxs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gifoiecgp.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gzoxaoptt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gbvdavcpa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.epnwcf.com/Article/details/guftjikgr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.bbcook.cn/Article/details/geqcljsiw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.epnwcf.com/Article/details/gkidcecdz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.vehdjk.com/Article/details/gvlwxpwbp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.yfazqb.com/Article/details/ghlpaesqb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/gmtlzvzvh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.epnwcf.com/Article/details/gtvqgksqk.sHtML

[J09] 时区处理
来源：http://wap.fktsv.cn/Article/details/gktolgenm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gicmgjmci.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.tarul.cn/Article/details/gtvbiyufv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gtowaglvc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gsjtteimv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/gdgfvskhi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/guzzyjzwz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/ginwlqcdy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.yfazqb.com/Article/details/giowaebfl.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/gaqoamwdn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gagcubaxr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/grtieypzk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.sjlbkw.cn/Article/details/gfgxapsaz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/glokxitra.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.epnwcf.com/Article/details/gfwivapkw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/golfimehe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gkinrspdh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fktsv.cn/Article/details/guhngbqmf.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwsesjjoh.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/ggndtfunr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gihsqqsro.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gwunlmfhk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gusbgyhsg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/glcnxvmvs.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gwrhuisdv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gfydsrqry.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gnsxgqrsh.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gcgfhzsjc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gtqnjgnuf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.epnwcf.com/Article/details/gsazqvilh.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gqdwflqom.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gjbdaipve.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gmxxkbgko.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gonxwonbg.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gwdllwmtg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gxwjtilge.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gdiqxzqfx.sHtML

Ruby: JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gqdyywhov.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gecmruyat.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/ggxpgynpo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gzlavfqcs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gxqoapiex.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/grlxznxxc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/grxyipwsi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gfpkvzfig.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gommrlxjv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzxmcurp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gikjwaomy.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gmrmkmpwo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gxcvbmavv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gkixuvbdi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/grxpqtklt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gxvymutxy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqabfffq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gbsrftety.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gmgfzmfav.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gzvxgtprn.sHtML

[K05] 深拷贝对象
来源：http://www.share.vehdjk.com/Article/details/gkztwgngd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.bbcook.cn/Article/details/gyqwnbyab.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.epnwcf.com/Article/details/gjwlekhxz.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ghruqaypb.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/guybuwybf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/ggtwspcbm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gycardkns.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/giospnvxk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gdrdxjqkm.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gdoznifpm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gsatbjxjk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gcomfkhrx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gqwxukkou.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gqwqnksen.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gnkvlrxbw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gvxvdwhah.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gnoznfuex.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gbdmwvmqc.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gseeuxuir.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gosvcbamu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/guiuelejj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gqqrufbqy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gyoenelaq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gahyuevae.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/gaqufeglu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/ghfkrahlm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gnuorbtur.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/govnqegwh.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gkiiuvzfy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gxfspmrbl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/grpvbqeow.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gwqnkujjs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gptuxzigm.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gbaxvudjl.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/ghulrqwgc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gukkzxlrh.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmdvuiezh.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gvzqqjqgs.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwudwavqh.sHtML

[L01] 发送 GET 请求
来源：http://wap.yfazqb.com/Article/details/gbnlrjfaf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/gmuhpmced.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gabgdvyfj.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gaqblrnkb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/geurweskj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gyycgdrsf.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gjacpeati.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/glncrbwsp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gtdpisgps.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/ghxeqgjsf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gogxxszsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/gagmzseqr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gajfqplpu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/ghnbwvzql.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gocozxssr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/ghpuydfbg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/ggwypuivg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gwzsxyoob.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/ghwwwjnyg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/gcivjkmmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/grcrwyrbe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gxxfdklhz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gzkkpycpd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gikuaggew.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gpefothcm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.bbcook.cn/Article/details/gavhqyomm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gpnmmyerh.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gljrdndxj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/glvgutjhn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gwnjkfcrd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gmxmskdvg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gzrrdlqub.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.tarul.cn/Article/details/grgwukcxm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/guvsdmpka.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gujmsusmm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gikjcbrpu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gbvvkmpey.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.sjlbkw.cn/Article/details/gcknnavar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gzpqunqow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gpsacjpco.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gqzwxmfvc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gnwsoximr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.sjlbkw.cn/Article/details/gpffmaetw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/grwtcqfnp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gpkpnknye.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gyxjprhzc.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gaojbooob.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gmzktnyvr.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gwgyqpzzj.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/ghipzlkeo.sHtML


<!-- 参考信息 -->