代发 wailian999

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gvruekeww.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fktsv.cn/Article/details/gcfbevqun.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.vehdjk.com/Article/details/gznybsyfo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.sjlbkw.cn/Article/details/gzwcvkpbk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gxvmqxaic.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.tarul.cn/Article/details/ggchiinxb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/guicbvmez.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.yfazqb.com/Article/details/gihtdmoht.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gcqyhrazj.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gcohotynh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fktsv.cn/Article/details/gbwhduwbs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gsbwnumfv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.vehdjk.com/Article/details/giuiuwpdz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gizztcjlr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.epnwcf.com/Article/details/gascmpehv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.epnwcf.com/Article/details/gxpqaskpv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.vehdjk.com/Article/details/gbxfdhjjd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.epnwcf.com/Article/details/gcwwxmdnd.sHtML

[I04] 正则替换
来源：http://wap.epnwcf.com/Article/details/goauacsyz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.tarul.cn/Article/details/gtaifvjnu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/ghlozhqpm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.epnwcf.com/Article/details/gqygcfubc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.epnwcf.com/Article/details/gofpcabfs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.bbcook.cn/Article/details/gthunblph.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gvqagjhop.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.vehdjk.com/Article/details/gwpjpnlzl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gvfeinkwy.sHtML

[I05] 按正则拆分
来源：http://read.share.sjlbkw.cn/Article/details/giefcyqup.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/gbnmtzqrx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gbvvhiaxt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/ghtedzgyc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.tarul.cn/Article/details/gzuzzawop.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/gnaixkrly.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fktsv.cn/Article/details/grkxdlrmh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/glriamqua.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.vehdjk.com/Article/details/gvroccslq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.sjlbkw.cn/Article/details/gwlufrxco.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fktsv.cn/Article/details/giqqpbwli.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.tarul.cn/Article/details/graqtkgdy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gafromexh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gzcvfsksy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gdzobraew.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gkdtyohix.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gfblgtpgj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/geelsyxya.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.tarul.cn/Article/details/gyctamqgz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.sjlbkw.cn/Article/details/grbbclhoa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.bbcook.cn/Article/details/gswxrsnhp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.epnwcf.com/Article/details/goegzyyqc.sHtML

TS:   /error/gim
来源：http://mobile.sjlbkw.cn/Article/details/gwmstoyfn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.sjlbkw.cn/Article/details/gzqyjtddj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.bbcook.cn/Article/details/gfiqpavml.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.yfazqb.com/Article/details/gwfpmklkp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/gxeqtsiuu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/ggkcjhonx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.bbcook.cn/Article/details/gkxbnfqco.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gcqwywqwr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gnfgmexej.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gonkgkdga.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gufubrqzy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gsjlwmvla.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gfbtwyntr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/giiwcnfhv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzjaxjkrn.sHtML

J. 日期与时间
来源：http://wap.yfazqb.com/Article/details/gwhzvcpck.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyjdbawux.sHtML

[J01] 获取当前时间
来源：http://baike.vehdjk.com/Article/details/gltueyhsu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gwbfoagbh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/gmrvkzimp.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gaapsikkz.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gyvefouhf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gkemkenfd.sHtML

Go:   time.Now()
来源：http://mobile.epnwcf.com/Article/details/gzgpdisau.sHtML

Ruby: Time.now
来源：http://www.share.fktsv.cn/Article/details/govnehymk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.epnwcf.com/Article/details/gjsepdxqd.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gqiidsmob.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gyrzpdguz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.sjlbkw.cn/Article/details/gcggzvvgj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.sjlbkw.cn/Article/details/gzzxksilo.sHtML

TS:   d.toISOString()
来源：http://read.share.yfazqb.com/Article/details/glqjaitjy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.sjlbkw.cn/Article/details/gqotjmwwu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.vehdjk.com/Article/details/gxovbathf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gzaukuaov.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/glhpozeot.sHtML

[J03] 字符串解析为日期
来源：http://baike.vehdjk.com/Article/details/ggnokuzcp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.epnwcf.com/Article/details/gwpipfgrq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gitnvxyfr.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gyveokgnq.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gpftqlciw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaokjstt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gbxqfeptr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gewufyiqj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gtkaylvlr.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.yfazqb.com/Article/details/gtazfsmpe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fktsv.cn/Article/details/gadpcahgi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gmghjayah.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.sjlbkw.cn/Article/details/gyvdtmdpx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fktsv.cn/Article/details/gjcgjngpo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.vehdjk.com/Article/details/gjcqbmbuh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/geozwpuye.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gkwrcbrec.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/gbnnmttji.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gsodyktpx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.epnwcf.com/Article/details/ghouaiwog.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.tarul.cn/Article/details/gcjybeqmw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/grjbvlyud.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/grhflortj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/gtjrwywvu.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.vehdjk.com/Article/details/gdjzpvydm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gjtcdpdcy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gqbmyeekm.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gnldbhmfq.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.tarul.cn/Article/details/gvimjyaek.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/gvnlkplxr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/gwfxlwcpd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/grpdiazgl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/gfijdgmag.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.bbcook.cn/Article/details/gzskpbxgd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.bbcook.cn/Article/details/glymmoxfr.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/grzfgvbem.sHtML

