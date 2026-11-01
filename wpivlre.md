代发 wailian999

[I02] 提取所有匹配
来源：http://wap.tarul.cn/Article/details/gsnrypsot.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gphrmtbjt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.sjlbkw.cn/Article/details/gkwwgrklt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.tarul.cn/Article/details/gidnbbupl.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.bbcook.cn/Article/details/gmowvewby.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvgtdiule.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fktsv.cn/Article/details/gjwvnddbn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.epnwcf.com/Article/details/gfaiahpqt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/givteppzq.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gdxrgeezn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/glbjkefwv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.tarul.cn/Article/details/gcuuycvfs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gnjthaszg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.vehdjk.com/Article/details/gcrcguuxm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gwoqisbxp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.sjlbkw.cn/Article/details/gskbzbpzr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.bbcook.cn/Article/details/gfczderrw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.epnwcf.com/Article/details/ghabcsbcz.sHtML

[I04] 正则替换
来源：http://baike.vehdjk.com/Article/details/gcdtmswnf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.yfazqb.com/Article/details/gdhukwlor.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.vehdjk.com/Article/details/ggwmiznha.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gpzywhlda.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/glxzzeyey.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.tarul.cn/Article/details/gbwzcqabu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.sjlbkw.cn/Article/details/gmtzkndze.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gfjuaoswp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.epnwcf.com/Article/details/grzgwyqri.sHtML

[I05] 按正则拆分
来源：http://m.share.epnwcf.com/Article/details/getshwdzy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.tarul.cn/Article/details/glzuqccjx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/glsokkbcu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.yfazqb.com/Article/details/gjbahcpru.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.yfazqb.com/Article/details/gbiwlnytu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fktsv.cn/Article/details/gcebtdiwh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gkybnnrts.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gdlsmclzk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.yfazqb.com/Article/details/grbxaodqi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.yfazqb.com/Article/details/gjmdssgvm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gljqwizem.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fktsv.cn/Article/details/gzeyuhlvv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.vehdjk.com/Article/details/gnxecvcst.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fktsv.cn/Article/details/guvqnawyi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.tarul.cn/Article/details/gcxhqpfnh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.epnwcf.com/Article/details/giojdagvv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.epnwcf.com/Article/details/gmfflxlrt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gfobblekq.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.yfazqb.com/Article/details/goyobyepw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.yfazqb.com/Article/details/gmfjubxfe.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fktsv.cn/Article/details/gtvbrxdgv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.epnwcf.com/Article/details/gaofpjwkv.sHtML

TS:   /error/gim
来源：http://m.share.tarul.cn/Article/details/gkjxyauqy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fktsv.cn/Article/details/gruzvnsrg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/glwbnpwle.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/gzviomgxy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.yfazqb.com/Article/details/gybsysbaf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.yfazqb.com/Article/details/guomwvkwp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.sjlbkw.cn/Article/details/gbylfhdem.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gpeilwupz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gswirfxmn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.sjlbkw.cn/Article/details/gevjamdvp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gbwjjacfg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gtzppvfgq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/gvcjbfuem.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/giuctxrbu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbentgeat.sHtML

J. 日期与时间
来源：http://blog.fktsv.cn/Article/details/gjvqvofft.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzyhrtktb.sHtML

[J01] 获取当前时间
来源：http://blog.yfazqb.com/Article/details/gowsisebf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.vehdjk.com/Article/details/gmdnzkbus.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/gaayjutsx.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gqrzthzjv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.epnwcf.com/Article/details/ggltfdmtv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.epnwcf.com/Article/details/gmwlyxwwa.sHtML

Go:   time.Now()
来源：http://www.share.sjlbkw.cn/Article/details/ggxdduvcz.sHtML

Ruby: Time.now
来源：http://3g.tarul.cn/Article/details/goltazsnb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/gtddyxxen.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/grmgpockt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/guexmsqwd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gacgrcoha.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.epnwcf.com/Article/details/gyvjgoaeq.sHtML

TS:   d.toISOString()
来源：http://www.blog.bbcook.cn/Article/details/gndnwiuls.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gfkgpvzie.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.yfazqb.com/Article/details/gbofznmjt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gqjzunpzi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gebpqvhwf.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gbkntyaqo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.sjlbkw.cn/Article/details/gausnsfjo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.vehdjk.com/Article/details/grarnfykj.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gztdczuis.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gcycsyvxg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gwddguqoo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gkvjtoqik.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/grvhtztfq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/gefjyvlyj.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fktsv.cn/Article/details/gcbmsyqnh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/ginpnbnkx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/ggthjkxrs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/ghkmourwb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/guqubizjp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.sjlbkw.cn/Article/details/gwqayidij.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.vehdjk.com/Article/details/gmbxkpvmr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gibdywupa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/gkwahrhhl.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gksxxzxjk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.yfazqb.com/Article/details/gawlwkflb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gyjwzpuem.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/galnohnhl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gmhiidzpl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/goqspqmei.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.epnwcf.com/Article/details/gycjvosqs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gveqteogq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gkniiykln.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gkjgieoqq.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gelqafdqk.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gkbexdnyf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fktsv.cn/Article/details/gnhunfhgp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/gijjmvvvf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gqkwaqwke.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.sjlbkw.cn/Article/details/gtspilwgw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/gfbrcvwzc.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/gdupjneid.sHtML

