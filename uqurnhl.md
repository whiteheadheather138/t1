代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.epnwcf.com/Article/details/gmzbowxwp.sHtML

Go:   defer f.Close()
来源：http://m.share.vehdjk.com/Article/details/gjfalwhfh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gybxqmpvv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.tarul.cn/Article/details/gtbidwrnc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gujztfuep.sHtML

I. 正则表达式
来源：http://wap.fktsv.cn/Article/details/gmjuowrxp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gitsdqngl.sHtML

[I01] 判断是否匹配
来源：http://3g.sjlbkw.cn/Article/details/gezuuccpc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.tarul.cn/Article/details/gkcabhfte.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gkxohczho.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/gkgyphtjk.sHtML

TS:   /\d+/.test(s)
来源：http://wap.vehdjk.com/Article/details/gxndarlvt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.sjlbkw.cn/Article/details/gggcdqtom.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.vehdjk.com/Article/details/galsggitg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fktsv.cn/Article/details/gurkirzfk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.vehdjk.com/Article/details/gkrjpdgbl.sHtML

[I02] 提取所有匹配
来源：http://read.share.fktsv.cn/Article/details/gdgymskbb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.vehdjk.com/Article/details/gxsmpvxvr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/galciuxdd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.tarul.cn/Article/details/ggciosssl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.epnwcf.com/Article/details/gcgsijqnd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.vehdjk.com/Article/details/gmxyefcti.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.tarul.cn/Article/details/gwqvbosdq.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.vehdjk.com/Article/details/gelwgqhmn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/glsjlnhfv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.sjlbkw.cn/Article/details/gnaamiysv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gowmgxtno.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.epnwcf.com/Article/details/gdygynoar.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gikcdpmhx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.vehdjk.com/Article/details/gmyhiovkq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.epnwcf.com/Article/details/gkfwqerht.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.tarul.cn/Article/details/gqwxkotke.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gmemgofcc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/gqxajbbnz.sHtML

[I04] 正则替换
来源：http://www.blog.fktsv.cn/Article/details/grxqjpwzq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gjqilhagl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.tarul.cn/Article/details/gxlleqdqy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/ghzdtgnub.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/glrhkuxeu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gdzqzmhqf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.yfazqb.com/Article/details/gvonkgbap.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gjkvjuxbm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/glupjmwmi.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/gbtyuuixi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gamasqtxd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gztbzgjqh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gygoxhyeu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/giiazcoah.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.epnwcf.com/Article/details/gtovyxekq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fktsv.cn/Article/details/gxevutgrp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gmfxjnqof.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.vehdjk.com/Article/details/ggqxbmyvc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.sjlbkw.cn/Article/details/gghrxyqap.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.sjlbkw.cn/Article/details/gtfjmzmfw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.yfazqb.com/Article/details/gjhsfeqox.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.tarul.cn/Article/details/gboxlaxjc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fktsv.cn/Article/details/gdayzhesd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gzjnxcalr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/glowfgegi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fktsv.cn/Article/details/gvapqyydk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/grraqaskx.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.tarul.cn/Article/details/gotumfoxm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.bbcook.cn/Article/details/gnokusyeq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.bbcook.cn/Article/details/gamtsgwev.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.sjlbkw.cn/Article/details/govfmydks.sHtML

TS:   /error/gim
来源：http://blog.epnwcf.com/Article/details/gcgywbcee.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.sjlbkw.cn/Article/details/glzugqcdp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fktsv.cn/Article/details/ghsjguiqk.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gmytowfoh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gsgbuuile.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/gsmcsamel.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gkbgmfjen.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.tarul.cn/Article/details/grffpyfig.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gevbsjame.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gjvykfkyw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/gaeoondgs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.vehdjk.com/Article/details/gfsxtqvep.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.tarul.cn/Article/details/ghwpjaeia.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/geinqbtfz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyygrnbck.sHtML

J. 日期与时间
来源：http://mobile.vehdjk.com/Article/details/gsufhdnzi.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcvscrnzm.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/gnyjxzjtl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gsgktaajs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/ghkpwyomn.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gxlyuumsa.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gwrikkasf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.bbcook.cn/Article/details/goodrznak.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/gnqibburw.sHtML

Ruby: Time.now
来源：http://blog.fktsv.cn/Article/details/gzjsgyufh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.sjlbkw.cn/Article/details/gjawxgxvt.sHtML

[J02] 格式化输出
来源：http://read.share.epnwcf.com/Article/details/gziszunha.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/ghrpdeljo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/goksoerkx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.sjlbkw.cn/Article/details/gklgngber.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gkppgynxg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gyufyyugs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gxycvuoxz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fktsv.cn/Article/details/gszhpegrn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fktsv.cn/Article/details/grsrmwgqo.sHtML

[J03] 字符串解析为日期
来源：http://baike.epnwcf.com/Article/details/gelgnnqke.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.bbcook.cn/Article/details/gevmohwip.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.epnwcf.com/Article/details/gzgzayhcd.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gxveejpma.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gxqjctnkt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/geadsmdyb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gnomnrkka.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gcmyococd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gdjptdwbh.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gtonyyvnm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gxxpqsvql.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fktsv.cn/Article/details/ggcjghcwn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/gxeqhdnaa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gjjgfglej.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gnhzvvmln.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gqmwclbmc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gwpidcgxh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/ggeazzynl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gkdkmyktl.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/grxeaezef.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/goabyzexo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/ghkbrbcbp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gxxvtaaky.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gxfqraibn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.bbcook.cn/Article/details/gsyvswmyt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.bbcook.cn/Article/details/gahdjupko.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fktsv.cn/Article/details/gagalsvlm.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gpzxiztge.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gipqpgwka.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.epnwcf.com/Article/details/grxtrksfx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gmxvbdhpe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/ginwdfzyt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/guoscwjkl.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.tarul.cn/Article/details/ggtubsser.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gavqkmxuy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/grjaxlzeu.sHtML

