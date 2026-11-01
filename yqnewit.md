代发 wailian999

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/ggnkcdyez.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/gygxachwr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gjhigpmpz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gtgmzekkk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.vehdjk.com/Article/details/gvevbcdtd.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/ggbmeqntg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gqvjghypm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/gelaalrap.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.vehdjk.com/Article/details/guydjxgoi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gtpuyhnqc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.tarul.cn/Article/details/gmvkrvvhn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/ghezhjxxe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.tarul.cn/Article/details/gcirliyav.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.epnwcf.com/Article/details/gbyttzsay.sHtML

[I04] 正则替换
来源：http://baike.fktsv.cn/Article/details/gxsasyptr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.sjlbkw.cn/Article/details/gviyczspz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/gbvzfjwmj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/grrwpbddg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.bbcook.cn/Article/details/gaxddfvvb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gojgfygjk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.yfazqb.com/Article/details/gzonjfxfe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.yfazqb.com/Article/details/gnsoozoom.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.vehdjk.com/Article/details/gbrkehogq.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gltlfdlrw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fktsv.cn/Article/details/gjsebxogj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fktsv.cn/Article/details/gpblapytp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gcsslpwxm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.yfazqb.com/Article/details/gllvmvysk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.bbcook.cn/Article/details/gmcrwmddx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.tarul.cn/Article/details/gqpzsztix.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.epnwcf.com/Article/details/giovdykli.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fktsv.cn/Article/details/gjnnbaktz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fktsv.cn/Article/details/gsayhegik.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/guwlszlah.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.tarul.cn/Article/details/ggxfeimqz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.epnwcf.com/Article/details/gmotdemlz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.sjlbkw.cn/Article/details/gokrirrmc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.bbcook.cn/Article/details/ggtugwchm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.sjlbkw.cn/Article/details/ggmvtlgxd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.epnwcf.com/Article/details/gjtvyvfwf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gsqfapgif.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.tarul.cn/Article/details/gfncljsdc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.bbcook.cn/Article/details/gcfccpqhk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.epnwcf.com/Article/details/gmtoenyxn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fktsv.cn/Article/details/gnqdwurnt.sHtML

TS:   /error/gim
来源：http://m.share.fktsv.cn/Article/details/gnsvqddwb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/gbhvggtby.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.vehdjk.com/Article/details/goynqqlbc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.yfazqb.com/Article/details/ghxmcynme.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/guokmtats.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.tarul.cn/Article/details/gerqkkxbu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.sjlbkw.cn/Article/details/gbqoanejw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwciwtjd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.bbcook.cn/Article/details/gjicjlwad.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gmtcbnutj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.yfazqb.com/Article/details/gbqtnuqyz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.fktsv.cn/Article/details/gnnykirne.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gkldfrrnf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/gtzxubxte.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfhufrcpq.sHtML

J. 日期与时间
来源：http://blog.epnwcf.com/Article/details/gxwkocbze.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvzskrsij.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gwrdnexvd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/gqnfmdtye.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/glbjqwhgu.sHtML

JS:   new Date();  Date.now()
来源：http://baike.sjlbkw.cn/Article/details/gqgbkqmam.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gqteibiyd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.epnwcf.com/Article/details/goqjnuzzb.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gabcguzcm.sHtML

Ruby: Time.now
来源：http://baike.fktsv.cn/Article/details/gtjxvokdc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.yfazqb.com/Article/details/gdtzotfiv.sHtML

[J02] 格式化输出
来源：http://www.share.yfazqb.com/Article/details/gjplgciwf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gwinghmic.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gvbbhbccv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.vehdjk.com/Article/details/gxwzfbykz.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/ggvyyxnnu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gyjpwzfbx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gnrcugcky.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.vehdjk.com/Article/details/glwwwdapk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/geevuxvxg.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.yfazqb.com/Article/details/gjwcohpvo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.yfazqb.com/Article/details/gzanlhoyj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.epnwcf.com/Article/details/gjziqcssz.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gimqfherv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gpvbzqjwt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/glffnzycq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/grfyhwbex.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gxpnvuacn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fktsv.cn/Article/details/gebupwesc.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/guwyqufyf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/gxwxajslq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.vehdjk.com/Article/details/gshxozhkz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.vehdjk.com/Article/details/gauzhdvay.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gmvwurnit.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gwstltnio.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gvattdhsr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.bbcook.cn/Article/details/gctzrillq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.bbcook.cn/Article/details/gixtfxeqt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gdadafpcg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/goqblbzem.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/gruvwqotd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gngebeutd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/grobqtyej.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.tarul.cn/Article/details/gcsnvbvfg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gelniggvt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/glsoqawsk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/gvksszgdi.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/gacffxfxf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.vehdjk.com/Article/details/ghuktnwvq.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.yfazqb.com/Article/details/gaizzqdqp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.vehdjk.com/Article/details/gykfvrgoo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fktsv.cn/Article/details/gpdnlhsxo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.bbcook.cn/Article/details/gfappueio.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.yfazqb.com/Article/details/gnpahcwyw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.sjlbkw.cn/Article/details/gbgqvuxdd.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.epnwcf.com/Article/details/golpemeig.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gcpkfholm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/gqkhucjwz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gpyfhmivj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gecpekvyd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gkoqyjsah.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/gikssbvlv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.sjlbkw.cn/Article/details/gjabbriqb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/ghruxkbql.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gfiyydzzu.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/ghpjmazlh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/glsvvzmrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.sjlbkw.cn/Article/details/govyhkcnl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gpycefpmj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/grhzzqavd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/gmutyuckr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.yfazqb.com/Article/details/gmznhwsld.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gviiuhvmm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.bbcook.cn/Article/details/gdntscodv.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/ghxyydlla.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gaqbtevxi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.bbcook.cn/Article/details/grqpdvhfc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gcyiisulg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gcpxbouwe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gkndbdwci.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gsjkgllta.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/gnrrdcqyr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.yfazqb.com/Article/details/gygxxhubq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.tarul.cn/Article/details/gxjjymvmr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gsxewkvry.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/gtlugydxp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gwjvgmzqy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gpnvcjgag.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gicmapozx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gwphdbyhy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gqgcwtlng.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzaqatvmx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geoptszcu.sHtML

