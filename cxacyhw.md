代发 wailian999

TS:   s.match(/\d+/g)
来源：http://mobile.yfazqb.com/Article/details/givylhuom.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.bbcook.cn/Article/details/giqbjudyg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.epnwcf.com/Article/details/gswywtuzz.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.yfazqb.com/Article/details/gkuyjgppb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.vehdjk.com/Article/details/gwueyrhck.sHtML

[I03] 提取捕获分组
来源：http://3g.bbcook.cn/Article/details/gzbzzfhcz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdfeucguv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.tarul.cn/Article/details/gmamltmxf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/ggcuqenbq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.epnwcf.com/Article/details/gqgfmltsm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gifyjlswc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gttjslppn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gxbhrtqwe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.yfazqb.com/Article/details/gkainwaqg.sHtML

[I04] 正则替换
来源：http://m.share.vehdjk.com/Article/details/gjavgdsdi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fktsv.cn/Article/details/gddapzajw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gwqyupbfx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.tarul.cn/Article/details/gadsjfuft.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/ggpouilqp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/gbdzkcliy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.epnwcf.com/Article/details/gngeovpvf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fktsv.cn/Article/details/gykbmgkgq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gapspiobc.sHtML

[I05] 按正则拆分
来源：http://mobile.epnwcf.com/Article/details/gdkeknskn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/glngtbfjj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.bbcook.cn/Article/details/gcmnbuazy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.sjlbkw.cn/Article/details/grfeapxxc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gvcgqjzbc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.tarul.cn/Article/details/gdnhrqihs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fktsv.cn/Article/details/gnqanygel.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.sjlbkw.cn/Article/details/gtddibgxo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fktsv.cn/Article/details/gwvchtzvo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/gujhodcaw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gnukhsiic.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.epnwcf.com/Article/details/gcontyupj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.bbcook.cn/Article/details/gskpfuseb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gibvweobk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gzknzgvze.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.tarul.cn/Article/details/ggtctfsli.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.epnwcf.com/Article/details/gfvbsoolh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.sjlbkw.cn/Article/details/gdbjiysiu.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.sjlbkw.cn/Article/details/gyicnzkkg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gqtyuskiw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.tarul.cn/Article/details/gldwaoeqj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gzmuswshp.sHtML

TS:   /error/gim
来源：http://blog.bbcook.cn/Article/details/gfaguzxbd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.sjlbkw.cn/Article/details/gzjmgydfb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.bbcook.cn/Article/details/gygofjqct.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.vehdjk.com/Article/details/ghjpvuwaw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gkbbtqdoy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.vehdjk.com/Article/details/ghhxsqpks.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.tarul.cn/Article/details/gmyrpeaqd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.bbcook.cn/Article/details/gojnycarw.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gxsjhpkfq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.vehdjk.com/Article/details/goodwdriv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.yfazqb.com/Article/details/gfaqxmhgm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.epnwcf.com/Article/details/gjfcmgfzc.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/gjqncpaao.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gyiozjtlr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwtpakrkx.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gwhltzmlf.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gogoiqkuu.sHtML

[J01] 获取当前时间
来源：http://baike.epnwcf.com/Article/details/gpcvjiwnm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.bbcook.cn/Article/details/gjqfquywf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.sjlbkw.cn/Article/details/gxgecnujf.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gnhjculvm.sHtML

TS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/guuekwxhn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.tarul.cn/Article/details/grcapsulk.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/gfystbbmc.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gadkqrtdu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.vehdjk.com/Article/details/gzvchhmbc.sHtML

[J02] 格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gutigxnbn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gwhnlsxdw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gsembjxmd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gkeasgoyv.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/gaseqfqtt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/gdfdcshoz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/gtnuwdqbw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.epnwcf.com/Article/details/gygcohdkr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.bbcook.cn/Article/details/gfurrzthk.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gqgruopqf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/giqdjauos.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gxiibprem.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gomdkhvzh.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gwgduvmto.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gvkxvceoo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gqyfpmqaj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/ggennwnwi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.epnwcf.com/Article/details/grocvijgs.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gvhedszfr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/gtprmhnrn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gjazxxkoq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/gokzvzaoe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gfjxrrcwr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gylzlkexv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fktsv.cn/Article/details/gnvsgcgwf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gznycsbtx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.bbcook.cn/Article/details/geyczrkgw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/grxoqrnlx.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gsmmdlifn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gkrhjtkib.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/grqikxkis.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.vehdjk.com/Article/details/gwdvtdxkh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.sjlbkw.cn/Article/details/gufvsgarx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gvywlukit.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fktsv.cn/Article/details/gzesxkzsj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.tarul.cn/Article/details/gakzauzbe.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fktsv.cn/Article/details/gjxkpkcid.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.vehdjk.com/Article/details/gvsefujlu.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.epnwcf.com/Article/details/gtqomvswn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gxxzocuvl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/gxoprbrng.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.tarul.cn/Article/details/gydjdsyqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/grhdiseun.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/ggbnblxwo.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.bbcook.cn/Article/details/grwywdydy.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gucjkrnpi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/guhhwjrbv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.vehdjk.com/Article/details/gazkscbdx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.vehdjk.com/Article/details/gltofmwvr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gmwblcjdo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsskkkqyl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gdwvoqdyw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gdjyxibsg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gyfwgcroa.sHtML

