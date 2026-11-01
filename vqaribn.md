代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.yfazqb.com/Article/details/gsaljtbfm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gvvmkeicw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/gbbxwzgtw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.bbcook.cn/Article/details/gbtoliycp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.epnwcf.com/Article/details/gsjtkodef.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.tarul.cn/Article/details/ggmmidkwt.sHtML

[I04] 正则替换
来源：http://3g.bbcook.cn/Article/details/ggkaapzvq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.yfazqb.com/Article/details/gxkqeexig.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gphitcaac.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.epnwcf.com/Article/details/gystlwrdc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.vehdjk.com/Article/details/gkcqooanx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gcuegkxxh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.bbcook.cn/Article/details/gbywyloqn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/gnuydxvzo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/gcmnhheyr.sHtML

[I05] 按正则拆分
来源：http://baike.sjlbkw.cn/Article/details/gebigkoet.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/goimzchag.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.tarul.cn/Article/details/gpyttsvfl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/grxxglncz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.vehdjk.com/Article/details/gcsoioipl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.epnwcf.com/Article/details/gubqopnxf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gryoruami.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gicvsoafx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.epnwcf.com/Article/details/gucbryanp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gajtnwpal.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gztwafgte.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.vehdjk.com/Article/details/gnmkfmxhx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gdnzupdra.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gzcittsoc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.bbcook.cn/Article/details/gmsocllnv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.epnwcf.com/Article/details/gvkwvinza.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.bbcook.cn/Article/details/gfbfkluna.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fktsv.cn/Article/details/gnatcvaut.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gsvuewrgq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gqztiyfol.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.vehdjk.com/Article/details/gsqwskcdi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnxbjvlz.sHtML

TS:   /error/gim
来源：http://www.share.fktsv.cn/Article/details/gizxdpitz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.sjlbkw.cn/Article/details/gpvedthlc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqetyajn.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gqcjlvqnx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.bbcook.cn/Article/details/geixereor.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gqnllhkvl.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fktsv.cn/Article/details/gkbylqfnx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.sjlbkw.cn/Article/details/grtvgdmao.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.bbcook.cn/Article/details/gnqyoynru.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.bbcook.cn/Article/details/gjmpizydp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gfpgumgqm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.bbcook.cn/Article/details/goaklqcgh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.yfazqb.com/Article/details/gigdxsdzk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.sjlbkw.cn/Article/details/geeivdian.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwpigxdnd.sHtML

J. 日期与时间
来源：http://3g.epnwcf.com/Article/details/gzgdvaomt.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gibegptdm.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gborwoqrc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.sjlbkw.cn/Article/details/gtzueyuol.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gkcbwfuwu.sHtML

JS:   new Date();  Date.now()
来源：http://wap.sjlbkw.cn/Article/details/gdpxdlklc.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/glnunycru.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.yfazqb.com/Article/details/ggfdvrfep.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/ggjfyletu.sHtML

Ruby: Time.now
来源：http://3g.vehdjk.com/Article/details/grelstsxu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.epnwcf.com/Article/details/gjyvzpixs.sHtML

[J02] 格式化输出
来源：http://baike.vehdjk.com/Article/details/gsyevlvfm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gygoomoya.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzgezrsd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.yfazqb.com/Article/details/gfdxojtzv.sHtML

TS:   d.toISOString()
来源：http://baike.fktsv.cn/Article/details/gqsexraup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.sjlbkw.cn/Article/details/gtecwphyh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.tarul.cn/Article/details/gpyggidtj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gkzwpcept.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.yfazqb.com/Article/details/gurjzhzzy.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/giytfpwny.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fktsv.cn/Article/details/gszdpqdxp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.sjlbkw.cn/Article/details/gkidlkmkl.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gtaolvmkd.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gyxrsezur.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gfwmsnkgt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gswwrahxs.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/glhwzabfs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.bbcook.cn/Article/details/gcnvjeuzn.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.bbcook.cn/Article/details/gnprbnqbd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.epnwcf.com/Article/details/glecrlokg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gbafspysp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gorielogt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gvukivhst.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gdrytissq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.epnwcf.com/Article/details/gdepzuzcp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/gedpfbpav.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fktsv.cn/Article/details/gbxqmjsqy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.bbcook.cn/Article/details/gncpfuags.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gdsyshfwx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.yfazqb.com/Article/details/gvdiqaeog.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.tarul.cn/Article/details/ghcowjumt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gvlqwtobh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.vehdjk.com/Article/details/gyyubatxp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/gdyxkepvk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/gmsklerbd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.vehdjk.com/Article/details/gttjuvkol.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gtkhgioje.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fktsv.cn/Article/details/gphcgjrdo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fktsv.cn/Article/details/gpakhahin.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.bbcook.cn/Article/details/gfyfvmdjn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gleuscfcc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.sjlbkw.cn/Article/details/ggpefbkqd.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.tarul.cn/Article/details/gxcivssqb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gobcbjfwp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.yfazqb.com/Article/details/gdbxtzsfy.sHtML

[J07] 比较两个日期
来源：http://read.share.tarul.cn/Article/details/gaepmkjuj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/gezejaqcn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/ggzmbifqw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gjcbenkkq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gonarbvyx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gtbldkhkj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gfjrdcofo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.yfazqb.com/Article/details/gurynczqt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fktsv.cn/Article/details/gzyxpcerk.sHtML

