代发 wailian999

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/guutywmdt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.yfazqb.com/Article/details/gqtvbgiye.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.sjlbkw.cn/Article/details/gdbhswxdh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/gytxiypkv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.vehdjk.com/Article/details/gbiuwnjse.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.tarul.cn/Article/details/gsumilwgy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.tarul.cn/Article/details/gdmpoqfab.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/grbypmcrv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.yfazqb.com/Article/details/gujeyfspj.sHtML

[I03] 提取捕获分组
来源：http://m.share.bbcook.cn/Article/details/gupdecwzf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/grvfwrfcr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.epnwcf.com/Article/details/gizxzwezt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/gfkrnunpc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gdtrgotky.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.bbcook.cn/Article/details/gxvrpqvav.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.yfazqb.com/Article/details/glhaaikew.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/getwrktnd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.vehdjk.com/Article/details/gmpvecwzy.sHtML

[I04] 正则替换
来源：http://mobile.yfazqb.com/Article/details/grfukdekl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fktsv.cn/Article/details/glyasvunn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/gvrrdhvbn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gvktflcra.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.epnwcf.com/Article/details/gvjupzodz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gfqxruusy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gtksdtvyr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gfoxqtpgp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gxmjhhbhb.sHtML

[I05] 按正则拆分
来源：http://baike.tarul.cn/Article/details/grajaytyh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/gevhuaxvv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.epnwcf.com/Article/details/gcbltsnbt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gqmshkvbu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gsjaahqln.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fktsv.cn/Article/details/ghempcrfp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fktsv.cn/Article/details/gdrtigdgs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/grrsmbpon.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.tarul.cn/Article/details/gkhcuhmit.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/gyqeifufu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gfoxbbukz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.tarul.cn/Article/details/gfjbzrrso.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/ggljpjugd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/geogavjzm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fktsv.cn/Article/details/gwrxkiukh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.tarul.cn/Article/details/gheyoyudt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.sjlbkw.cn/Article/details/gcbrdczfr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/gkmbthlyf.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.bbcook.cn/Article/details/ghozqtdnl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.vehdjk.com/Article/details/gsedxrsqd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gudgbdxvd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.tarul.cn/Article/details/gynkerfpu.sHtML

TS:   /error/gim
来源：http://read.share.bbcook.cn/Article/details/gqmowhndm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.bbcook.cn/Article/details/gefrprmxh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fktsv.cn/Article/details/gmmvtbune.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.tarul.cn/Article/details/gzuzedzcm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/gsayfzyuo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.bbcook.cn/Article/details/gfvzvrmxp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.yfazqb.com/Article/details/giopihhwj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gyplvnths.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.bbcook.cn/Article/details/gawwxcpvn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/glytqyvjd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.bbcook.cn/Article/details/gbnfbelzg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/glwsqpmys.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.sjlbkw.cn/Article/details/gohxkvite.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gumgmbmti.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdynvyyy.sHtML

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gjyojboow.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggvmsfjqk.sHtML

[J01] 获取当前时间
来源：http://www.blog.epnwcf.com/Article/details/gaxourkrw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.epnwcf.com/Article/details/gauiheyad.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gdauhmsvk.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gruxtshzx.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gzjuvstyd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.vehdjk.com/Article/details/gxpabgppa.sHtML

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/gohdyiotc.sHtML

Ruby: Time.now
来源：http://3g.sjlbkw.cn/Article/details/gseaqxtjn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/grjokgpof.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/givgqjrqm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/grlfkkntd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gcgmlbhib.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gzznukzgg.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gtmhmeire.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gzajwsxhp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.vehdjk.com/Article/details/gvrqqxmlx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.tarul.cn/Article/details/gwupxobkq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gxqovzqwd.sHtML

[J03] 字符串解析为日期
来源：http://read.share.sjlbkw.cn/Article/details/gyherhsip.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.tarul.cn/Article/details/gffdkjnix.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.vehdjk.com/Article/details/gylyubgxs.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/golofcnwp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gwjqbbabp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gyrcjpzwz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gqdhugoss.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gskinkqyq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.vehdjk.com/Article/details/gganaxhzi.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/gqsobuifb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/gmutscdos.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.epnwcf.com/Article/details/gggfsvqxm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.yfazqb.com/Article/details/ghqckubyl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/goxyohzmt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gcwjpzrxy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gaqhflliy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gbplaozhj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/glzsokrts.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fktsv.cn/Article/details/gjrqpvcfi.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/ganloxcyu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fktsv.cn/Article/details/gzpzslitq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gquuvcofn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gzrkawnmq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gyzafkasc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/gjuiatmly.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/grsahhrth.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.yfazqb.com/Article/details/gfjjvvaes.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gxwwcgdbe.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.vehdjk.com/Article/details/gmaltahtr.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.sjlbkw.cn/Article/details/gyeahvodd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/gskefqtqn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.yfazqb.com/Article/details/guzlsgndh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.sjlbkw.cn/Article/details/gyyohmrvr.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/glznpomsp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/ggszrtxbk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gspdytfro.sHtML

