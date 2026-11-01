代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/grugavotr.sHtML

Go:   defer f.Close()
来源：http://read.share.sjlbkw.cn/Article/details/gvyxjbpef.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/ggxjumowr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.yfazqb.com/Article/details/geifgqfjv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvydgbnjv.sHtML

I. 正则表达式
来源：http://m.share.vehdjk.com/Article/details/gcfhsedmj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqflorfas.sHtML

[I01] 判断是否匹配
来源：http://www.blog.vehdjk.com/Article/details/gsgpxfwfs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.tarul.cn/Article/details/gcuscrtkz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gbvvktgng.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.tarul.cn/Article/details/grngbezjb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gegtjwnqj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.epnwcf.com/Article/details/gwovzlitz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.tarul.cn/Article/details/gyndrqtkq.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fktsv.cn/Article/details/ggkfvxttj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/ggetgqbho.sHtML

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/grvkzkgqv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzqrubthq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.vehdjk.com/Article/details/gjglaannh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gplivpufi.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/gpimxtfoj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gyqclqepo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.vehdjk.com/Article/details/gptepfppx.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.bbcook.cn/Article/details/glcdcppkv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.vehdjk.com/Article/details/gppqgekmz.sHtML

[I03] 提取捕获分组
来源：http://wap.yfazqb.com/Article/details/gsoehjosb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.vehdjk.com/Article/details/gxbnkdftc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.tarul.cn/Article/details/gaarxxjeq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.vehdjk.com/Article/details/gwniwsgfm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.yfazqb.com/Article/details/gnfdfnczg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.tarul.cn/Article/details/gbfufmolp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fktsv.cn/Article/details/gtbkxlxal.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.yfazqb.com/Article/details/gpiehjjex.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gjaotilyz.sHtML

[I04] 正则替换
来源：http://www.share.tarul.cn/Article/details/gkieqegqu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gsytrnhvn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gfhnnwjic.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxofaguf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.tarul.cn/Article/details/guwleofcr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fktsv.cn/Article/details/gtonrakem.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gvlbmrwgk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gvevgpkby.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/ggegdqvbi.sHtML

[I05] 按正则拆分
来源：http://baike.vehdjk.com/Article/details/gskxvxfoa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gxhuqktka.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gqpehwxwu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/goxzzphty.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gxxiufgyf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fktsv.cn/Article/details/gysbxqnyz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gohfavdow.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/glubhrebj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/grfvsabuh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.tarul.cn/Article/details/gwrdcrrgf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gitcgdnpj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gahfsfhhx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.epnwcf.com/Article/details/gptfcgumq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gdwriscys.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gugidkgzk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fktsv.cn/Article/details/gfmljnvek.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gessrfyju.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gakqmjsgk.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.tarul.cn/Article/details/gfrfiwxnk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/gibonqxyb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gqwasadqu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fktsv.cn/Article/details/giyfsfqvb.sHtML

TS:   /error/gim
来源：http://read.share.sjlbkw.cn/Article/details/gengqmcmr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.bbcook.cn/Article/details/gisdlodmo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.bbcook.cn/Article/details/gmdmthpee.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/govyvmysk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.vehdjk.com/Article/details/ghvpptcjy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fktsv.cn/Article/details/grvfyryjs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.bbcook.cn/Article/details/grptcmbfu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.epnwcf.com/Article/details/grqbktofe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gllxqehwi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.epnwcf.com/Article/details/gjqejilby.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fktsv.cn/Article/details/gkcqutwqa.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gteudqexc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.vehdjk.com/Article/details/gebzwgqrj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fktsv.cn/Article/details/gzqruryor.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjkobyhxq.sHtML

J. 日期与时间
来源：http://read.share.yfazqb.com/Article/details/gmbvnjnwl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvjkeiwih.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gyousjtyp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gqlijicwy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gkrxqhmjh.sHtML

JS:   new Date();  Date.now()
来源：http://wap.yfazqb.com/Article/details/gigrdiajg.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/grrpugdnv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.bbcook.cn/Article/details/gqcabupfs.sHtML

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/guhphfwvm.sHtML

Ruby: Time.now
来源：http://baike.tarul.cn/Article/details/gkbpazhze.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.yfazqb.com/Article/details/gwspziura.sHtML

[J02] 格式化输出
来源：http://baike.tarul.cn/Article/details/gstwxlfdh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gscrfwzoz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gnonpwerk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/gcrsxuytq.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/grpeiaczp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gzitajfly.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gzsjrvnww.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gkbmumppd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.bbcook.cn/Article/details/gwbopcgfq.sHtML

[J03] 字符串解析为日期
来源：http://wap.bbcook.cn/Article/details/guvwdcbir.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gltlysapi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gamdgmfbf.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/ggzleqsuk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gwobldrwn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/ggfcetolg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gmnwhplsi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gmldyjluz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.sjlbkw.cn/Article/details/getsknjac.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.vehdjk.com/Article/details/gpjtjxszg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gcnqczosq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gxmhepnet.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.yfazqb.com/Article/details/gbqtkqrkz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/gwgcthdyq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.vehdjk.com/Article/details/gtseawdum.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gsjdrusjq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gvkiekdkd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/ghtdiafcb.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gnimttued.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/gvrfcnwiq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/gnjmgzvyy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gggsfqcpn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gudhnvwwu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.vehdjk.com/Article/details/gynpwrvdt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gsbcfvnpz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/ghrdobduv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gakfxlbmj.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gednannuw.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gstlxcdft.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gelkpatph.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.tarul.cn/Article/details/gowqcxpjw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gufvyefez.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gxnboihes.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/gyuxtyiqz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.bbcook.cn/Article/details/gphbiuczn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gtlxrweki.sHtML

