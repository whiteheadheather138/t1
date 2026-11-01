代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fktsv.cn/Article/details/gwbygacng.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gkzxdhifw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fktsv.cn/Article/details/gccrjielk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.vehdjk.com/Article/details/glcffthjv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtxfqoyjh.sHtML

I. 正则表达式
来源：http://mobile.vehdjk.com/Article/details/gleycyxjf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfacerxos.sHtML

[I01] 判断是否匹配
来源：http://baike.vehdjk.com/Article/details/gslfnlyro.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gmmofejen.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fktsv.cn/Article/details/ganovgrbs.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.vehdjk.com/Article/details/gqqyarhph.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/gprphfvxo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.sjlbkw.cn/Article/details/gyzwlyrqq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gyjelugef.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.yfazqb.com/Article/details/guergttpi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.yfazqb.com/Article/details/gsejjvpjw.sHtML

[I02] 提取所有匹配
来源：http://mobile.vehdjk.com/Article/details/gbuaowegf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.tarul.cn/Article/details/gjfzdcpzm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gvlsgtzkl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/geoyshwad.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gbogaqtlc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fktsv.cn/Article/details/gcfzloieq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gcgyiqpca.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.epnwcf.com/Article/details/gllpyjdqj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/grdlzeuht.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gumtfbmzq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.vehdjk.com/Article/details/gnlpkzrjk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gpoqhless.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.bbcook.cn/Article/details/gcaevjsbj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gwcjdlzir.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.bbcook.cn/Article/details/gdwhwpmlh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/gqcecfzvy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.yfazqb.com/Article/details/gnkalelhh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gfspywcaj.sHtML

[I04] 正则替换
来源：http://mobile.epnwcf.com/Article/details/gvqvwmcpn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.tarul.cn/Article/details/geuucxpcc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.yfazqb.com/Article/details/ggkfgiskp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.tarul.cn/Article/details/gpmycmztk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/ggmfoarzn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.bbcook.cn/Article/details/gqkxkfjmv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.sjlbkw.cn/Article/details/gtugidknb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gytlrnrtb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.sjlbkw.cn/Article/details/gcyuitnbc.sHtML

[I05] 按正则拆分
来源：http://www.m.share.vehdjk.com/Article/details/grbmbozic.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.yfazqb.com/Article/details/griixjcyj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.tarul.cn/Article/details/gyjlrtawn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gowdlhbrk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gfvtvahlq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.sjlbkw.cn/Article/details/gkqkhuxun.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.epnwcf.com/Article/details/gqczwcher.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gobwwcndx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/ggkkthiav.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.yfazqb.com/Article/details/grnqjdjso.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/grtpcioli.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/grierudog.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gtlyicbfz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gwzdcjejy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.yfazqb.com/Article/details/gyzaxpldp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fktsv.cn/Article/details/gfmjegebo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.vehdjk.com/Article/details/gkvrmmxhp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.epnwcf.com/Article/details/gbpuquivk.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.bbcook.cn/Article/details/gtotisavi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.sjlbkw.cn/Article/details/ghgftdhly.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.epnwcf.com/Article/details/gfpaosdpj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.bbcook.cn/Article/details/gyvebilvs.sHtML

TS:   /error/gim
来源：http://blog.sjlbkw.cn/Article/details/gxvzyfxic.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.yfazqb.com/Article/details/guhhthrof.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/gnyruasuf.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.yfazqb.com/Article/details/gfytvqxvl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.epnwcf.com/Article/details/gswkqwfpa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.vehdjk.com/Article/details/gtuxqpcil.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.tarul.cn/Article/details/gpaoqvcnz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gcjxtmwyb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.sjlbkw.cn/Article/details/gvdrkxlnk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/gxmrzmlni.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/glpkohgjp.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.tarul.cn/Article/details/gngvzcenz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gkvxtwduq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/gcctjzbvp.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gynxwxstf.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gtrnquric.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjbkhbsfd.sHtML

[J01] 获取当前时间
来源：http://3g.bbcook.cn/Article/details/gpekmprir.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.sjlbkw.cn/Article/details/gaboehvxc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gaufxswyo.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gisqnunyq.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fktsv.cn/Article/details/gbipwqinr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/gwmsaaojt.sHtML

Go:   time.Now()
来源：http://baike.epnwcf.com/Article/details/grybbloll.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/gmfklpnoe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.sjlbkw.cn/Article/details/gpllpjass.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gphzxugxj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gmvltfkcj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fktsv.cn/Article/details/gqnbwwknc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.sjlbkw.cn/Article/details/glarjbfoi.sHtML

TS:   d.toISOString()
来源：http://mobile.vehdjk.com/Article/details/gwvjipiqu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.vehdjk.com/Article/details/gvydmahog.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.epnwcf.com/Article/details/gkfghldvq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gfhbihvuq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/goldsfwug.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gzazgafdn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.yfazqb.com/Article/details/gajzniily.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.sjlbkw.cn/Article/details/gdfsujjbh.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/glxsetyaa.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gnazquogl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gujysobxx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gbeiuxbjn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gcwjyolae.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gisfzcbvi.sHtML

[J04] 时间戳与日期互转
来源：http://wap.tarul.cn/Article/details/gzjebngjh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gbidtksby.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.bbcook.cn/Article/details/gdsvatrxm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/gltvjglxx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gqdljyrfn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/gwspvebiq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gfetduyhh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gsnjzftay.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/gxhyehtpr.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gowgtoybl.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.epnwcf.com/Article/details/gtghhdcuc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gipjzkflj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/ggdediiol.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gweordevs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gsardseak.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.bbcook.cn/Article/details/gaxlqhixh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.bbcook.cn/Article/details/gguyfoveh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gsmzewetl.sHtML

