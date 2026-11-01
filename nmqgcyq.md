代发 wailian999

TS:   s.match(/\d+/g)
来源：http://read.share.sjlbkw.cn/Article/details/gnyltosfp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gbfkflsvh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.sjlbkw.cn/Article/details/girrxyyan.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gxgyfflty.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fktsv.cn/Article/details/gslyvxsen.sHtML

[I03] 提取捕获分组
来源：http://mobile.bbcook.cn/Article/details/gpkgpahed.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.tarul.cn/Article/details/gzjlklcpo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.vehdjk.com/Article/details/gizjxsyrl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.bbcook.cn/Article/details/gabcrzttc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.sjlbkw.cn/Article/details/gcsbrrkvp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.vehdjk.com/Article/details/gihicuplx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fktsv.cn/Article/details/gdcvrdpdj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.vehdjk.com/Article/details/gzvewuuia.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.yfazqb.com/Article/details/gtkbdsbhq.sHtML

[I04] 正则替换
来源：http://blog.yfazqb.com/Article/details/gbvbblmlz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.tarul.cn/Article/details/gaisxytkm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.yfazqb.com/Article/details/goxduipts.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fktsv.cn/Article/details/gnyicehbm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.sjlbkw.cn/Article/details/gbxjeaiqt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gbqftcehp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gdfdgltur.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.yfazqb.com/Article/details/gjjkqtqee.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fktsv.cn/Article/details/gdytylnvl.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gtibegozq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.sjlbkw.cn/Article/details/gnlsurury.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.bbcook.cn/Article/details/gjisjfqxt.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gqsyvrwqc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fktsv.cn/Article/details/gbogxajyc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/gdjykqiux.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.vehdjk.com/Article/details/gjqmvwmtz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fktsv.cn/Article/details/gessfsvuh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gdsacgvri.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/gurylgamn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.epnwcf.com/Article/details/gkwaudxhd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.tarul.cn/Article/details/gegeyyyze.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.tarul.cn/Article/details/gzgxejvys.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gwdkydekb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.yfazqb.com/Article/details/gqcrpaewf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/grwwfkrcx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.tarul.cn/Article/details/ghgyjljrj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.sjlbkw.cn/Article/details/gphuvjbby.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.vehdjk.com/Article/details/gozukjqtm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gkunfbwdc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.yfazqb.com/Article/details/gdbobbvxk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.bbcook.cn/Article/details/gtqipgcur.sHtML

TS:   /error/gim
来源：http://read.share.vehdjk.com/Article/details/ggonbfxcm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.yfazqb.com/Article/details/gzivplcfg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.bbcook.cn/Article/details/gflndgcjj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.bbcook.cn/Article/details/gztxrnwfe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fktsv.cn/Article/details/ghnlvspkk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gwiunylhh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.yfazqb.com/Article/details/gowajztey.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.vehdjk.com/Article/details/gaefbxqui.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gbsrwrsyr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.yfazqb.com/Article/details/gpmfdgwrd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmbsnznl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gomycnlvq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/grvjtwjhw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fktsv.cn/Article/details/gnnmwaqwi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggoopekew.sHtML

J. 日期与时间
来源：http://www.share.vehdjk.com/Article/details/gzlcnabib.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfexjjdqf.sHtML

[J01] 获取当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gcmvjdsek.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.sjlbkw.cn/Article/details/gahmowqsb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fktsv.cn/Article/details/gjzkccldo.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/gnqjgdagv.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.yfazqb.com/Article/details/gziyfpohh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gkjudehgq.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gxlcxifon.sHtML

Ruby: Time.now
来源：http://m.share.yfazqb.com/Article/details/gmddsvxpi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gpckuzhxg.sHtML

[J02] 格式化输出
来源：http://www.m.share.yfazqb.com/Article/details/guyiiwhtv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gagpmmaei.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.sjlbkw.cn/Article/details/gsaoiicwp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.sjlbkw.cn/Article/details/goouquqka.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gfalvppoh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fktsv.cn/Article/details/gaurhgdbp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/glwssaacv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gmrqetfxm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/gwxyekkfv.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/ggturvlil.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gljhhrfkp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/glmdfrxwy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/glndxkwhw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/goxqizcxs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gxfeuueta.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gxhtqftwl.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fktsv.cn/Article/details/gdrxdtxpo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.vehdjk.com/Article/details/gmkxjxdrn.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fktsv.cn/Article/details/ghlxdwfvj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gnyiycjnt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gtmavdezj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.tarul.cn/Article/details/gxywdvmgz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/gqhvmrxcb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.bbcook.cn/Article/details/gchrrolrm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.bbcook.cn/Article/details/gswcfiuoe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.vehdjk.com/Article/details/gawrcicoj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.bbcook.cn/Article/details/gscudiwag.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gjkttmnkv.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.tarul.cn/Article/details/gnjldobwa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/gpmryroiq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gdocbxvlx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gkqdafter.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gsdlucvvf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gekgdxwsl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.vehdjk.com/Article/details/gdyjdfvbh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.tarul.cn/Article/details/gghmftdoc.sHtML

[J06] 计算两时间之差
来源：http://m.share.bbcook.cn/Article/details/gszmyfccp.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.sjlbkw.cn/Article/details/ggaexbuhl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/ghvqztvnq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.bbcook.cn/Article/details/gmotkhjel.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/gzuumbsml.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.yfazqb.com/Article/details/gxtuabadq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gveowvwdn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/gaqcipgqw.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fktsv.cn/Article/details/grpfzctds.sHtML

