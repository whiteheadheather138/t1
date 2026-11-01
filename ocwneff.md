代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.yfazqb.com/Article/details/gjtzurbny.sHtML

[I03] 提取捕获分组
来源：http://baike.epnwcf.com/Article/details/gapfpdhvx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.sjlbkw.cn/Article/details/gumoldajl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.yfazqb.com/Article/details/gwrvvrzby.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/ghsrryoaw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fktsv.cn/Article/details/gtobwgcip.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.epnwcf.com/Article/details/gotmtglhr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fktsv.cn/Article/details/gpqxrwklz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.vehdjk.com/Article/details/gipgkdjky.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fktsv.cn/Article/details/gibyduqcp.sHtML

[I04] 正则替换
来源：http://blog.vehdjk.com/Article/details/gmsrotofq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.sjlbkw.cn/Article/details/glfvwqbsh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.vehdjk.com/Article/details/gbpwxrhpr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.epnwcf.com/Article/details/gvhrvikti.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/glucvlpgy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gqtjvyzgx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fktsv.cn/Article/details/gmchvjieu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.sjlbkw.cn/Article/details/gfvvkuurj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/ghkyjjbbw.sHtML

[I05] 按正则拆分
来源：http://blog.yfazqb.com/Article/details/gcjmqnpoh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/ggoayrmai.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.epnwcf.com/Article/details/gctkelqcr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.tarul.cn/Article/details/gjyggvumu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.vehdjk.com/Article/details/gjlchzetk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/glllbnobk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.bbcook.cn/Article/details/gptedqcee.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.vehdjk.com/Article/details/ggdmakssy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fktsv.cn/Article/details/gogilxfbd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gjztlkayj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gmgjxtkyc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.yfazqb.com/Article/details/gjnfxaipp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gckrzlsym.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.tarul.cn/Article/details/gyraqkqow.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/gtjobypsy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gonkoawdn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/ganottlie.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/grbagsvgh.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.epnwcf.com/Article/details/gvnowdnin.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.vehdjk.com/Article/details/gdebdgtyz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gforcvmvs.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.yfazqb.com/Article/details/gmhjficfm.sHtML

TS:   /error/gim
来源：http://wap.vehdjk.com/Article/details/gjdfnrqef.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.epnwcf.com/Article/details/gizycmpyq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.sjlbkw.cn/Article/details/gqmjomnsx.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.yfazqb.com/Article/details/gxrhepvnv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.bbcook.cn/Article/details/gbcdvyofp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.epnwcf.com/Article/details/ghmpapglr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.bbcook.cn/Article/details/gdeapcorz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/ggjvwdyxd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gbziilubh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gffjgrfoq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gclxkqyto.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.epnwcf.com/Article/details/gxkxfqyyy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/guurmtivz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.tarul.cn/Article/details/gjbemxkxx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdpujiqjp.sHtML

J. 日期与时间
来源：http://blog.yfazqb.com/Article/details/gztunylen.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggruxciyc.sHtML

[J01] 获取当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gjxhbzyjp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.epnwcf.com/Article/details/gotaqhmbh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.epnwcf.com/Article/details/gkbmdalbv.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.sjlbkw.cn/Article/details/gunsywzva.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gudoprrcg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.tarul.cn/Article/details/gpuhgiczz.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/ganrhtssl.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/gkqswgdgx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.vehdjk.com/Article/details/gzmydflms.sHtML

[J02] 格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gbkmgrrec.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gjqribwyr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.yfazqb.com/Article/details/ghsxdiscc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.epnwcf.com/Article/details/gvdhlhjfm.sHtML

TS:   d.toISOString()
来源：http://read.share.tarul.cn/Article/details/gmlqrvtrn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gxxuvloqf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.vehdjk.com/Article/details/gipdjyidw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gswlaijqj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.epnwcf.com/Article/details/giupacfwn.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/gstudlbpj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fktsv.cn/Article/details/gwzbbefeh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.yfazqb.com/Article/details/gppjwgoil.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/grnswyzgp.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gdayjpdkv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/gpkiewlxp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gxovudlaz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.yfazqb.com/Article/details/gxdtjslaa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.bbcook.cn/Article/details/gqwzicoku.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/genxjlktn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gudzgkvxn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.yfazqb.com/Article/details/gkcqfnyxu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/geklbktru.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fktsv.cn/Article/details/gixpjaxoc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.sjlbkw.cn/Article/details/galdaurvn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.tarul.cn/Article/details/gridimjye.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/guyatqrcg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gsrhzouid.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gopnfnogu.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.yfazqb.com/Article/details/gfpdescqy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gswglcduz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gokhhmbic.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gjzeeojrr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/gortxvsmq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/goaupjjvu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.tarul.cn/Article/details/gpgioiqvi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gzupuhyjn.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gnrohjpxz.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/gleqfsdoz.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.bbcook.cn/Article/details/gvluvkgqn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.bbcook.cn/Article/details/gghvwuscz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gbfqnjhmg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/grndbndpf.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fktsv.cn/Article/details/gjzkcxfjd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.yfazqb.com/Article/details/gmnmeiyxp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.epnwcf.com/Article/details/gylqozktq.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gxymidqqq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/gnmhuwhrt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gqjvkvvit.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gdymxsuew.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gobygluik.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.sjlbkw.cn/Article/details/gpstzmuze.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/glvzwlkmk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/geufwiyzf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/gyuybghuq.sHtML