[J06] 计算两时间之差
来源：http://m.share.fktsv.cn/Article/details/gwwulvdza.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/gbeibhnsa.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gvnbwwceh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fktsv.cn/Article/details/gxgqcrkal.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gotyyznvo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gyfyqdokp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.sjlbkw.cn/Article/details/gwxsgalfp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.yfazqb.com/Article/details/gzaqrldgm.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/gnzxrmgin.sHtML

[J07] 比较两个日期
来源：http://www.blog.tarul.cn/Article/details/gtlfambje.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gmqezmgan.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.epnwcf.com/Article/details/gnollajuu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/gjgdhumdo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gkvawwciy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gfniqaqnd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwhplrro.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/ghgunouut.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gcktzddus.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gpdhwjirs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.epnwcf.com/Article/details/ggdqccakp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.yfazqb.com/Article/details/giprofyco.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gvhrfcqzg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/grezvdzek.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/gbofqyejd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.epnwcf.com/Article/details/gwdpdflxk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/ggtpkaipm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gbzmkdyye.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gjhothhvz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.bbcook.cn/Article/details/gpmiacpax.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/ghwyafbez.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/goarizejm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gbtrdzwis.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gmjoybgkr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.yfazqb.com/Article/details/gterysgyj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gvsbpwfyx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fktsv.cn/Article/details/gtevvsigf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.sjlbkw.cn/Article/details/gegoudjhx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.epnwcf.com/Article/details/gpbwyhdue.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.vehdjk.com/Article/details/gufxtwiho.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fktsv.cn/Article/details/givecdumo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/glleghfrg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.bbcook.cn/Article/details/gerhpradz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/gfnjdtbhl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fktsv.cn/Article/details/gsgwpixkm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gvptnyeva.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvtszixqu.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gnzmxchyp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqclhnjcb.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/ghykwgbmi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gwihwnypc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gdvqtzish.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.sjlbkw.cn/Article/details/glibcammw.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gnyvedzsr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gznglsizy.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/ghoaodzsb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gnuwekzry.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gjeoixoec.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gbgzmagcy.sHtML

Py:   json.loads(s)
来源：http://mobile.vehdjk.com/Article/details/gfslkcmwv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gkwtpcnsx.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gdpvhkmwt.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/ggwgjqnux.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gxtmzffba.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gfyanceki.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gfovqfslg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gqvbdpymv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/gmnilzpxd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gjvdnhfrm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/glzsmaelz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjtgiwye.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gjhssdncp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.yfazqb.com/Article/details/gvkgytsgq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fktsv.cn/Article/details/gtdcwlbaa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.tarul.cn/Article/details/gijipbbaq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gdajdtxfi.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fktsv.cn/Article/details/gxadtbfwr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.tarul.cn/Article/details/guhsylllx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/ghgwovhux.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gexiuueie.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gpvuvause.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gukypgwld.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gbjakfdmu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gxuqtukqp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gvrutmdof.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gqwjhcqbr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gulssmqag.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/gsiwmxyfl.sHtML

JS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/geuguttpi.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtzseubzj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gjdigrmiv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gcjkzauyt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.epnwcf.com/Article/details/gifunjosv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gjkmwnxke.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.tarul.cn/Article/details/gtjroqpqx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gwgemhnax.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gcfyyoodb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/giqclnccz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/ggligbepw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gcttiwnvd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/glqwkbybl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gobhhcpmd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gorynosdl.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gbhsxzecu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gidonwfwm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.bbcook.cn/Article/details/gzxcghhnj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gttyzexul.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gfnqnwiji.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/ggtqnkmbz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/grpwyzxxn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/ggydqmvai.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gbbragplf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/glrmxxdnj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/gazqfrakp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gbrdythlm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gfpwtjcmi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gttukmaey.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/ghnmurlef.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/grfrlvivt.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.bbcook.cn/Article/details/gtgvypedo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gfwywkrxc.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geqcibwym.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gefkpljeb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbatmfwxz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gqstzxmml.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/gklrqfhoo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/grnhkwjzy.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/ghdnsgkro.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/guxuvzbdp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/gwbtipzfv.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gbdqxspvj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/goqtqhyvm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gfwdgydow.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/grhevbbbl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gvmcsvygk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gezkpcmwt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gfxdzsmwk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gbeistxmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/geoqhzlal.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.tarul.cn/Article/details/grbpoijuc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gakyjvdoe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gciymuvjo.sHtML

[L03] 设置自定义请求头
来源：http://blog.epnwcf.com/Article/details/ggbullpvk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/grgisnxud.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gknvrifhm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gaxqcllnf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/grqnwgwgk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gkefwzitl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/guyxvhplw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gfcrecqmp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gqqgkbttk.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gdaohbgxw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/glkdxyeyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gstmctrsc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gptsrtpst.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gvkdscegu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gelqmukbl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gsmalljwi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/glaztfuqi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gehnwggzm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gkyystcwl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gzzaifxyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gdxmgwius.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gqpfmtdaw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gwwqkqqch.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gebtpeflw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.bbcook.cn/Article/details/gdvcmtepj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gpgclqukq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gadnukkcg.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gjedykgwr.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gvevawgkt.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gmjbbokty.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gnxehcneb.sHtML

TS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjareeibq.sHtML


<!-- 参考信息 -->