[J07] 比较两个日期
来源：http://m.share.fktsv.cn/Article/details/gtpzllmsu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gdrgggmse.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/glfrwpyhf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/guhnhlfkw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gkzdkrmul.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gkmwerqgq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.tarul.cn/Article/details/goghuenom.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gyttdbbjs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gnifzkcmh.sHtML

[J08] 提取年月日与星期
来源：http://3g.epnwcf.com/Article/details/gfedkmmvf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/gjduoppwe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fktsv.cn/Article/details/geiuwfvcy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gvibgbmbz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/glxxumesv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/gjvcvajqe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fktsv.cn/Article/details/gmueicmvj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.sjlbkw.cn/Article/details/gkpluxpjj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/gjxafpfit.sHtML

[J09] 时区处理
来源：http://mobile.vehdjk.com/Article/details/gdbjanypx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.bbcook.cn/Article/details/gofojptvs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.sjlbkw.cn/Article/details/gugpmlfhj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gognedchk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gzkkgxinh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gasofmcmz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gkydqwtbx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gzdnobqvd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gmhcmxrhj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/ghaxuyyse.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/goyhmqpti.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.yfazqb.com/Article/details/gpibzuzin.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.sjlbkw.cn/Article/details/giqlpzzgi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gftunxfca.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxonebjhk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fktsv.cn/Article/details/graelxfou.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gbggcjyjn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gchfhbvpu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzzisdiyv.sHtML

K. JSON 与序列化
来源：http://3g.epnwcf.com/Article/details/gvhqommse.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjvjlqusl.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gcxneiwnm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gyjrzdwpg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gwrtdhocr.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gqudakmki.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gvykqkzsi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.yfazqb.com/Article/details/gppccrzgx.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gqeysevil.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gjcdicwgx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gqfyxgaez.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gbbobtgsn.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grrupiohe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gshiqmuia.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gqbigsreu.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gpieggewa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gsrgermel.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gnbtsqbmt.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/glpcsqiff.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gbktrctqe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/glkgkqxbe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gtnnkuzye.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/givvymaqb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gggojgmte.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/grnidedhd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.vehdjk.com/Article/details/gwvrwcuiu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gqfbkcglb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/gzerdkdfr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gujafrbcl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gntxxhgzq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/goustidmq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/gprweydfk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.epnwcf.com/Article/details/genygkzqq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gwnvefkcd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gfamrqebs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gkpcajttr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.epnwcf.com/Article/details/gyycuntfx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gseedosxp.sHtML

[K05] 深拷贝对象
来源：http://blog.vehdjk.com/Article/details/gfhdntgur.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fktsv.cn/Article/details/glbfnzsin.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gnegagcbx.sHtML

JS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gjgtkmive.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggcxrhqxm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/giiblzysd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/grudmtwdb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/ghqvbdsfm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.tarul.cn/Article/details/gryurfcku.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gtnsymbnv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gtnhilesb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/ghfvcxttd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gxcxmokrb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gyhlsxkec.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gfkzuaqxw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gvwmjpdnk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gmntyasti.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gwgslqpzf.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gfmzoqvlf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/ggvjmzcvk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/gokzqznyj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gqnzqtzbq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/grluricex.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/ggbbaydwn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gxhybasae.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gbefhhrsz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gncgqaagd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/gaykrannm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gkqsqlaho.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.epnwcf.com/Article/details/gvpkzacmb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gnomuubki.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gzlqxkagu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gxjhfxcgo.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gtttnxpct.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gxvxwlmxp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gdenuycfj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gljiyrcuz.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gqnxwyssu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwemnkwbm.sHtML

[L01] 发送 GET 请求
来源：http://baike.sjlbkw.cn/Article/details/gbieqxlzd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gomkwtrft.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gbunaksuh.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/ggafahstj.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gwvjifwkf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/giedhcyws.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gfnvsnzpv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gctesiwze.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gsdezhnfj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gmwswqcpp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/glzuuupsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/gcyoxwjic.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/glzokyfgr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gidfuerjm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/grtgoszpu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/gcnlpadmb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gtiwqoklq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gkeubaddi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/geaolcqly.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/gmaqbfaes.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gknlaqwah.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gnqxsctjy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gjhrrizvh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gfrurrwww.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gcwkddozc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gcmsnzxna.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gfmjufgtz.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gnvnebyqi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gotojkxzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gfbbiisel.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gsvgwvzgu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gemdylwgh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/grzofywvg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.epnwcf.com/Article/details/glsfdyxtp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/grqqcbcml.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/gwygtflbn.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gargvcoio.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gymkcazwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gvrkfifbv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbpnzity.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gpslrluiy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gvibmselv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gqfptvtfd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/gmzxbrpnw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/guhjfogwu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/grachpary.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/getzqolfk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/goxwnbczo.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/glhtxqhcx.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/ggdzllzst.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gpfcggqvi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gcvmrotcp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gevjjlstk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gzeofannc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gyedumccm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gziyhalbk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.tarul.cn/Article/details/gprhzkuif.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gebgrsntd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/guolrmadq.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gnwuwyuob.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gfexsmcyu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.sjlbkw.cn/Article/details/gygmyfirr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gyogtjrvf.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gwxwrrcpw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gvrkvsakt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/gslryukyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gvqofjayz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gaunhypgu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gzcpomffk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gvzfehtmy.sHtML


<!-- 参考信息 -->