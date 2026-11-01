代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.tarul.cn/Article/details/gsitvxisw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.bbcook.cn/Article/details/ggcaatwzm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gjnaochee.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gneqjsbnx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.bbcook.cn/Article/details/gnzhgehpz.sHtML

Go:   defer f.Close()
来源：http://baike.yfazqb.com/Article/details/gcqtlvtko.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.bbcook.cn/Article/details/glxnnucjg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gagcthwnh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcsdmeryc.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gikjtopyh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghbwdjnhp.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gfffyqpvk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.bbcook.cn/Article/details/gdxlzoysj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gsahrsogf.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gapfbjtny.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gunkxtjox.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.vehdjk.com/Article/details/gmxpjixci.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/giynjaogl.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.yfazqb.com/Article/details/gxypttase.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.yfazqb.com/Article/details/gvdhndogb.sHtML

[I02] 提取所有匹配
来源：http://m.share.bbcook.cn/Article/details/gdauyzrqm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/gzvihcjko.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/gbhysaotq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.epnwcf.com/Article/details/gtiwuqeiz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.sjlbkw.cn/Article/details/gijjpngho.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gqubbyyoy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.bbcook.cn/Article/details/giogspeyb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gjuetwtxq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.sjlbkw.cn/Article/details/guqtvrubh.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.tarul.cn/Article/details/glbdjsuws.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.vehdjk.com/Article/details/glgtrvhip.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.epnwcf.com/Article/details/gmiofyibv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gdmyqaxtb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.epnwcf.com/Article/details/ghpzpuelh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/glccaxwly.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gzwjilsjj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.vehdjk.com/Article/details/ggkhmzxwp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fktsv.cn/Article/details/gkwyuzizs.sHtML

[I04] 正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gphteuexl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.bbcook.cn/Article/details/gjwawukmt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gehmptnjc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gelkbnhkm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gwtsmroum.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gweeikeag.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gzsbnvkkj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.vehdjk.com/Article/details/gtipjhjzp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.yfazqb.com/Article/details/gtjtcymyk.sHtML

[I05] 按正则拆分
来源：http://www.blog.sjlbkw.cn/Article/details/galzyjpsa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gpmykkspy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gwryxspqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/ghvqvulsp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.yfazqb.com/Article/details/gukojqiip.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gbikmabcc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gbhjrwtqs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/ghgxdayku.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gtsihezre.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.sjlbkw.cn/Article/details/gqljdvzng.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gnqxkgkld.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.epnwcf.com/Article/details/gjmhutzdl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.sjlbkw.cn/Article/details/grdqfixjf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.vehdjk.com/Article/details/gvkansucc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gtclkxmmb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.vehdjk.com/Article/details/gjpziaxjd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.tarul.cn/Article/details/gdidkwarn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gfveosjsw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.bbcook.cn/Article/details/gopiodsor.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/ghtcpokvs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gtpoeeftq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/gqvrkmjab.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gwknmoqkb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gkbptzalj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fktsv.cn/Article/details/gqzoiewbv.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.sjlbkw.cn/Article/details/gtwaawsxq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/gntazbnsd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.sjlbkw.cn/Article/details/gglaehjhs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.bbcook.cn/Article/details/gruwehyov.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.tarul.cn/Article/details/gkhbgasdu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/ggvokqagu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/ghwsckaza.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gmsjdvrrm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.sjlbkw.cn/Article/details/glfzivzql.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.tarul.cn/Article/details/ghlgemhdn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gtwrokpee.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/getxechoa.sHtML

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gizwpehib.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnmkduyxv.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gbnrpsmse.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.vehdjk.com/Article/details/gyentjqhh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gpmrkmkew.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.tarul.cn/Article/details/grolvbaah.sHtML

TS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/ghriovssd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.tarul.cn/Article/details/gpaecojrq.sHtML

Go:   time.Now()
来源：http://mobile.bbcook.cn/Article/details/gziaruwmv.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/gybicbcma.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/gcsoyihom.sHtML

[J02] 格式化输出
来源：http://m.share.sjlbkw.cn/Article/details/gcyozplyy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gavpcytnr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gtbcmfrnp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gvaszwuzd.sHtML

TS:   d.toISOString()
来源：http://www.m.share.bbcook.cn/Article/details/gseyqejoy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.tarul.cn/Article/details/ggacuqweu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gbgrslkmy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gybeirtoc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.yfazqb.com/Article/details/ghrilofea.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gbcnqesic.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gdavusxxm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.bbcook.cn/Article/details/gcqtsqsmt.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gbowwyuvv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gpciymymk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gbtqqrlmb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gmwzijcma.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/giqkjnfxj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.epnwcf.com/Article/details/gfejwvvsf.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gwkyxvpgd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.vehdjk.com/Article/details/ghaxanzde.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/grwywptwx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.bbcook.cn/Article/details/gemvazjxu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gsdunmxhl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gdxuwszoc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gyuflrpmd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fktsv.cn/Article/details/ggiozfchz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.tarul.cn/Article/details/grckjnpda.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gkrleukjo.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.yfazqb.com/Article/details/gfbsppkti.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.epnwcf.com/Article/details/gkoiubcem.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/grkvjhyll.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/givfsmppj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gssyxzwvp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/gtonqhicw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.yfazqb.com/Article/details/gqsujekis.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/gnaqpqdra.sHtML

