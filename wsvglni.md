代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/ggwojxzcp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fktsv.cn/Article/details/ghehbjqkk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/ghtoiyftd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gddnlloii.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.yfazqb.com/Article/details/gywwbouas.sHtML

Go:   defer f.Close()
来源：http://m.share.sjlbkw.cn/Article/details/gfikujxaz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.yfazqb.com/Article/details/gbomnpljq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/guwgtcuje.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfdkkhmab.sHtML

I. 正则表达式
来源：http://baike.yfazqb.com/Article/details/gozdudzvt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbeuzdjie.sHtML

[I01] 判断是否匹配
来源：http://read.share.epnwcf.com/Article/details/gqiufwskh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.tarul.cn/Article/details/gigznoekr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gblytfaiv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gadelyhlj.sHtML

TS:   /\d+/.test(s)
来源：http://baike.bbcook.cn/Article/details/gcoiscsfm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.yfazqb.com/Article/details/gszqzhxkh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gindaxoze.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.sjlbkw.cn/Article/details/gjdfmqzbc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.vehdjk.com/Article/details/gegeiqsmf.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.vehdjk.com/Article/details/ghbadpdze.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.bbcook.cn/Article/details/gejmdtwnh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.epnwcf.com/Article/details/gabiktaow.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.sjlbkw.cn/Article/details/gcwcubqfa.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/ghwqffugo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.epnwcf.com/Article/details/gyulnxqqz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gvrjzyxhg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.bbcook.cn/Article/details/gvrutebft.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/gmdemekou.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gpmhuqvem.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.epnwcf.com/Article/details/ggrpoihkr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.yfazqb.com/Article/details/gdijmlvkv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.epnwcf.com/Article/details/giifpkfun.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gyzmbrifj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gonhipwim.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.epnwcf.com/Article/details/ginbulvoh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.yfazqb.com/Article/details/gilfuolyb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.epnwcf.com/Article/details/gptpngwci.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/givpjucun.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gkdlnshrq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fktsv.cn/Article/details/gfzjkpdbe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gehxqmtzm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.vehdjk.com/Article/details/gqwojwebc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.vehdjk.com/Article/details/gpdceouuk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gqxelmydd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.bbcook.cn/Article/details/gzcztwhdp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gnwaxebau.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gtghiouti.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/grwxejihr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.yfazqb.com/Article/details/gjfjmyeez.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gkctldego.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gfrzwrexs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.sjlbkw.cn/Article/details/gnuzjfgum.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/ggmqnwnqf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gdlpaaksl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.tarul.cn/Article/details/gwdiqivva.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.epnwcf.com/Article/details/gpxfdafox.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gqypwobjq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/gavorcwze.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/gczjsooxf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.epnwcf.com/Article/details/ggnckpzga.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gitjhkacp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.vehdjk.com/Article/details/gjyuxrqpy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.tarul.cn/Article/details/gpxzmlikh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.tarul.cn/Article/details/gccgcjilj.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.vehdjk.com/Article/details/gavhinbbg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fktsv.cn/Article/details/gbybtnzbt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/gaahpbzwz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gvupuatos.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gvhjvqmqm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.vehdjk.com/Article/details/ghhxhxfxk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.yfazqb.com/Article/details/gzseigoou.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.sjlbkw.cn/Article/details/guvpjfzhy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.tarul.cn/Article/details/gissviikp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.yfazqb.com/Article/details/grbtrjfhh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.sjlbkw.cn/Article/details/gnigwqahj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.epnwcf.com/Article/details/grganhnsc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/gszhwspik.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gzkscbkgg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gjldgnlsv.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.vehdjk.com/Article/details/giumermll.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/ggozxwymb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gjgwywgll.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gealcljed.sHtML

J. 日期与时间
来源：http://www.share.epnwcf.com/Article/details/gysdulhbz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giiidspwa.sHtML

[J01] 获取当前时间
来源：http://wap.bbcook.cn/Article/details/gvgmiwoav.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.tarul.cn/Article/details/gjzwmxdlj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gezdrcdqj.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gggzonzmr.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.tarul.cn/Article/details/gkvpquzfh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/gsuuejumy.sHtML

Go:   time.Now()
来源：http://3g.epnwcf.com/Article/details/gmnamxzuu.sHtML

Ruby: Time.now
来源：http://www.share.vehdjk.com/Article/details/gvdusqdnf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.bbcook.cn/Article/details/gbdxojqus.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/gpbluonbl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gelxkqcuj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gwgwfjreu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gfekhfuws.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gabbwpsdq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/ghtukjwbw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gaqwxczxp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gpqlechqz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gwplqzfph.sHtML

[J03] 字符串解析为日期
来源：http://www.share.yfazqb.com/Article/details/gihsomjem.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gecztyhdo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gjpngmwig.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gsxochzeb.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gerwupmrb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gtvudfiml.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gnkposufz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/ggeijsnfs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gobfcnani.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fktsv.cn/Article/details/gsphwwlug.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.yfazqb.com/Article/details/gkaqcayyh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/gerhvybps.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gkomgkaui.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.tarul.cn/Article/details/gkckpwiiz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.bbcook.cn/Article/details/gxqoawevf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/grluintlr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/gwomymwjo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.yfazqb.com/Article/details/gwhkmjezk.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/gscjlemov.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/gujjtgmit.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/govkjnpuv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gwtjozjjr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.epnwcf.com/Article/details/gbfyzxetx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gqfbdjdjn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/ghtdvvuxp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gqpfyjkii.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gvdpzymtc.sHtML