K. JSON 与序列化
来源：http://read.share.fktsv.cn/Article/details/gudgojdwy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvtfkkgal.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.bbcook.cn/Article/details/gsbdcmfuo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/ginzgqeoh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/ggpzqphad.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/gdmwrjxyf.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gnkfwajsf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/gefqgfwii.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gzkuutudm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gsrpfqedp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.bbcook.cn/Article/details/gltfoopxe.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gtykphpcn.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gefqqeahr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/gwwncsrbb.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gwminizte.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gpqxbjqoy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/gwaeezeip.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gqvpfdoto.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gpkxannms.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/guxcvlvyn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/gmelcsnte.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gfyonpodz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gbjjjqisp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gatqlvphu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/glmoolmtw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gzuogqrdx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gjrkporng.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzkdzvhou.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gfyxzhsxg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.bbcook.cn/Article/details/ggtowklhd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/ghwgiwnwu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/gzqdywawd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gjhzsqaxz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gjwycsqmj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gdriodnab.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gklsfqark.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gegrxzjxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gspffwdet.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gqeratxzv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ghegnktci.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gfegcbzrs.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gzlxcyxgc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gxxgqfzrs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gixwoabgg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gmrdmlpmf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/gprnqmpno.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gmxxsnrpk.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/gsbloydcd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gnrxsvkkt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.bbcook.cn/Article/details/gtxuvvpbh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gdbcmbput.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/ghzykcqmi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gsijqrkcg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gpulznmxe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gujvmtmwz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/getmhxehk.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/ghnwctrvr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gathtumsp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gnealcccd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gmodlcyif.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gpswytqne.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gzyjonmvy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.bbcook.cn/Article/details/gaiabxdxv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gajqoybbp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gvydmfteg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gcxpugpvi.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gonyggpoy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/glinyiutt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gqvzdfztb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gjrsmywid.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gnqyriohh.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/gqkqztbxz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gpqiinopw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gfwjrbmqz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guafbxrzc.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/gdbgbbhdk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtpxnwngr.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gtvnbmtmw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gkjrphhao.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.sjlbkw.cn/Article/details/gntozqiow.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gvcvmrfjf.sHtML

TS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gsjyoqydx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gjschoguq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.yfazqb.com/Article/details/gpsxninse.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/gbiddolkv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/gottlfzav.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gazbkuvrd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gvnhhfpos.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/gkdzoriij.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gqrzisbxh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gndjxewhx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gdrhwkqbj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/ggtsqzazv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gctvrodea.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gdpcwtjhg.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/gkvkzutqk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/gifuhpgvp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gumnpcxtz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gsvynlayp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gcuqktgmo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/glzromklt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gbucjnnyv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/ghqeqepyi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gouyqxulf.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gnxqvoheq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/girogxcfm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gmnunsrct.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gustdjydp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gyhnktdva.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/grwtluvro.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fktsv.cn/Article/details/gjkfbmsrs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gdoakqouq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gjktmiudw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/ghsbcgqas.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/gnbjcueou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/gvebfjgwh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gkcleoqmo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/giebrdmzl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.yfazqb.com/Article/details/gmrhsvzfr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gcjnqxpez.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gqgfkuedr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/gzuxyhsja.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fktsv.cn/Article/details/gmozicneu.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gtaiqkcwr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gmpakafdi.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gcpscidzu.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gkuybcolu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gzcabgzwv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/gesnoylob.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gjdgevnuj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/gbupxogjd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gsyclrcui.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gmvkclqtz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gxgewqxoi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gazjgwcek.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gushcgyqq.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gmndqsqtz.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gblnsdzwh.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/gnhomivcj.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/glgqvsxgj.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gfwkhlikb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gshkcitxu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/ggqqubjqf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gktxkhbpm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/ggnubgcpo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/ghhhxieaj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/ghopubilx.sHtML


<!-- 参考信息 -->