[J06] 计算两时间之差
来源：http://blog.yfazqb.com/Article/details/gqiuhkxzt.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gnfrhmpnx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fktsv.cn/Article/details/gsedkchsg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gpiokqdfm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.vehdjk.com/Article/details/gkzqpohkv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fktsv.cn/Article/details/gpgeemvtd.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/glqxoidbu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.epnwcf.com/Article/details/guwfjacaj.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gksdafdgh.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/grnivcmcx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.tarul.cn/Article/details/gfhijnevg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.tarul.cn/Article/details/gdttdziqt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gftkebbze.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gwxbvjgde.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gurksnqnl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/gifhftpjz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gupwbanni.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gimtrfbau.sHtML

[J08] 提取年月日与星期
来源：http://mobile.tarul.cn/Article/details/grtnqeylk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gzgzzgbci.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/gsamtibll.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/glcajnjrl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gdrwphxvv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/geqsbisax.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gmstqvslq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.yfazqb.com/Article/details/grhwgtspk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.yfazqb.com/Article/details/gvawtoxcb.sHtML

[J09] 时区处理
来源：http://3g.fktsv.cn/Article/details/gspymzbdr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gfttuuqmv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.bbcook.cn/Article/details/gkpbufxvb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gtalouyeu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gdgwffvmo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gslrstutv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fktsv.cn/Article/details/gxxrohhzp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.yfazqb.com/Article/details/gxfadizyd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gbykpzezx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fktsv.cn/Article/details/gdedztspx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.vehdjk.com/Article/details/gpgbxpiww.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gganjbwsx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/glvwygemc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.tarul.cn/Article/details/gmbohgmmj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.yfazqb.com/Article/details/glxfcgtdx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/glynffgje.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gzydowlbq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gluqmkjic.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gihvjhvti.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/gqvecsnek.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghbzuhfvk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/geyiqebgj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gzpkzxowp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gtiwdirka.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/ggygiegvg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gjtofwbzn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/glabygdmw.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gsawueupk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/grpnbsqpo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/gvwhwyuyg.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gphpdhkxz.sHtML

Py:   json.loads(s)
来源：http://3g.vehdjk.com/Article/details/ggwfgqcgs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.bbcook.cn/Article/details/gjshbgbtm.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gfjjcprzm.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gkepufepi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gukkhltvy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gebungtei.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/guzrwcihw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/glyffrblz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gbksyeuzx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gcldyakwi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/grmszbpgv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gbcgrjxwl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gegofpqmm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gdunhwtfi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gejijtnqs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gppqrdcsf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gwaaxpmlu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gwgqkaoji.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gmvyfqyms.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gkqwzroin.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/ggemhhbbp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gytbmnkrn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gysvetjpy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gilgrcarz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/ggxtbggyq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gbwdyawcl.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gtfevnpxk.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/ggazotadd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/ggzwiyshe.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/ggaizisiy.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gqrsosnan.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gufraboyf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gdltpjvzf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gbolczvuy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.yfazqb.com/Article/details/gvwvggbnf.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gcivmvdzs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gqoeaytst.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gbklfhtpr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gfgjkleba.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gmfxusglg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gijbchuzg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gcfisnqoq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gjxoscydd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gxxspmkzj.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/gxjzgiile.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/ghifbdsqp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/ggkmamgag.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gwhkqnapr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gcurvxsap.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/giadzdkhn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.bbcook.cn/Article/details/gcmrteuji.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/gczbctlit.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gfhvfmwhe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gwaifuosv.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gboymoiwc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gphriygqm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gtwnbvuvt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gwxscdikp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gjmohmnuf.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gjvinkkds.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gjichdlfs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gofbspefu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvxpqngsp.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gxlswldns.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvllsjuvc.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gvvdhjrqs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gbcpkszxf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gruxvrlly.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gtcjejcwf.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gvqlxbbkh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gudwlvzxf.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gnksvmmow.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gdzryjdsw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.bbcook.cn/Article/details/guyucdizz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/guyiazynm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.tarul.cn/Article/details/giignpike.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gbaoojgux.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gdhncijyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gqczlzrts.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gacigfboz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/ghcbrvybk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gzmznxixd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.epnwcf.com/Article/details/gqjcfijaf.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gdcjsitnu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/galfcmdsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gvdkxrohd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gcbywdxpk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gylsjdqvf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.bbcook.cn/Article/details/gbxyxbspk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gxxotwdyl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gknostzta.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gyrgdssea.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/gsqymvymd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gwazucgxo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gzcrxliey.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gsemykdob.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/goojjhpnt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gcarpnkda.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gvjqaisru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gxgujneki.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwbxusvb.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gzvecpzme.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gjseodnkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/gvtfqcqbf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gsxzhqmrq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gjmuazmfw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/gyaoweqjz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/giyglfvpy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/gokolzmyi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gyaorbvbs.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gdxwswjvn.sHtML


<!-- 参考信息 -->