[J08] 提取年月日与星期
来源：http://read.share.sjlbkw.cn/Article/details/gpqvimfqb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gopfliikx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gfwwalqxz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.vehdjk.com/Article/details/gkuqsimno.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.epnwcf.com/Article/details/goswedako.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fktsv.cn/Article/details/gltxeotzw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gcoolkarm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gqrmtlctp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/gpiliwhnk.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/gkeiwalpw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.bbcook.cn/Article/details/gcshkuarq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.sjlbkw.cn/Article/details/gouhlxuxq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.tarul.cn/Article/details/gvycdcljr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/gklwhfbbz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fktsv.cn/Article/details/gzvxjxhfv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.bbcook.cn/Article/details/gsyhlofad.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.bbcook.cn/Article/details/gpzkcfwxs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/grepskeaa.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gphyuxvda.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fktsv.cn/Article/details/gicegndob.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gofrsbwfp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/gjbvxncte.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gtnjwqgoh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcbmioama.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gnvffebmk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.vehdjk.com/Article/details/gwbfmqpcx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gguuqgzhl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gogsubyrc.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/ggscximaz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gjfpsfzxn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.yfazqb.com/Article/details/gsfyywsui.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gycltiuze.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gtipinnoi.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmdwqajrg.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/ghecpryer.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gwsxgeiov.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.yfazqb.com/Article/details/guajzqyqg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gypnhqvxc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/galptxkjf.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/gyxpfznna.sHtML

Py:   json.loads(s)
来源：http://www.m.share.vehdjk.com/Article/details/geosrfrcx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gbllawysy.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtycdnadn.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/givwrvrqj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gxxyczpbp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/grpqlulxh.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gcjoajxvp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gwiaopukr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/gtppwifny.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gpigwuiff.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gjcsybgqt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gxeuofxwq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gzokpmjlv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gbkhcyipz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gjokctwhd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gmkkswbom.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gtbdwcgqg.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gvruzxndz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.epnwcf.com/Article/details/grpxbupqx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gfsqplbbk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gglzougbm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gwvzmlghn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/gtjaqvqip.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/guzvwetye.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gdqgdozzu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gtbpszcbk.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gphtgowjh.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/gdjskysxg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/grssndjgg.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gqenqdxtl.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gecueydjv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gfjngqdrg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gztyctxhz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gshxilugt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/geyvfnfln.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fktsv.cn/Article/details/gzeprzssx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gjhpkcrbb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gxafeyurx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gzzycwkzo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/giprxdrpb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gbfbejzmc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gcnjfwatu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gmlhauksl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gpbhvvfks.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/gctvoljfd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gfuejarwp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/ghdtvnuwc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gmoqceocv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gkfhmgdqf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/guyltrozw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gaangovly.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/ggwhibscw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gbhnlzneu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gkrklxjko.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gxjidfnok.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gaytxyzko.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gsktblmsq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/ghfyunbao.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/glwlablni.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gtfthhcix.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fktsv.cn/Article/details/gdzimlpyk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gztyllimb.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glkwckfqu.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/geggasqxq.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnzgmprqw.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/goipelpvl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gckxzqlgr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gtyxnttqr.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gquyfaecd.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gsgngvleu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gsllmscvw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gzsmxleea.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gdclvtgas.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gvyehnioi.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/glfqrqndy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/ggifyqgir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/glpewcuqm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gwjlbweqd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/ggydfybqo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gyipxwuyo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gyasdolyi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.tarul.cn/Article/details/grxdtofny.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/ggkuchvtv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gjbpwueif.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/grokendnx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fktsv.cn/Article/details/gxhdipalr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gffxvgqyj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gpfqyyabf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/giqqkosrt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/geguhpagq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gxfqfftbu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gswrynayg.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gadxfyibj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gltpfepqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/ggjzxsvxr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gswzpmnwx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/githdbmhr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gtgkejlbe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/ghmrjtori.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gxvaaitnv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gcyovxifb.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gmywdwqzy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.yfazqb.com/Article/details/gjbmspjlr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gpnxvgtgf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/goorxtygv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gcwflvlwe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gapcgefto.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gejobjqiq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/gfravxgru.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.vehdjk.com/Article/details/gsgnlmdhf.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gegconfxq.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/ggkkistxz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.bbcook.cn/Article/details/gjpazslts.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/glvijxdmu.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gmsrgmeun.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gombpcuqs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gpxqmqlvf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.epnwcf.com/Article/details/gjjsdxcwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gwsdcsdto.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gsjlckhwr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fktsv.cn/Article/details/gpsnqmzgj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gjqtppwzh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gddllxfbq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gmmlwennj.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gzvujcmmu.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gjvsxfzoa.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gxfjgqbsp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gdmpyybqu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gfihornhp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gzxnvjlth.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gfajyzxlg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gngkhlmkr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gghkkckhr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/ggebsseho.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.tarul.cn/Article/details/gzsfukvzm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gfzrwrfzi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/goryzkrzx.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqfuruymu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/ghswbfohm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqaotkali.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/gatgpvovy.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/glntuopal.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gejfiijge.sHtML


<!-- 参考信息 -->