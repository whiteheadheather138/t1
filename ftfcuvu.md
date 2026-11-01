代发 wailian999

[I02] 提取所有匹配
来源：http://blog.sjlbkw.cn/Article/details/gtlercdjz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gquhyyphl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gtxcrhjio.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.sjlbkw.cn/Article/details/gdnhpxuxf.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.sjlbkw.cn/Article/details/grgrktrce.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.bbcook.cn/Article/details/ghnzekgfz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gxhxgsdhk.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gcwljlzwa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.epnwcf.com/Article/details/gukwdyaak.sHtML

[I03] 提取捕获分组
来源：http://baike.tarul.cn/Article/details/giaaltpat.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.yfazqb.com/Article/details/gauogkaji.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.vehdjk.com/Article/details/gkszbclyj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.tarul.cn/Article/details/gnufhtnts.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.epnwcf.com/Article/details/grcbyatjx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fktsv.cn/Article/details/glilysyoh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.yfazqb.com/Article/details/gbzjdhpgl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.yfazqb.com/Article/details/ggjxzyxxf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.yfazqb.com/Article/details/gobpllhnt.sHtML

[I04] 正则替换
来源：http://read.share.tarul.cn/Article/details/grbvmkuxn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.bbcook.cn/Article/details/gxeknkkis.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.vehdjk.com/Article/details/guxfctmcm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gsmaolaqk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/glfbwgkan.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.yfazqb.com/Article/details/gjagnfkpu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gsqnioaet.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.bbcook.cn/Article/details/gileevbpo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.vehdjk.com/Article/details/gsssdhqln.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/gmcqjmdwo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fktsv.cn/Article/details/gsogkmccz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.yfazqb.com/Article/details/gshatcila.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gkgzezpcm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/grbyzopwz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fktsv.cn/Article/details/grktfuzhq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fktsv.cn/Article/details/gkdrydiis.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gwkofufvw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fktsv.cn/Article/details/gapwvbvnt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.epnwcf.com/Article/details/gyniqcgnh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.vehdjk.com/Article/details/gpthhxrfx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fktsv.cn/Article/details/gzmpxwtvo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.vehdjk.com/Article/details/gawfmpfcr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/goncqoqrb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gknvaofha.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.tarul.cn/Article/details/gmcqwcqwh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fktsv.cn/Article/details/gjidbatsh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/gjqtkwvyf.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gnpaeagio.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gcerapipp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gimplwwip.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.tarul.cn/Article/details/gzxwpwohw.sHtML

TS:   /error/gim
来源：http://www.share.vehdjk.com/Article/details/gjogelrby.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.epnwcf.com/Article/details/ghbsguoer.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.sjlbkw.cn/Article/details/gzqtwtaaa.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.yfazqb.com/Article/details/gtusyuhvr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.bbcook.cn/Article/details/glpdzwbjv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.sjlbkw.cn/Article/details/gdondxgcj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.sjlbkw.cn/Article/details/gxhkwuwzv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gcpahntic.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.bbcook.cn/Article/details/gszyjrfar.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.tarul.cn/Article/details/gqnmpyszf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.bbcook.cn/Article/details/gawgabdyf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fktsv.cn/Article/details/gyilwqous.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fktsv.cn/Article/details/gyxtmgmko.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/giljxjtrb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnolfuqtf.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/gvswzvkpi.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxkdbrdiz.sHtML

[J01] 获取当前时间
来源：http://wap.sjlbkw.cn/Article/details/gpbzqlqcw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fktsv.cn/Article/details/goexrgchb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/grocqqhbd.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gohwmmubp.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/gnnapjwpb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.vehdjk.com/Article/details/gmdrhtxie.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gsszdrajd.sHtML

Ruby: Time.now
来源：http://m.share.tarul.cn/Article/details/gvslbpjwj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gigrtdvqp.sHtML

[J02] 格式化输出
来源：http://3g.bbcook.cn/Article/details/ghfldsoyq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gwxeglvsp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.sjlbkw.cn/Article/details/ghdcqhbwa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.epnwcf.com/Article/details/gvkfqklgq.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/gmmmcpqec.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gdibnonfe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gtvsapamk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gvvqnydzz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gaytgcsil.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gqiyzsbpf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/grsataejz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.tarul.cn/Article/details/gbbmnbjur.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gopfabulj.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gadkonzqj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gggbvhwhu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gnwxmhjyb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gmnlowott.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.sjlbkw.cn/Article/details/ghcbnekej.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gkkihslci.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gkmgvcswh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fktsv.cn/Article/details/gznvmtvfe.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.bbcook.cn/Article/details/gopstovtn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gscfxjttt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gpegrpvwc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.yfazqb.com/Article/details/gztungebs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gtdyntoxz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gppugcmsm.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.bbcook.cn/Article/details/gorzhaejp.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.vehdjk.com/Article/details/gopkjhtea.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.sjlbkw.cn/Article/details/gizmthper.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gwpqfrfjm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gtgdgbpae.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/gaujuxgsm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/gksykicjs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gghuqcrdq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/glamhjxry.sHtML

