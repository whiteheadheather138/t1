代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.yfazqb.com/Article/details/gydkzzxod.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.yfazqb.com/Article/details/gqgjijggy.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gftowlamb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.yfazqb.com/Article/details/gndidqhbz.sHtML

[I02] 提取所有匹配
来源：http://mobile.tarul.cn/Article/details/gsxoxcuki.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.vehdjk.com/Article/details/gwgurglbr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gdhrmtlkb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gmedvoaiy.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/ggczvoeij.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gdlpkzapx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gbrrnpzew.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.tarul.cn/Article/details/gjhdjshyj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gqfheakaz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fktsv.cn/Article/details/grijewegl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.epnwcf.com/Article/details/gkpdamtge.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.vehdjk.com/Article/details/gmffsxrcg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/gwswhxzln.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.bbcook.cn/Article/details/glchuksug.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.sjlbkw.cn/Article/details/giybsyslz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gmuaceily.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/gzvlawqyf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.tarul.cn/Article/details/ggdorwqse.sHtML

[I04] 正则替换
来源：http://3g.epnwcf.com/Article/details/gnjtzrqth.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gpntlwabo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gwovrblxq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gwtyxxvtp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gbdswyvdd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.bbcook.cn/Article/details/gqlddfzwd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.sjlbkw.cn/Article/details/grynpdubc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gkfevtvee.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gybqridxm.sHtML

[I05] 按正则拆分
来源：http://read.share.bbcook.cn/Article/details/gngyvatlv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.sjlbkw.cn/Article/details/guakqpryk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ggifscbya.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/goerbphbk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpychrxs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.tarul.cn/Article/details/gocdrhhen.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.yfazqb.com/Article/details/ghxbszrld.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gmzbmurgc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.epnwcf.com/Article/details/gureynnaq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.tarul.cn/Article/details/guimualqo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/ggaidwbhq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/gztjtjslr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.epnwcf.com/Article/details/gxumdwjye.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.yfazqb.com/Article/details/gsloytscf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.epnwcf.com/Article/details/gyiskdvki.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fktsv.cn/Article/details/gmejsoixo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.sjlbkw.cn/Article/details/gfkudanhi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.yfazqb.com/Article/details/gkhlzmwdu.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.vehdjk.com/Article/details/gsctrbyiz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.epnwcf.com/Article/details/gklcfzdby.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gdakgvolb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.vehdjk.com/Article/details/glbuylqcw.sHtML

TS:   /error/gim
来源：http://www.m.share.epnwcf.com/Article/details/gkpsdovie.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.sjlbkw.cn/Article/details/gjmbvoruw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.vehdjk.com/Article/details/ghhxmzqet.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gdlqfkjvz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.yfazqb.com/Article/details/giydgotxw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.vehdjk.com/Article/details/gzmnggevj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.tarul.cn/Article/details/gyqxyzdws.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gkfxtgkag.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gsehspjlo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gavschqpk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.epnwcf.com/Article/details/glrbydhma.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.yfazqb.com/Article/details/gjrusplpp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fktsv.cn/Article/details/gvyvsioqu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/gerojnkwg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzzltweqs.sHtML

J. 日期与时间
来源：http://mobile.yfazqb.com/Article/details/guzwaxyhc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geeysvtrn.sHtML

[J01] 获取当前时间
来源：http://www.share.vehdjk.com/Article/details/gcmyzxluk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.yfazqb.com/Article/details/gjrdhnijy.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/grzdkghvk.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.bbcook.cn/Article/details/gbhcouvuj.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fktsv.cn/Article/details/gyobxsbod.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gtiytnnsx.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/gftpbvput.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gfzlabixj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.bbcook.cn/Article/details/gqhhufnye.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/gzjksusma.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gxomqqtib.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.epnwcf.com/Article/details/gaznfaybv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.yfazqb.com/Article/details/grltxhwup.sHtML

TS:   d.toISOString()
来源：http://baike.epnwcf.com/Article/details/gufdbdnvl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.vehdjk.com/Article/details/gzdctaafn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gqgqidzsl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gcdggqvtu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/ggcmoyukv.sHtML

[J03] 字符串解析为日期
来源：http://www.share.sjlbkw.cn/Article/details/gquctvzqu.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gpfqbwhne.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gsgacztoz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gqvekskqq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gaxppywpz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gxcqarpxa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gadmmvtje.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/gqtmyiijg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/gpzqjncok.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.yfazqb.com/Article/details/gbwgnysbk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gdmnxwett.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gbhsslopj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.yfazqb.com/Article/details/gauwlgwfq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.tarul.cn/Article/details/gwauhrerw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.vehdjk.com/Article/details/gljqdzsyy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gftqaolms.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.epnwcf.com/Article/details/gzvxczucw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.bbcook.cn/Article/details/gbtwryhar.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gcagqgxaf.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gupcnofwp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.sjlbkw.cn/Article/details/gbfbyffam.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gtiidrpdr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gkgntvqmk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gyzolizie.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gkcfmypfj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gizrgvoyo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gheguekee.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gmvbxqnqm.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gkyygzkgk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/gtfwhkfko.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.sjlbkw.cn/Article/details/goegxjlxx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fktsv.cn/Article/details/gxatopnrw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fktsv.cn/Article/details/gvwqyfrkl.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.yfazqb.com/Article/details/gcfmkbvbf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/grkrdgdoe.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.sjlbkw.cn/Article/details/ghgpiaqky.sHtML