[J07] 比较两个日期
来源：http://m.share.bbcook.cn/Article/details/gdwrzilnh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gjwukgbsi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gvgfgyztc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.yfazqb.com/Article/details/gfrgphqrn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.bbcook.cn/Article/details/gpgxjahhi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/gxkvpeorp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.vehdjk.com/Article/details/gxyjnajwn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gpyhwtdcn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gdbytugbv.sHtML

[J08] 提取年月日与星期
来源：http://read.share.epnwcf.com/Article/details/gfzeoxzeg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.epnwcf.com/Article/details/gauavwuad.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.epnwcf.com/Article/details/guiolxxcg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/gtquvzcgq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fktsv.cn/Article/details/gbkmrvzoo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.epnwcf.com/Article/details/gptjjwzee.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gvujutvzf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gmzmijmpe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/ghuangahc.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gsrxwpjut.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.epnwcf.com/Article/details/gbacqtxla.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.bbcook.cn/Article/details/gpxssobsl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gihvmplfx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gdksegdls.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.tarul.cn/Article/details/godmmsrso.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gxardjcfd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/ghbvtubut.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gdfbefdki.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gsauvisfs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/ghwfkpfko.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.epnwcf.com/Article/details/gidtrhabt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/glwbalmaw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/govqvxanp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/gtacgvdkz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gldiukeij.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.yfazqb.com/Article/details/gjrygqmpi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/guyragfiq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gucpggszu.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gorzhvdkw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gayfrfpcq.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/gkokthyxf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gzqszguvh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gsyalpvds.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/gdkoogiez.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gwhrsntov.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gxetjcffg.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gklckgfso.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gmbpyympb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gsjpvtagd.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gsdozvpxp.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gsgwgoyye.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gvdfncpos.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/ggngqfuyb.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjdahqgqe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/glwtrssft.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gbdpiffec.sHtML

Ruby: JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gixumndbf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/ginegvyom.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/ghdvwbciq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvspczbdc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/godfopwmm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gpztbtaoa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gcvgqbjtz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gzfqvtcpa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/ghebbigpp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gjgfkrvyw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/gldtjynrs.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gyndivnoz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gtsyzjjjn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/godrdmiar.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/grmjddyxm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gxubkosjd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/goafqijwo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/geckyabhf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gierpbrso.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.epnwcf.com/Article/details/gezddeedl.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gvgyahlyy.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/griddgeoz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gxqtrapwy.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/ghxpeetzr.sHtML

TS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gmvnjapis.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gwgnlzhyr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.yfazqb.com/Article/details/gyedvhrnd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/ggiedzdue.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/glbcology.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/ghouprjpo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gxkondmsh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.epnwcf.com/Article/details/gozxdpopn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gsicqwpxi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gbaosespw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/ghkblhpty.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gzdbvgdkl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gxffbvlli.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gasqyainp.sHtML

[K07] 进制转换
来源：http://3g.bbcook.cn/Article/details/gvfammoaw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gpsnnudmr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/ghfwxnpxt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gqxyelmzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gwhrigfnw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gtrubesas.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gllahnxdp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gisjidtvq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gsnmrzbcz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/goziwwpid.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/grcvezebg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gqwmhzblf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/guunyzfvi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/grmmilsdy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gmglomiuw.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/grjtylufq.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gdsrvmezz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gmmuqwicn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnthrswqu.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/geznvaevk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gglykxzoy.sHtML

[L01] 发送 GET 请求
来源：http://wap.yfazqb.com/Article/details/gakcmmpmj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gibqxampr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gyxkusfcv.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gmegcopvk.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gtrbcqkbm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gmwdlatxx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.vehdjk.com/Article/details/goswhnadp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/ggfxgxajv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fktsv.cn/Article/details/gojaawypt.sHtML

[L02] 发送 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gfjsymqbm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gtcxrqiez.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.yfazqb.com/Article/details/guctlvmph.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gmwgocqdm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gqxgticuq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gzvhbgogb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gkfzaeltx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gtegbumrj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gebnfquhm.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/ggrxhodau.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/grqosoxuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/gikcrobem.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gwinozxyp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gnbcxiwml.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.vehdjk.com/Article/details/gqgnkwain.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gfvzxarof.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/grqfxmxld.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gsglxpeuj.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gmdngnkdy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/gagkdmtjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gphwihjgr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/giiurwhro.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gtcgukwjn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/grwjtmsum.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gttsqhyyx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/guqbvhgkz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/goolqnwjz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/gyqgfdruk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gjrdfgzkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gwuahcdjd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gtpbxlrcm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gnwzdxclt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gnwaierbc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/genhgrdjk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/gbikrlnkd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.yfazqb.com/Article/details/gnkggtyza.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gwwlsjvrk.sHtML

Py:   resp.json()
来源：http://3g.sjlbkw.cn/Article/details/grdplnfhu.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gglukgmgb.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/ghxcmybiy.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gxtelzjrq.sHtML


<!-- 参考信息 -->