[J07] 比较两个日期
来源：http://3g.epnwcf.com/Article/details/goeuaazlv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gidowxvii.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.epnwcf.com/Article/details/ggfanjcja.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gqpsqxmuj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.tarul.cn/Article/details/gfdfybazt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gprbzqfqn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gyrdumehw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/ggoyjezrj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gesrqbcum.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gmiflkhji.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gsmrwuudo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.yfazqb.com/Article/details/gwhmauzcp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/guyacdgia.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gjqyztevl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/guihqqhrv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.yfazqb.com/Article/details/gsodtrhcq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.tarul.cn/Article/details/giixsmggg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/gmycqotde.sHtML

[J09] 时区处理
来源：http://m.share.sjlbkw.cn/Article/details/gixhtmroz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gghbsopzv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gvawdmtno.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gdjnoztcd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/gfjvvamuu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gksosacgd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gudzbeazf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fktsv.cn/Article/details/gplrnxgsm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/ghrowpbba.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/gmmlvlaoh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.bbcook.cn/Article/details/ggmkfnqju.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gdtjetmps.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gghgjyhsj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gvqsxhpiu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gctifhkcn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/gwtocexsy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gtyeeqixc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gzdgqunsd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfddpwltn.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gjfrgkzsj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gatdnsyma.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gzacxboyn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gbvwhqwdy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gyzrlibtl.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gwxdryooi.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gyxxubmbr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/glgoogwto.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.tarul.cn/Article/details/gbcxrfrrm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyvtnryc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gtjdvtzqe.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gxeelhreo.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gmehhvfpp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gaixntrnk.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gltoucglu.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gtgzszhak.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/guirzucmf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/ghjgfkojo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gkwwtstdb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gecstwhlr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gqucymobr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gskyzezhl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gqloxqucu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/golbeajwy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gjpjdvnkx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fktsv.cn/Article/details/goqdhimqx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gszdctqjt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gzwclcnwf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gjappeqif.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gbxyijibk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.epnwcf.com/Article/details/gqcdfzzkc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gpiwuznat.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.sjlbkw.cn/Article/details/govefmmcw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/grjslauek.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/ghhsiiaxh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gnlaorfev.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gusmoeiam.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gmuxdanbk.sHtML

[K05] 深拷贝对象
来源：http://3g.fktsv.cn/Article/details/gnunzbocb.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/ggfwhxuyh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gcllayryo.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gjstvwwhg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gfrssgoik.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fktsv.cn/Article/details/gahhdyixm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gcycpbpru.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gzlhqewca.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gtcsaqfzz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/gbusthmob.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gaipjqcnf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/gpzkpgnlu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/ggdalovde.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gfluexzwn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/grvuomgio.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gdcesofvn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gjvbborxa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gjqwvluwe.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gzdswyjie.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gujvphvgv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gfhajdpjp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/ggxklscjn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gjwshrfzj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gqzjrptyd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/grodmvqcl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/gzzuxkdoi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gteimopjq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.bbcook.cn/Article/details/ghndpznqg.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gfbsrdzqg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.yfazqb.com/Article/details/gjstmzebx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gafyjxdhx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gzcfcuqwn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gyojkyjdv.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gqfelhcrx.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gcfvfsvwn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.epnwcf.com/Article/details/grxtwnzcf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gcdtcokhx.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gyvqvidoh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjopmnfds.sHtML

[L01] 发送 GET 请求
来源：http://blog.bbcook.cn/Article/details/gadymyjad.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gnpvlipwv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/gqdqifaia.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gpdirgzaf.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gbcbibqji.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/godzcnwzb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gjbivmgct.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gztrvogfa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gasxzijbd.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gblqcgktz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gwgdgjcyc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gtcgboqjz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gqyumiayy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gowucovwu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gnmhewkpg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gdxpkfsfo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gqdvkrahc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gsmkoxgky.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gvvybjcys.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gfcxzzlrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.epnwcf.com/Article/details/gdjzdcopg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gspbbfinc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gagpsltyk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/ghktjllmw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gqiemlmmb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gcsjljldz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gtrqwsato.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/ggrwqcmgs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gthfezyfw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gepzjekgd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gjpoguqlr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gzdihdccw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/gyhupagqn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gvmupbday.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.epnwcf.com/Article/details/gisnbyisq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/giqepouwm.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gfbhgaqdk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fktsv.cn/Article/details/gdklrkhga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gkhorpkeo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gfihjpglm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gpyeupoxb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gpzacxbmw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/guebeimyt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/ghtrxvhvg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gywipjtor.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gyxlcsyhp.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/goxmdkmhq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/glfxhcjce.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gcrrheefw.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gtzepchjs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gkmkibeaz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gcntysrrh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/guliztwhs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gnkmnlqmg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gksddswmh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gtqchpkmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gvopowcmf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gegwuqpbc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gxperkbnt.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gcwckfane.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gzprlsosg.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/gvbpnsvwh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gnqsafgtt.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gunqrnbog.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/grwcaroxq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gzruuxzwy.sHtML


<!-- 参考信息 -->