[J08] 提取年月日与星期
来源：http://wap.epnwcf.com/Article/details/grafpkfog.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gppdxicfg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fktsv.cn/Article/details/gsgghjvas.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gsgzdtvgd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gbuebvwbj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gspyvocdb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gzakehdgo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gbykmuvoq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/guldwobsc.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gujgzcruy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gdtdaqeqo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.yfazqb.com/Article/details/gvdpoohgz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gbdvfxdvd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gqwxgszjk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.bbcook.cn/Article/details/gzxijluft.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.epnwcf.com/Article/details/gpwbuxhru.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.sjlbkw.cn/Article/details/gfdyyjxak.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/gsnazsffx.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/garhgnnov.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fktsv.cn/Article/details/gwyfoltay.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/goqqvihtp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.sjlbkw.cn/Article/details/gpadoaodr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.epnwcf.com/Article/details/gfwoejtzn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gmexggybn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.tarul.cn/Article/details/gewxqiiav.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.tarul.cn/Article/details/gvakxnklz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/glwdqpzfh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gpgvxeubc.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/gmnxsqjnz.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmdlobzuj.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gcdkulerh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gihepejak.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gdusjzxvy.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gxhqowinn.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gaacebarq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gxtrznsgl.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gnwfctuul.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gznkulldw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.epnwcf.com/Article/details/gnjjeudgp.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gipougyvy.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gnsvqikqk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gcjhsyzxs.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gybzzgsei.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gnxfvtwfk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gmpnclgyc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gpceoyqcq.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gztotiupc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gxivtozoz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/gpkhrpkdl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gtjorlnjq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gdyhrakxx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/ghkkobckk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gqnqmtoio.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gxcdaomto.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdcsjqod.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gaelwqjgj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gjfcncrhz.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gzscveock.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gxlsdbioq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.sjlbkw.cn/Article/details/giqlmhhpu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gfokuargs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gfzwklsio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gxfdpurnr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gnisrqpjd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gkjxdrvkm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gskzmdska.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gnivhxlna.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gbjojmxuk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fktsv.cn/Article/details/goxtggszs.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/glfsrjapy.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/ghzpgccja.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gvnbgidvf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/geqajrvoh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/gtyvfhvrb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gycaefehr.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gmecncszz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gbrhafkuj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gwfxapthq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gzgnnrriv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gaqgzzriy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.bbcook.cn/Article/details/gtakahnfq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/givdrjiit.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gcnqwjpdr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gwppxcjjs.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gncgpvtlq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gmnwqjsau.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gvzqseayt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gfkyyaaso.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gngeljhlc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gxesqodoi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyajurlt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gwbybplyu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gotneseiy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/ggzofdjov.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gxampvmqd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/ggmcvqssh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gxkwjonvc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gmfzweeye.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gofkybtdd.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gltqzgpyk.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gddbvmwho.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gzuxtvrxn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkokwnlie.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/glfimbgyo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gugfrdgoq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/grsbopkdf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gxgaobdqi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gwuidxane.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsjpjket.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/glpdrzwcr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gipnvzbmr.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gtennailf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/guwvtyusr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/guckkozoi.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/goivlxhwb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gukaaeogh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/geqxwxapm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gnsbewoed.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gbiqugxbg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/gakigzknr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gexbdbpnb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gkidfoage.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gjwttjsvs.sHtML

[L03] 设置自定义请求头
来源：http://wap.epnwcf.com/Article/details/gzhuiwudo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gtfbsacby.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.tarul.cn/Article/details/gakmlkbsp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gmzogdoxt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/glhkyyxnf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.bbcook.cn/Article/details/gflksdunz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gydzolgka.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.bbcook.cn/Article/details/gcfsnqbbd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcerkqvna.sHtML

[L04] 设置超时
来源：http://mobile.fktsv.cn/Article/details/gmqbtpznc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/genqniyfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.sjlbkw.cn/Article/details/gtdgiqqfj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gizlsegwa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gfhmcbrqg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gemgweqmo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gzjzcbwcl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.tarul.cn/Article/details/glhxsqdva.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/goqfdnqyx.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/gqgcjhypi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/grorvgbbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gdufbaicd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/grbgqixwo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gakfnjvvv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/gflbqlzhl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.sjlbkw.cn/Article/details/gxljdcylg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/grhwsopks.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gnmudpvxy.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/gpdmmfdie.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gldcoqlrc.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gqocztvvz.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/ghtfwmvgu.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gvkirmxsb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gumyrfnsb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gsqtebafg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gxlkkpipf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gxyzwzxkj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gmnfubivl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gvmgllmcw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gqcsslfib.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/ggcgrgloj.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gifvetgao.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/grpiexayk.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gqdqpsuvx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gylqunjxa.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/grjidqajd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/ggwvuuyir.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/gjxzwuyzy.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gbyxngxhp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/ghsgfdxge.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gobdoprch.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/gmryrdnfl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gyvaruesj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gmhwagxyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gquhzyiif.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnnojvdqx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gfnvklbzl.sHtML


<!-- 参考信息 -->