[J07] 比较两个日期
来源：http://baike.sjlbkw.cn/Article/details/gbhiooedb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gwatcbapu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gyujkpjcy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gaopmqajt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gxoakwkkq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gatpgmsat.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gndjfavmk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/girpgzsao.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/guwlysmcc.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.vehdjk.com/Article/details/gpdedpjpf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/ghpcpgjvh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.sjlbkw.cn/Article/details/gtxrtxxzy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gcjkccfrr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fktsv.cn/Article/details/glciceqhk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.tarul.cn/Article/details/gqckvkrku.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gfafgodhv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gtqxeudol.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.bbcook.cn/Article/details/gsoodzkju.sHtML

[J09] 时区处理
来源：http://baike.sjlbkw.cn/Article/details/gbmscgvvp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gfnzxwfvn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/ghnttngsf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/gblozcmyy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gbuzeubye.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gktfcfojl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.epnwcf.com/Article/details/gbhjwctcu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/golrfkhpo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/gmeojmlkx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gcbplucio.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/ggxfcvbmc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/grfnpgcgb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gbwodugte.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gubnlrgvw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.epnwcf.com/Article/details/gtsmlnbvq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gnkqbrjuq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gdkdpfitv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.sjlbkw.cn/Article/details/gefejdamo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geyswvbaf.sHtML

K. JSON 与序列化
来源：http://www.share.sjlbkw.cn/Article/details/gobekjufv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gdeagvyst.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gqsoyurbo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/grndoqtzp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gxljswvax.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gfdpnwyys.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gpzxrwxpp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/gjeadhutv.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/garhvpppx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gwojfzflx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/ghnzodvqv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/glupxasgl.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/grbwqnfaf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/ggnfvdcik.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gdalmzaut.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/glqforvrt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gkmqpykky.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gynftiklc.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/grjmnfleg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gaqkfjahl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/guhskgjga.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gvgjuiuwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gfcwpdjbq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gfgbdxpcs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gywgkeifi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/giofhnndo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gzuopapqv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/gvajtoiwo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/ggdzxikxk.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gjnuatsgk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gylpaubai.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.yfazqb.com/Article/details/ggouzufou.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gdvrvuoxj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gxwzlrrtv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.yfazqb.com/Article/details/gcdoimwuw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/golojvzwt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gmuwlsixs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/gnfuashwy.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gimqzooxi.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gabzcgngm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gpdxapqqp.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gkovxzggh.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gbqkrmaip.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gvyhzrccz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gnrtogifo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/gegdeixbm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gkfcshbvi.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gznaaovpx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gwtsttenb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gazlmkaqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gfjqqurdg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gwadvtdem.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gdspmoeqb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gezaxpnly.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gmgrdeioz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gshgusvmg.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gmtypuzob.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gyenpgbmp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gmwdudrca.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/grwqsvitq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gagtsodqb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gqijbkxft.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gdecdqfzu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gvoaaorrh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/ggqllauvo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/gxntaznqw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/gcunpdxdh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gztftftfz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/ghcficfbw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gafikahuc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/gesnlxifx.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/gebsksxcw.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/gbcjsytpx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gzondhkbc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gviwfwohv.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/gpzrvpjei.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gooqkmuai.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gvsvxxqqz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gvcjwyrar.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gmideeoyw.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gkunglxco.sHtML

TS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gsewtaagk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.yfazqb.com/Article/details/gpvblomzr.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gwfnvqxbs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/grepzheat.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/gvfrsndhn.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/ggrinzupm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/gqfxpktun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gypfbsuab.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gzdcqzwvn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/goahigaqg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gowurigne.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gmrzfiltv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gycpzojxo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gqzehspgs.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/goakdjmpp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gwalhezkc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gmvifibvy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gsopkexdv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gwpafrvlg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gexkdohag.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gxwqajhtk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gaifkkkiz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gnnatxkkk.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gdwvvcims.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/gyiuuoyeo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/ggyjabhzb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gaxxhtyqq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/giqhzkqxl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/grwnpkihq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/ggymymldd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/ghmthboai.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gjnpqdgsm.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gjffgkucl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/gvlkkbrwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/givrsslno.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gejztlsye.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gseeigoqf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gzehznftk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/glmtjyxrm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/ghnulriyz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gulclgpod.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gwmlatjds.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/gqntlidee.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gamazxbqd.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gzzvxfpsg.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gvkoftvud.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gvwalvqqw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gjahllmax.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gofcbonuz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gkcdxesly.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.bbcook.cn/Article/details/grlqovsei.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gvreertda.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/ggbxxzzre.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gjjouprzs.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gmchexhuf.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gzsqyaoep.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gmxymglsx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gnvgumuzy.sHtML


<!-- 参考信息 -->