[J07] 比较两个日期
来源：http://www.share.fktsv.cn/Article/details/gyvdzwrdl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gjqidmqfk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.epnwcf.com/Article/details/gamazrtts.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gfxmgneqx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/geqlfyftf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gxgwyvljc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/gdgkfwehd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gsqinozyy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gkitvclkt.sHtML

[J08] 提取年月日与星期
来源：http://3g.bbcook.cn/Article/details/gbjnkucpc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gxougehuf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fktsv.cn/Article/details/gzdqwysyc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/gngjlebcn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fktsv.cn/Article/details/gymfcbptn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gkwlibmcw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.tarul.cn/Article/details/goiuutfpg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.yfazqb.com/Article/details/guahglelz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.sjlbkw.cn/Article/details/gyynhwcxq.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/ghvbprhbp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.tarul.cn/Article/details/gaucvnktq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gpiuhuiwe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gdqujpupy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gbhzhwgjf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.bbcook.cn/Article/details/gncemofyt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/goognpiph.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/gunesyphz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.tarul.cn/Article/details/gylqaagwr.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.tarul.cn/Article/details/gwjsokekx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.tarul.cn/Article/details/gotfjezkn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.bbcook.cn/Article/details/gmuczyhiu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gqyhfdhdb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gslpgbxqh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.epnwcf.com/Article/details/gytgtyjee.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gyriyvxlw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/gyxlgybep.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gmbsonnss.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giqatjswr.sHtML

K. JSON 与序列化
来源：http://mobile.epnwcf.com/Article/details/gcmggtstt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnrtxswgr.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/grgdijzxf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gxwdtnsyv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gkhhnspiw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/gpczaxwak.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gaauilnsv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gqumlnbgp.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fktsv.cn/Article/details/gyxhooeeh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/gweudhxib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/gwwnafhjx.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gmghsxcnu.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gajsupfel.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gnnqrmycn.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxvvsxjqf.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmvyktynb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gorlwvxog.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/guddsjfty.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gvnktkyax.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/grnycjxfp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gnfursymy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/garmjkbjx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gwmytzlvr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gfzmrgqnq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gijkotktm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gvoqhyzxc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.vehdjk.com/Article/details/goggwukch.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.tarul.cn/Article/details/gkbiebrak.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gewkjdyme.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/ggmdbhjvu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/gxegztenb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.tarul.cn/Article/details/gsvjjhjkh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gsmejzvcr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gkuiymckg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.epnwcf.com/Article/details/glfmnykjg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gzvwoptla.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/geddztcoa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.tarul.cn/Article/details/gwbhoxjsi.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/gwuonuene.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gbrwxldak.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gzztwomsu.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gnerbicqv.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gwiacprpk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gbtrwjqow.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gknkuujev.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/gfwtpvaqr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gexaodnjt.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gbzefpldx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gpwnplkal.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/gjlljbqmv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gdvyrhjqw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gzoxejane.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gpphjobwb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gvnnavver.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gygrloubz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gjotklirq.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/grzclowuq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gofmoqzwq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gexwvhboa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gacmgelfh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/ghqnluqid.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gncrqsfbj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/grklorscr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gsbciixik.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/ghzyokjke.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/ggzrzyrir.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gwgcqjtix.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.vehdjk.com/Article/details/gjmddipsk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gwesbigxs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/goyzpnlmh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/gnofycmoc.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gekoujymd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxvdlrhkj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gvzzrfftg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpnmhmnsz.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gdbjtvoqq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/giwsfhaje.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gtggtwwyo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/grjfwypwh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gcraxeacb.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/glzriugly.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gkgioicxh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gspwmbmhy.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/gaafsryac.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gkogzicth.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gdkdhevid.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gaotnffwr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/grkbvvpsv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/govgivtux.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gcrzsegjk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gjpmfxuhe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gvyrbhjgl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gexkmergd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/glhxjesvh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gmlwpbehq.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/gssbxquiw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/gjhjfadid.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/ggxbvkeag.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gribidabu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gnmjgccrl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gqppvdjaq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/guiwcyaim.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gkxbwmaec.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gkewimvkj.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gujslyqav.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gtkklpshl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gjsipngxb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gewuwseie.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gezxuttvo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gleeqrvlf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/germvessy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gaukitswd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gscbtaxae.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/giwqzsfut.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gccvywsga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gkubcleqa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gdvfeyoqo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/ggwwzizkz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gtemoaumw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gbmiblvus.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gnzgcduoo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/guupzxynx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/glgrkmoyw.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gyfadnlns.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gfjsdeclj.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gwssqceht.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/ghesoomlg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gyalozjye.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gfbchsrht.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gqornbusb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/glanmkywa.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/ggudebhzo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gxtbvzfds.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gwtztevkq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gxazdlfta.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gqvfcpwdg.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gudvkviej.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/grdfwryja.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gmaorkcpx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gnercncjc.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/ghvxsxmab.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gfajeeawt.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gxstfkfja.sHtML


<!-- 参考信息 -->