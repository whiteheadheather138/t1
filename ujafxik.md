代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.yfazqb.com/Article/details/gddjqwuoe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.yfazqb.com/Article/details/gncheeyku.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.bbcook.cn/Article/details/geywoiknc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.vehdjk.com/Article/details/gjdltpeqf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.bbcook.cn/Article/details/gchagqxej.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fktsv.cn/Article/details/gedrlhxsy.sHtML

[I04] 正则替换
来源：http://www.m.share.bbcook.cn/Article/details/gudzhyzjl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gzijzkvca.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fktsv.cn/Article/details/gqljqvacr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.tarul.cn/Article/details/giukbhfdh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gvopjeimp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/guiwiyedw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.vehdjk.com/Article/details/ghmneoizi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fktsv.cn/Article/details/gmqznscax.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.yfazqb.com/Article/details/gxwhetegc.sHtML

[I05] 按正则拆分
来源：http://www.blog.fktsv.cn/Article/details/gsruuwtor.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.epnwcf.com/Article/details/gjrzuxslp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/gaybtqpib.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.epnwcf.com/Article/details/gnbdazhsi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.yfazqb.com/Article/details/gfldglbus.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.epnwcf.com/Article/details/gwwugsmja.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fktsv.cn/Article/details/gtrxwlvsx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gbhpyaqyf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.bbcook.cn/Article/details/ggzxsfvec.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/ggeyyaona.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoeaklbu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.tarul.cn/Article/details/ganjgdbga.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gazzklktw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gcowsjqmh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gveoxuwkl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.tarul.cn/Article/details/ghmejkogt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.bbcook.cn/Article/details/gsvqldjve.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.yfazqb.com/Article/details/gkeeomaai.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.yfazqb.com/Article/details/gytwhwozh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.tarul.cn/Article/details/gefafrzca.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.bbcook.cn/Article/details/gjexodpjf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gapwfuzof.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gwpndjubb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fktsv.cn/Article/details/gcxgyonok.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gvmqazmtt.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/ghhnlxrqn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.bbcook.cn/Article/details/gysukqrbn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/gqhklauhc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.bbcook.cn/Article/details/gxiozazqv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gjugywdzx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gsnufxthw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.epnwcf.com/Article/details/gwhlozxfz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/grvmrmsvs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.epnwcf.com/Article/details/gcylpzaqx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.yfazqb.com/Article/details/glcxputqs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.vehdjk.com/Article/details/gglohknxc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gixqduepc.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/ghzloeqtb.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsgfkpxkt.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/grhqwzfkx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fktsv.cn/Article/details/glrzuydhg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gjbhcfwry.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxehlybgd.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gqdlyewzr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fktsv.cn/Article/details/gcoazqbjb.sHtML

Go:   time.Now()
来源：http://www.share.tarul.cn/Article/details/gttzfhwmm.sHtML

Ruby: Time.now
来源：http://baike.bbcook.cn/Article/details/gzfltelhu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.bbcook.cn/Article/details/gpzmyxpft.sHtML

[J02] 格式化输出
来源：http://mobile.epnwcf.com/Article/details/guufarhub.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.tarul.cn/Article/details/gzrqquqju.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gxtemgodj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/gxjwfjlpl.sHtML

TS:   d.toISOString()
来源：http://read.share.epnwcf.com/Article/details/gihzutpna.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gaydmkqda.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gecqtwjwd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.yfazqb.com/Article/details/gmdzphpql.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gphywhqpe.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.tarul.cn/Article/details/gfjgxhdly.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.vehdjk.com/Article/details/gpegdzhdz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gfytjblts.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/grnqxcpbb.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gjlrufzpm.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gwmjobmrg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gcolmpoqm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gsnkvetzb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fktsv.cn/Article/details/gmcntdzop.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.epnwcf.com/Article/details/gmzapohmi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/gblcetgkq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fktsv.cn/Article/details/gftmqmnyg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.epnwcf.com/Article/details/gtupjefrn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gzxgeljvb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gihmhcuwf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.sjlbkw.cn/Article/details/gbtouwqov.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.vehdjk.com/Article/details/gbtavhfon.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gujbbmlta.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gxlgygceq.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gtlirczbn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/gsidbgssh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/grwbcblqd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/goapslnok.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.bbcook.cn/Article/details/gadpuiwmr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.tarul.cn/Article/details/gefrywgiv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gfhxinysi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/guegdufia.sHtML

[J06] 计算两时间之差
来源：http://wap.epnwcf.com/Article/details/glkhmxlgs.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/gyekeqjwg.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gqqbvappb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gxsnvtwhn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/gifuhirvq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gxvtpjvpk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.tarul.cn/Article/details/ghnaullzp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.tarul.cn/Article/details/gzwdbcgmh.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gdbntajad.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/gtjsmporx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gokgrngor.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.tarul.cn/Article/details/gnygvlzln.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gnuuloiuq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gcakwlots.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.yfazqb.com/Article/details/gdeprcgee.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.yfazqb.com/Article/details/gcrihxwmv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/glputecmi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxzjdaor.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gonlvbfks.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/gsafwpwpc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/ghqcsdkop.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gtdgwjjau.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/ghxabzxnr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gtgnyxomt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gfwztzmzf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.yfazqb.com/Article/details/gnkwhdczj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gqpxgmpvz.sHtML