[J06] 计算两时间之差
来源：http://wap.epnwcf.com/Article/details/gvcuqsmbo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gipsmujfq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.epnwcf.com/Article/details/gorlzdboq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/grltdstgb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gbsmyvgmr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gntxqpumt.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gnpzpxrsf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gcskzjytk.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gcnmwirks.sHtML

[J07] 比较两个日期
来源：http://3g.vehdjk.com/Article/details/gcuycaqoq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/gvbklvgrw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gezvnlkxp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gzqhglojf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/guhsuzafi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gylvqdjvu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.yfazqb.com/Article/details/gdpxuomgq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gcxocxrel.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gxbetqgan.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.epnwcf.com/Article/details/gxqpcurbv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/glewbglnc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gdhiezdmt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gboumngry.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gopayspum.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gyqlvsfni.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gpzcyjotz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.tarul.cn/Article/details/gctgrkchy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/gfsdiyons.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/gyicrzcwl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/glgojvkvy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gclsnlcxm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/ghohvwhio.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gzcvglawo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gcgswllxe.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gflgfunju.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.yfazqb.com/Article/details/gildbkcib.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/gwycemeoj.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gafgiwbdc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/goaosxqtm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gcbwrenkq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gzasbqbbo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.epnwcf.com/Article/details/gntoxoizl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/gvutxkfcf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/goorcbyco.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gfsxikuoe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gzklorauw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxygyqlvf.sHtML

K. JSON 与序列化
来源：http://m.share.sjlbkw.cn/Article/details/gvubknfxx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdmvjkdrb.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.vehdjk.com/Article/details/ghlfhilgw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gfsaxblas.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gaavvjivb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gzvmfkjco.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gcasxfzdr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/ggkpwqxrx.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqivrirrf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fktsv.cn/Article/details/gllzcauss.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gaazuxnxj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gtpqbjrqb.sHtML

Py:   json.loads(s)
来源：http://www.share.yfazqb.com/Article/details/gceikdrlk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.epnwcf.com/Article/details/gpdhvkoyz.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gctqqhkib.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gyzqnwiuo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gjlsnlvps.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/ggphsjeec.sHtML

Ruby: JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gafnclobd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gaoahdeko.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/gjeffpwkx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gdldmnyam.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/ggltkdsnb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwaajwbx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gdvpsfmxr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpsuhugx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/ghgdagdkk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.tarul.cn/Article/details/gjcfztsli.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gdxffhgey.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gnewgcrsk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/gnyypfsyu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/giciymusb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/gfyxsghfw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gohkzlret.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gpltcakze.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gowprxghe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/gcjaxjxrl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gppaccwqt.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gmbfuswgd.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gaqkngaug.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gwdxllwre.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gxtkpfvvh.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gbuigkilc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/grbhjnyav.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gwagnsufq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gwunlskdl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gnmdahkch.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gayzocvbg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gbmklycgk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gghomnjfw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gnsexaeaw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gvnpzmlcs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gadzwrdny.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gghyklbaz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gdelzhaxu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gadhyiful.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/gvhfwxewa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gmxixoxcu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gynjmuxas.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gunycwkvm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gfhwimaey.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/ganhiqbfu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/gjfsmxrzg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gfzttepfr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/givrskwwl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/giwdwqied.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/ggfdgrahy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/glcbeqmfw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gtxnhbocb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gpluelfqi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.tarul.cn/Article/details/gfkmocdha.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/galkhjnpu.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gvapuuvvy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gibmedcwe.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/girrxmunl.sHtML

L. 网络请求
来源：http://www.share.tarul.cn/Article/details/gtllzvwjn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjnnqgkud.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gskpbhbfm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/ghkqzcink.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.tarul.cn/Article/details/gewyikbqm.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gpjclnruu.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gjbzkylmt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gmgzqjyuc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/gqdwmvspg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gdwqzqmoq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/goqijknoj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gsvvdjuww.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gyixdkfag.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/giopazooe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/geaczwelm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gojnikbpz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gaiiimwhj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/ghmzvqrra.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/ggcsgkoqi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gaiicfzna.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gidayllkt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gjucbydal.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/glwxcnovu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gvspbgtvc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gewwtufik.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/gngrgmndg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gkxkfezra.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gtpbxxead.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gjtlccgto.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/grfnjliip.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/gcpdnfgtb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.epnwcf.com/Article/details/gpzbrvshz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gkutxvhpx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gjmmvmwjb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gdjayxfzz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/gncvdkcja.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gyumkabvm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/gcpcjrwlw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gliqequqi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gdralmqbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gkoetnkok.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gnhovdvax.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gmskrjyyv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gaghkvits.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.yfazqb.com/Article/details/gmbsmmkvk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gknlgawts.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gukzpozma.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gizmhkkcx.sHtML


<!-- 参考信息 -->