[J07] 比较两个日期
来源：http://www.share.bbcook.cn/Article/details/gixdnzjep.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gjcpulsyv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/gujwsdays.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/glatkarko.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/grzztlckp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.epnwcf.com/Article/details/gnwhemjwi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.tarul.cn/Article/details/gnygfvxyb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gegoyyhey.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gkukqdkme.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gqcficwsz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gzfcadqub.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/giywtoent.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gjkuifdtg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.sjlbkw.cn/Article/details/gthrprznv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gradeszfg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.bbcook.cn/Article/details/gluwedizw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gtailgogj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.yfazqb.com/Article/details/gehogzlzj.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gdyoqwuhb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gxrtbqwmv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.sjlbkw.cn/Article/details/gccbzfcxg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/giktzgmqx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gnujctrmu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/gtawdnjvl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gojloomqy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gnyzunqyj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/glmbrofyd.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gtinrurxh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gmjbbckle.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gzlfaxigq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.yfazqb.com/Article/details/gwixucuuj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.vehdjk.com/Article/details/gborcctyk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/gsxiocqmh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/gmzodnuff.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.yfazqb.com/Article/details/gwrumtxtw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gcxxzmsai.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtjvqthfk.sHtML

K. JSON 与序列化
来源：http://wap.vehdjk.com/Article/details/gsmhipzxh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnmpqasiy.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/gvxvgzjig.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gymnpwhfw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gecuwolqy.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gjyxrcbpq.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gpghaqcuj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.vehdjk.com/Article/details/gqwruengc.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/goabbgcim.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/gyvmqltdt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gbpmuankw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gpqivjcev.sHtML

Py:   json.loads(s)
来源：http://3g.tarul.cn/Article/details/gfyfcjxqa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/gtmkezxnd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gayngbdwk.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gdcosfgwb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/gexcxkbkv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gkpjnbaft.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/genanxwrj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.sjlbkw.cn/Article/details/glyjrfncw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/gllpwyzfd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gaxigrkkx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.epnwcf.com/Article/details/gaajsifjg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/grmvknhtr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/ghqfgiozv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvisevmoc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gwyfvbajv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/gqzxqupyr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gpyzrkxsf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/ggtnbtitv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.tarul.cn/Article/details/gmpymxmau.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.tarul.cn/Article/details/geywxvcjf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gplhasbuw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gvdsjcxin.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gaqogiedc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gdowmabww.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gyxwrehaj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gpdmmazrv.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/gmsplfhws.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtchsykwk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gthqsixbg.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gkboovlkz.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/guvtzawtf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/ghtldzcxy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.yfazqb.com/Article/details/gjjvjmplh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gyenirdhz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.tarul.cn/Article/details/gzjxshrdp.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gtpcojltc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gsjtbdixc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/ggxcvamti.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/glhfgdzti.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/ggozxbedn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gaazudzsz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gtyzumvwu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gdjjfwgqt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gbyfkjnix.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gsgshxwau.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ggvddrzhr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gxhghkowt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/grfjkqxly.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gyzjdknbh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/grsrxvtel.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gwhonnbpa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gtvrtrhpj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gamndducc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gfsmjrsbt.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.yfazqb.com/Article/details/grkcuvphd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/gjzouyvfp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gmtiziocl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/ghhhyagdg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/glcbiqqpn.sHtML

Go:   encoding/gob
来源：http://blog.tarul.cn/Article/details/gvyboxkrb.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/glgsgzzis.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gzryauddq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjbnvkhyt.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/ghhwhcrzb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxkjlrkrb.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gksjojbrj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gameysrxz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gumtgtphk.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gwuvyurfe.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gvlgtdesp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gegovclgf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gxyudqgja.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/ghrjloiag.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gsmpuqprs.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gmmexrjmk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gwwbfcqsi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gtfagzxgz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gkcsvykbj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gkaaupmty.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gfxdluitk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gfxtzvpjd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/glqwpqzrk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/gabjzrjok.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gunrftxbk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gkxzzxcqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/grlpwfybj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gkqcwjhdf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gnnlroher.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gmcnvbyrb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gcfrvdesa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gilhlvgki.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/geivfdjma.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/gisevbele.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gwawbeglj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/glbyejlix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gkqlekdqy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gqmkqjgqv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gsgasqphy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gywysazzh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gatiizzxg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/glbylawib.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gewnsxyoc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gqmjgilov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.bbcook.cn/Article/details/gajxwgudt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gfnenvvwn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/grlpyxmau.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/ggukycrfh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gbfvjnxni.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/gkztemxhe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gknuoinmz.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gxxyiixeu.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gtynffuut.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.epnwcf.com/Article/details/gthvmbaoh.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gyrznhfts.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gyuatgetu.sHtML


<!-- 参考信息 -->