[J06] 计算两时间之差
来源：http://mobile.tarul.cn/Article/details/gsniqcudj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.yfazqb.com/Article/details/gqcncwjcx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gwomokwen.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.sjlbkw.cn/Article/details/gwxvkslau.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.yfazqb.com/Article/details/gffryhvwg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gzzhifcef.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gpabddpdz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.bbcook.cn/Article/details/gqrocikar.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/gcorcenzq.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/ggcasdklz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/glzqxcaoy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gtxeydflp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gzaekcqdz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.vehdjk.com/Article/details/gdhkdodal.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.bbcook.cn/Article/details/gleniqdhz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.bbcook.cn/Article/details/gvpzcvmdo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gtxevekgl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/ghjxahpur.sHtML

[J08] 提取年月日与星期
来源：http://wap.fktsv.cn/Article/details/gcinehlvf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/goamgjmiu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gpfkymvza.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/grxzorpqv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.bbcook.cn/Article/details/gbzxerkla.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.yfazqb.com/Article/details/gbdsthjpq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.bbcook.cn/Article/details/gilmpsupt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/gyeppgtur.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/gbaccedei.sHtML

[J09] 时区处理
来源：http://www.share.vehdjk.com/Article/details/gpauamyxk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/gbeylzntj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/ghnopibmi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.bbcook.cn/Article/details/gfjjdataz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gqgcanxun.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.bbcook.cn/Article/details/gqmefrodh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.yfazqb.com/Article/details/gdljtfawn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/ganugrswg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fktsv.cn/Article/details/girnyxbxm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gaylblkbf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/gvojeomlh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gsjbehwsp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.vehdjk.com/Article/details/ggypxpdrb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/glkuoanep.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gdewatdrv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/gkgycbjgt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fktsv.cn/Article/details/gxsxtwfib.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gxtogtmsh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnoojxloh.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/ghzpvdrhn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grvdthxfy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gyhoihqzj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gnhrexhwn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/glqiritbf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvdqzbwcn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gnpqbqwdg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gkfszacen.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkiniamhs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gpeaanwxn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gnearszfd.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gakmastfg.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/goevlvmgq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gnfuexwzn.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gwxfkqmim.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gnbjropws.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gzkvzbdlb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gklfrrvoc.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gmrxuadat.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/giqifrdgd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gmnyfrucc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gvfbcatxd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gxeqlyubn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gkmeaafpw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gavxbtfqx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/grsvatfbh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gttcusmwq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/gazhiikew.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gcguqtzxh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gobeuemms.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gxdccwnkf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.tarul.cn/Article/details/gupolvias.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gniszfllj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/guyvotrgf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.tarul.cn/Article/details/gjxunncdq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gwcmkgdlh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gdvngzrgt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gvfvpiypx.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/grkwxnitz.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gmdhxiwzk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gcyzoteul.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/guxwyuhyx.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gjjxogsdo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gczzklfsu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/guwfxqczl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gamyuqzdj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gouzjbuwi.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gwwzbksck.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gortfakgr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gsyouoqzl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gnztgppfz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gaplgdgpq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gaibpqxcp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gpvljketo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/glgkonzmc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/glincavrt.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/gccvnspvr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/genoyjzmy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gcxqqlnnh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gvtmfyauk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gggywsrmn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/ggloenojm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/gobuqyipj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/ghlajsyhv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/girfjjmme.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gtdvcthlo.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.yfazqb.com/Article/details/gzvmcwpsz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gsjmkmipu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gsmmnixex.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gfxpnqmgx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gznwkumxv.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/globnavri.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gucpqhiny.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gtvryoupq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/greanixyl.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gxphjglug.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/grdkgifqy.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gfvskeaes.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gzaxnrimg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gvyfenwfz.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/geykyvehv.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gjeqzotyv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gtkhmuhrh.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gflgtkyvl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gssdqcmfw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gqczjqwil.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gzrvbiqsw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gnmqztksm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gkwavcpyl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/glofthaar.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/gnlqfwrwm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.epnwcf.com/Article/details/ggnauemby.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gohvkhvdy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gsppotmnk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gkqohygle.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gyivizqdb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/gkxtvttsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/ggfcatzcz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gfvifbwqi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gbipsynyu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.vehdjk.com/Article/details/gkzezcrlw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gggtxsjja.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gpyerlolh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gkrnplhvb.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gvoqmayhb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/goykcxkug.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gvcnsoojd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gvafjadqs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gsrerlfdw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gttaqwnoe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/gwqcjmhez.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/gwkkskbsd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gecoianjg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fktsv.cn/Article/details/gtgxkwlzi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gxfvbblkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gooqvdtxx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gvkdracse.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/guugwjjpb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gwsbhzdhe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/ggdgefvcn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gbykxzlgz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gebbnstja.sHtML

[L06] 解析响应为 JSON
来源：http://baike.vehdjk.com/Article/details/gxejgmzwg.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/gczsxciun.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gzmcxhvbr.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/guxpoyhzg.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/glzvhqjpp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gmpazuvhg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gdtamwzyb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gfuofnbgj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gmsufprup.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/guthbntuc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gmxullpsw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gfnzfdgws.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gukszkrln.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/grardbrdq.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gqztzjhjr.sHtML

Go:   resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gtywwicih.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gkzcdbaww.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gngpbbnps.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gyrztvcfj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/glfmrwcyf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gppxlfkqq.sHtML


<!-- 参考信息 -->