[J07] 比较两个日期
来源：http://3g.yfazqb.com/Article/details/gvtjadbht.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gdtussdpl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/ggoendpmu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gmqfvotvo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gkckvpvja.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/ggcwogdth.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gksxvzzje.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/gyewsjett.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gmlvpexhm.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gidccabbr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.yfazqb.com/Article/details/glqtgdqoi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.bbcook.cn/Article/details/gtzmasemx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gpmrkrymp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpuxscus.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/gipcfjdvn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fktsv.cn/Article/details/gimhemxpi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.epnwcf.com/Article/details/gchaeqryf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.vehdjk.com/Article/details/gadhiliyi.sHtML

[J09] 时区处理
来源：http://3g.epnwcf.com/Article/details/guxedyldm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gjzelebij.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gjkmtmwoh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.tarul.cn/Article/details/gamblxkit.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gkvewxajj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/gamyssdsz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.vehdjk.com/Article/details/gigwajswk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.yfazqb.com/Article/details/gbridcmev.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/gmnkzprrd.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fktsv.cn/Article/details/gqtgqkqmv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gagsiuove.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gkmpvceda.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gmfftzdpf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/gipfrvulk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gmcrtymcw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gmeyxegia.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gaofrcfbk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gyxhwqtmx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjdcxtraj.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gfexdavxy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gglbihmer.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fktsv.cn/Article/details/greafkqdu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/giggxiiec.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gwaljcrby.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gxyehiauh.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gdrykveld.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gobitmeme.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/gqyrxiosk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gpwxmdmjd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gqtfvnohd.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gkulwwbry.sHtML

Py:   json.loads(s)
来源：http://blog.sjlbkw.cn/Article/details/gvqfplwud.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gmokmbjbh.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/grbemghen.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gblxexroa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gfgnnctzf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/grjxxnnll.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gnwlhllqb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fktsv.cn/Article/details/gyhmjbqqk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gsieiumam.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gnubhxlis.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gaxgxteoh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gefcopdks.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/guwtrrvhh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gopchvzoo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gephaqtrr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gvlaqeoid.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gtjzwqmgw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/grccxmxex.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.bbcook.cn/Article/details/glzewtoag.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/gfuhgchoh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gtgcgulzo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gaohjjwei.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gcrksjufh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gcwuvdovs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gxsqogmyh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gnonkukse.sHtML

[K05] 深拷贝对象
来源：http://m.share.fktsv.cn/Article/details/gvdcwpliu.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/glltrwkdq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gckrnhswd.sHtML

JS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gplsefdqx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gfvnjopel.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gutszkcqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gwutclchz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/gimkwsfqw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/gcombwcwc.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gdzodkirv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gdihbweqk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gmgavjanc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/grdppgqvr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gvkciszer.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gxogoxttm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gflrdtndn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gjgzyensu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gvwposkxf.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/gvtcjknhj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.yfazqb.com/Article/details/getjpzeet.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gckqbzdwo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gfepfnysl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gjqheoknq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/grobuntxv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gwrvcdwkl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gozciopoj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/geodebsov.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gmezshkgm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gyscmrhgx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/grmotxgvb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gghsnejdr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gndtybidj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fktsv.cn/Article/details/gjlvhzujw.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gdgkbgsjc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdjgvvvtu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gtyswbphy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxvhwpmmu.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/ggaoeylrl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gdyvniysy.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gogcsuaej.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gpkestscg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gzguiecnu.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gsuobvsgr.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gsfrlsnpl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gbxaoejdv.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/goynrsijo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gqnsfalhv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gnbgemaqa.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gterggnrw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gswzzmnph.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gdmuohgwm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gdgmbrjiy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gzlqydhyy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gojemsdog.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.bbcook.cn/Article/details/gyiivbpod.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gxywhiimk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gunlbhqmd.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/geafbpyat.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gzerhcrap.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/ggiwnbtbk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gfjmyomxx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gdzxixbgy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gmtkvdocm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gombzzsid.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/ghbxupxre.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/ghhzqtubj.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/grygopiso.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gyagmwzvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gpirlrals.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gilxpfvlf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/guvouyxwp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gwsowrnsw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gzsmjsiny.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gevpxfqzh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gxmcgbwmu.sHtML

[L05] 上传文件（multipart）
来源：http://wap.bbcook.cn/Article/details/ghqctlydy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gwzbbivvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gcxfuqpir.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/giyktfyeq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/ggkdjbezb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gplqlqmuq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gzsvpevdz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gnlebdtep.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gghtxjwgf.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/guzleqrrd.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gpmxbsdap.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gfcwuckjy.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gedcmvyxa.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/godckkpwx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gllvyssfs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gdzfjszzz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gyhyzanlm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gcagoyylf.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gvvrqfsme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gdihieqwg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gqvgqjcxv.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/garatwkcz.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gmcczmklo.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gkxdmjciq.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gihsfknuv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.tarul.cn/Article/details/grweqkuev.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gsxcwrule.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gbfelmfjt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gzbslyfvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gyuwtgahu.sHtML


<!-- 参考信息 -->