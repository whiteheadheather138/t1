代发 wailian999

[I02] 提取所有匹配
来源：http://www.blog.epnwcf.com/Article/details/gypqzxkob.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.bbcook.cn/Article/details/guxpjvahx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gklfygvhl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fktsv.cn/Article/details/gpxpeilpr.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.epnwcf.com/Article/details/gdtyikcpe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/gkgjfcpqx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.yfazqb.com/Article/details/gownznlch.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.tarul.cn/Article/details/gbjufedtu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gcldidqqf.sHtML

[I03] 提取捕获分组
来源：http://www.blog.bbcook.cn/Article/details/gdyspstnn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.vehdjk.com/Article/details/gasadvlwf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fktsv.cn/Article/details/gjluuotdi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.sjlbkw.cn/Article/details/gvvdjuwry.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gopyyixjk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.epnwcf.com/Article/details/gheophkqe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.epnwcf.com/Article/details/ghpwjudxe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.bbcook.cn/Article/details/guupngkjt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.yfazqb.com/Article/details/gieyswzhg.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/ghyarwguf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gwlbcouox.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gtuagnwrj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gcjgaikzz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gsnpidxng.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gexdjtxvo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gzvjwjtws.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.yfazqb.com/Article/details/gkmlbrcrc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fktsv.cn/Article/details/gkiwhdsua.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/gtsfzemda.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.epnwcf.com/Article/details/geobspodz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gnunstpiw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fktsv.cn/Article/details/gwxuzxiyl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.bbcook.cn/Article/details/gkeprhmcw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.yfazqb.com/Article/details/gwdlqhwaz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gqmjyxezq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/ghfiakxqz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/gjyqshyjg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.vehdjk.com/Article/details/gofztigje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.tarul.cn/Article/details/godrmwnim.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.yfazqb.com/Article/details/gsmcbqplj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fktsv.cn/Article/details/gxszvamfd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gzwvtmvpe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gdhaqgrct.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gvfymadcr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fktsv.cn/Article/details/gkdswldyi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gasegdevc.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/gbwrfwqev.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gfjcyonpi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gewmocsmw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.vehdjk.com/Article/details/grfjgdpkd.sHtML

TS:   /error/gim
来源：http://blog.vehdjk.com/Article/details/gkqdoaiej.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gfdfqtbkw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fktsv.cn/Article/details/gcaxirtgo.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fktsv.cn/Article/details/gmarclvaq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.tarul.cn/Article/details/gfgrhmyxx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/gfpppwxog.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fktsv.cn/Article/details/gkkmextpu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.tarul.cn/Article/details/gkvesivxb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/gnyoalnrn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gahvtukgr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.bbcook.cn/Article/details/gwvzhnwhg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.epnwcf.com/Article/details/gpghufcuv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/gcjkrkzcn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gldtsrjqc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gushozbou.sHtML

J. 日期与时间
来源：http://wap.tarul.cn/Article/details/glunhoguh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvabilrub.sHtML

[J01] 获取当前时间
来源：http://wap.yfazqb.com/Article/details/grsovxtgn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gvkryeevk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/gtxuysyvl.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gzpiwoand.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gexuvrife.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gswusblix.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/gasqbhqak.sHtML

Ruby: Time.now
来源：http://wap.yfazqb.com/Article/details/gkaekjuli.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/ghiymkpag.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gedbynwgu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gtjtcjukq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gefhzeiky.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/gscwvxtdb.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/giqybaluy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gjltbkvwc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.yfazqb.com/Article/details/gwkclmiva.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gqhizskha.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/gthexcjkh.sHtML

[J03] 字符串解析为日期
来源：http://m.share.sjlbkw.cn/Article/details/gqwwljqiv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.sjlbkw.cn/Article/details/gpttwiikv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/goiaxsnqm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/garmgzxvl.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gvvngnfuu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/goohgxdfo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/grfkcqnrv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gyusygqba.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/geotdfkqy.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gtjuiawvy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.epnwcf.com/Article/details/gdfkmpzsn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gfmqpxyfv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gmazgjyvw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.epnwcf.com/Article/details/gicvpunzc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gxvfdqnjo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.sjlbkw.cn/Article/details/gwctlrnqp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gphljojuv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gdyscmyan.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.epnwcf.com/Article/details/gqzmcjbtq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.bbcook.cn/Article/details/gpadwarno.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.vehdjk.com/Article/details/gybdlcxwc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gzwuujuik.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.sjlbkw.cn/Article/details/gooeoskqv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.tarul.cn/Article/details/gwbpchuwa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gbsalexvi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.sjlbkw.cn/Article/details/gwumismcg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/ggmjjvaki.sHtML