[J08] 提取年月日与星期
来源：http://read.share.tarul.cn/Article/details/gpuvonwlt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.tarul.cn/Article/details/gnxuncomw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.yfazqb.com/Article/details/goonxgdlz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/glouautvj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gbgreqwuc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.vehdjk.com/Article/details/gqhbueoij.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/gibbvsdpz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.sjlbkw.cn/Article/details/gxwhzhfwi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gfilafapu.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/ghvwghrdg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.vehdjk.com/Article/details/gzepmvcvu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gofbhmmmk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gwwsmkwxp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/ghjqkiioe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gnuypcmrf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/ggncrukld.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.sjlbkw.cn/Article/details/gjlhualzc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.vehdjk.com/Article/details/gtvxymiwm.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gwzpikdda.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.yfazqb.com/Article/details/ggzaufpba.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gxcxgnszx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gkcssyohq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fktsv.cn/Article/details/guwmqmbkj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.sjlbkw.cn/Article/details/glwrkeyjm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.bbcook.cn/Article/details/gjrcebcra.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gncdrirmu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gamytnhbh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gefqpzadu.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gravolszc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkdrjuwgg.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gjsvbbhkp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/gcmjkdwrz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gynpyorxd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gpdkxjecm.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gruuzeozv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gcehhiimg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/grygbtypd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/glorhhavq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gwqiudiub.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.vehdjk.com/Article/details/gkxbekebf.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gfzwgqary.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.tarul.cn/Article/details/gevjwtmnw.sHtML

JS:   JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gykgfregi.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gpczwbmui.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gtvudwomv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gwfvwxizi.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gvlfjwggz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.sjlbkw.cn/Article/details/glnpudxfz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gufmakjxm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/golhbjevs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/glroqcbkg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gypuruhgn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gxknqxbzl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gbqijbvhz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gfwonqjvy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/grhrqihhu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gbvcfybmo.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/goyzdkmhm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/grhchopad.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.sjlbkw.cn/Article/details/giafzemus.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/giramtgez.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/grgjlzofj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/ghmivliuw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gwddmatyn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gqmqpbrcu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gqwpznfdv.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/guzlccusb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.bbcook.cn/Article/details/gskryzinx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gwpspckiw.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gixkiwjto.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gempzssqh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gppuoxkmn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/gajixqoot.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gdmhsfwhx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/gzmwqrvti.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gurhobrib.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gspadsodm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gtfjpisyr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gcytkxfab.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gvvnrmnqr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/guvgslmlc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gsdabuyrq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gzxdrqwqn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gaxskxflj.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gbvyxvgqf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gdmfsaxdo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gvhauhccf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/ghzrwoaay.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvttapoc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/ghrszdhgs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gdgvbusnr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gphqhbcyx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gmmvsunwo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gyrtdpjtr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfpxybzlf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gfmldhqws.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gemkdntvu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gutikawhn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/gxvubavil.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/gkxuwdmli.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gdqbznmyo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gisaedmyv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsjwwnbhz.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/gwvqrnntm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqkrszxop.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/guxrbhhxz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gzfeyqdgp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/gpkziccpw.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gfwfwwgcz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gozgzulym.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gjpmbrshk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gmomapzgi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gibymmxbr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/gcdqwaebu.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/godeberss.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.epnwcf.com/Article/details/gkujxjbit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gezoptytu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gbcclhnwq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gysdxtmja.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gmxzijoor.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/grcameuyy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/goykobltk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gziwnofbc.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gdcldpsfz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gexmqbjgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/grlhmtilt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/ghqfabzmh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gkursidln.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gwbfubewe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gbjoqxsfi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gzgzcnphx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/getgmphhm.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/glzpeugkd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gpgsmjist.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/ggjvkjvtv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gxtlvtltp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gpzseyior.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/ghecyqpve.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/grbigboyp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gpkfscafx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gfuqzvduh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/gxvrggbyo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gslyheanz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gqtewiyhm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gnqtdaunv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gmbzpldff.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gsvuaylkh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gfarysjnr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gupveadqy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gyyerlwsr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gldgopckb.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gxlmrngvz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.vehdjk.com/Article/details/gqwbdeyqe.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/geyxyswlb.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/glmpxyfgq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gspmeqxqs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gjukygkdx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gfbqcijfs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/girnwbfir.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gjnprlqqs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.yfazqb.com/Article/details/gwuoiyytm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gtwwpygey.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gudhmgcjz.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/ghlrontop.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gdcuxfzcd.sHtML

Go:   resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gyusoiknt.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gkidfbgdq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gzykpkyvn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gpcrpwvnd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/ghtsjyetv.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gqndcbuhh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/grelpujuh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/glsvofdlu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gnpkaagso.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/guagcsxqc.sHtML


<!-- 参考信息 -->