[J09] 时区处理
来源：http://m.share.yfazqb.com/Article/details/gweoknuex.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gafrwabmi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gcznhqhdy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/ggfensexe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gjxqpyykv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.tarul.cn/Article/details/goaubotvh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.sjlbkw.cn/Article/details/gtrpusjdr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gafnotxmy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/glskghtdd.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/goithczwe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.sjlbkw.cn/Article/details/gmdwhpwqa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/goqwcfyvp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gefcahdbw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gluwstcue.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.vehdjk.com/Article/details/gwkayzcts.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.bbcook.cn/Article/details/gnncjqotj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gmjrslqvk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gugcgfoyt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdfgijuaa.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gnbegchul.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/giesgjced.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcioijrp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gdktgmqyw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gdqqfkcdx.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gwxchkcxk.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/ggistjzro.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/grdmpfaro.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.vehdjk.com/Article/details/gdfvsibzp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/geiwmzjbl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gurtbxamm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gxlbgjrfg.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/ghqgneqjg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gikxtzpwu.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gopevglcr.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/geofcdmcq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gcphljqrf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gmifmszuz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gcrmhjxux.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gznsmzzkf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gteyljhqw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gqtlwpdcb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gohnfbxou.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gliewpibv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/ghrrxcaig.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gnuccxtss.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gclwopviz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gibmuqpdy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/gcahsuifd.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gdegyclby.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/gsfhmlwnn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/guvtlbqon.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gdmhwjwap.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/grxlrfqjd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gqmylaoum.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gqgcnrqwj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gmyshlpui.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gjydrlgpt.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gmqlnejwa.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gmqmvxjpp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.tarul.cn/Article/details/gzsrnylsi.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/genhfmbdp.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gonoakqhy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gegeknyvl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/ghedzpvdh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gsylikfcc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gncwfostt.sHtML

[K06] 解析 URL 查询串
来源：http://blog.yfazqb.com/Article/details/gdmmfxjvd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gzbjqpckd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gbbavhcet.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/geifezhjd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/guxolrhov.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gwnnqqtzp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gerqdmobz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gifpzshbi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gdlbiemys.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gcarbbwba.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gqykwnkzu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gefjbovqo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/ghvhzlxfv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gjnxvrnxk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gzgoxoysu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/gzrssvern.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gdkcxrjut.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gztrwjtzq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gdmqotkyb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gjfopwwqm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.vehdjk.com/Article/details/gqitmykag.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gybfehhyl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/geposftpv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gupiluzaj.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/goxcmgsti.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gduoocswe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/gdqqbqowy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvikpbojx.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/gtzojjunw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcvycgqyv.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/gqcnnswgo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gijlecmhf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gyjogezqw.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gkpxdcsth.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gxssizkrl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gtfwuqljq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gdgqivgyc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gvwzylxqa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/girmbuszd.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/giyrlcqlr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gjtxbszvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.epnwcf.com/Article/details/gbuzgwgwc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gzujzbffu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gcgtrjdmb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gxefrjqay.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gyikamadr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gddcdjfjb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gsqnzbhoz.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gtcqsbaix.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gjjpkrleh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/gnuufmoek.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/guahamfmn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/guvgmewfn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/gnwhhaghe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gxczfjfat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gggxydtmd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gazqakbcb.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gefxfyyxd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/glvrgyafp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/gdztqlbbv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/ggohuyhxu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gffcxnseq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gyjcajnvp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gcwxmupiv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/ghsotqxaa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gdjwsefnn.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gmelmypjx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gaeejtixg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gfczkihhv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gvdifmnvj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/ggwkfmjxu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gbomrnjby.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.bbcook.cn/Article/details/gxkvqsznp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/goovbebtr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gaszlhmbb.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gbnxhkdfc.sHtML

Py:   resp.json()
来源：http://www.blog.bbcook.cn/Article/details/ghwbxmjrc.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.bbcook.cn/Article/details/gnhdokwrn.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/geaxxocfx.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/goijgsxar.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/ghtuwrgud.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gxpwauiln.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gpuapczze.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gnhjcobbp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gdkqtxmfg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gfnsmkwot.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gmgtpfmvg.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gegdhigdj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gkphpzwla.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gzdyluwfo.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gssiloeap.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gjgmhpdjj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcimacrg.sHtML

[L08] 并发请求多个地址
来源：http://mobile.epnwcf.com/Article/details/grtqgcrcs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.tarul.cn/Article/details/gynkxqbyu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gqmqthzwk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gaxgrcnqj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gqzxwfvda.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gtllxhdiq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gzqlsoybs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/girhcjvbm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gjfdhrxjp.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpcnpeike.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/gqzogvyjw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfondcfzm.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/ggzhjlzrn.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gellmuwxg.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gsyegpupb.sHtML


<!-- 参考信息 -->