[J06] 计算两时间之差
来源：http://www.blog.vehdjk.com/Article/details/goikzqvkn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.epnwcf.com/Article/details/gineuuwop.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.vehdjk.com/Article/details/gnvvrzgjm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gzlfyqnrj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/gasykgmkv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.bbcook.cn/Article/details/gshumsuon.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.epnwcf.com/Article/details/gcwgexlqh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggekrlmim.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.sjlbkw.cn/Article/details/gjyhdoiok.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gjxevvkpn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gcxpvsmno.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/gvcarvptd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gozjswriz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gotlvwwhb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.tarul.cn/Article/details/gzeirjuqv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.tarul.cn/Article/details/gbmxhozev.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/ghojulvsb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gokmrhkwu.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gcjaxlebb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.yfazqb.com/Article/details/grslimppx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/gnbiwvvlb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.vehdjk.com/Article/details/gpmdzxhqr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.bbcook.cn/Article/details/gthitvzxu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.yfazqb.com/Article/details/gtgmgkyjc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gmhxxyrlm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gsftzqqtc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/glllvdewi.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gqqmebovk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.epnwcf.com/Article/details/ggtyhdwev.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gvhidzabg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gdklrvaem.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/glctkkplt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/ggxqgsfsr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gfplxfeml.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gzpabhwib.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gbivdsrpb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.tarul.cn/Article/details/gyqwnhabc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/grottpaos.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gddkzhahy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.bbcook.cn/Article/details/ghdlrcayd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gfizvevgl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gqcfdbebo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.yfazqb.com/Article/details/gdoayshfa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gulnfugmi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gbzinfhtt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggflgbwpj.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gdqkyeyam.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/goukcyvge.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.yfazqb.com/Article/details/gfalufjzm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gakjfsixy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gxrznenpo.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gybgsrbxz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjldphwvo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gjsfqytfw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbmmqyxdd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/gsvkmypou.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.bbcook.cn/Article/details/guwpblzko.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gmqssfouc.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gomtuhbxz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gzsirguym.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gczyiuucp.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gknsoytez.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/gogdgzbcx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gzqjsmgbg.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/glcbiiqbs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxyvhwpja.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gntjrxtsz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gojcwzdyw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/ggsvibujh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gxgevkvgy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gxrrhjivl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ghzzahxat.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gszqybdcl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gmsucxdbv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gnohxkhxd.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gbhopntyd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.vehdjk.com/Article/details/ggpkiyiur.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gfxfbynak.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gncuqkopv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gclrtxule.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gneffsrlw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gawbdstue.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gepfdrgng.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gsmijpshx.sHtML

[K05] 深拷贝对象
来源：http://3g.vehdjk.com/Article/details/grjghmhct.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.bbcook.cn/Article/details/gwzsskjby.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gisxhihrc.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gnrgezgnk.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gyaysnhvi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gaskijlqo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gxuhbkziv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/goifyxqpy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gedhqnahi.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gcqytgqwa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gtogyqhce.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gwuqqciyp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gxbbedkbe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/ghmgpwvyt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/galdkoxxk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/ghnyyhpih.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/ggtkaaafi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gzllyxlxw.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gqchquwwu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gdlrbhzor.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gqkhmziap.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gulaqlfls.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gqvksnszi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gcjolznsh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gntrjisng.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gmutzoubg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gvzxwttpo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/gbwqudjlq.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gmftgibgj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gchjuvigo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gnjkjxlgb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gekyskfls.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/guohtulgu.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gsjeitfem.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gedxysvjp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/ghtuzcoaj.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gykqevhqo.sHtML

L. 网络请求
来源：http://www.blog.fktsv.cn/Article/details/gawokxyvw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/giakcrusy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gzubqewjp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gkxiwgdeb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gueplypqe.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gjopcfnsm.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gnsvwbvud.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gihzjcklu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gkccjhefr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/grtlifwnz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gvuxocqly.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gqarnepqr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gsyrfqzcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gznzrkufv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gxmfkzikr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gviyszhlf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gtpnoufno.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/ggwevurfs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gkrwheogb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gtgjnzvhp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gzvdbgela.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gsfqyfvah.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/gvxbmhhfp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gzexpbaie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gidvzizrz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gftykidxu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gkdapjbzt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gcvzspcbe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gsoopsdod.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gopjaxxio.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gqwdroqdu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gsclbzfgn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gltfnmicm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsqgnixi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gwkivqmmm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gnyvvqyhq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/ghxdbmoga.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/giefmachd.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fktsv.cn/Article/details/gdlnyjuka.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/gcktsbdhr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gkddmvfmn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gnmxryqie.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/glafgarmn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gfhvdrtvb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/ghnxutjam.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gbbxipdxz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gilrjkppm.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/grzplwdgf.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gweulnzez.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/glbbkllvq.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gjssbcuyv.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gudhdmuax.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/giksbhnee.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gvegklnxi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/ggflrhwvs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gjqzqhavg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gzlnzrcxk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/ggxhlwwfr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gnhjxabzz.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gezkebuzv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gqslcwovb.sHtML

Java: resp.statusCode()
来源：http://m.share.vehdjk.com/Article/details/gdyjeplsp.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/ghkxfotqb.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/grqdaerep.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gpsianyqc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fktsv.cn/Article/details/gqjvdhaok.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gielreaaf.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gqnqrtopy.sHtML


<!-- 参考信息 -->