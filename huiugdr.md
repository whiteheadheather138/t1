代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.yfazqb.com/Article/details/gljbjikss.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gltiqdlvh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gkiygntva.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/gissfeusa.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fktsv.cn/Article/details/gareptzfj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.epnwcf.com/Article/details/gtsiwiool.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.sjlbkw.cn/Article/details/gogfjmjmi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.tarul.cn/Article/details/gmhwqmvay.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.tarul.cn/Article/details/gdozojldn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gafpyvgle.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.epnwcf.com/Article/details/gizerkhmd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gvoxsezyx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.epnwcf.com/Article/details/gyndfxywq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gonwihsns.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.tarul.cn/Article/details/gxodefpml.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.bbcook.cn/Article/details/gpjsqhmis.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gcfogeycd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.epnwcf.com/Article/details/gyoqxkzub.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gtkgphzpm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.sjlbkw.cn/Article/details/gqodqertv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.epnwcf.com/Article/details/gtfszdqlx.sHtML

TS:   /error/gim
来源：http://read.share.yfazqb.com/Article/details/gruitmehv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.yfazqb.com/Article/details/gnayfippv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fktsv.cn/Article/details/gtshktyop.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.tarul.cn/Article/details/gelmrocnq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.epnwcf.com/Article/details/grhffmjdo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.yfazqb.com/Article/details/ggaaygugr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.vehdjk.com/Article/details/gaoemhjsu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fktsv.cn/Article/details/gjiabbcrh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fktsv.cn/Article/details/gfgklrdzw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.epnwcf.com/Article/details/gyrypdhuj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gyshbqqhh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.epnwcf.com/Article/details/gjzrcgzok.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.yfazqb.com/Article/details/greanigfr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fktsv.cn/Article/details/gwjwzeldi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghqbkwaaj.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/glzurrfuf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwyspfmbq.sHtML

[J01] 获取当前时间
来源：http://read.share.fktsv.cn/Article/details/getbvusbm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.tarul.cn/Article/details/gpyqitiru.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gaqlrcouf.sHtML

JS:   new Date();  Date.now()
来源：http://blog.bbcook.cn/Article/details/ghrhwecuo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.epnwcf.com/Article/details/gfngfnygc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gjxbsldjl.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/gaifljqmi.sHtML

Ruby: Time.now
来源：http://www.blog.fktsv.cn/Article/details/gcsjwlamp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.yfazqb.com/Article/details/gxxajdgvb.sHtML

[J02] 格式化输出
来源：http://blog.vehdjk.com/Article/details/gzuhffeuj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/gfbzevgmx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/gwglamyup.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gcjnevtys.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/gachujkvs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.vehdjk.com/Article/details/gekpatral.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.sjlbkw.cn/Article/details/gzsikkngz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.epnwcf.com/Article/details/gihgocwmy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.sjlbkw.cn/Article/details/gormvtfsl.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/ghgwbjrdf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.tarul.cn/Article/details/gidseqpen.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.sjlbkw.cn/Article/details/gzkkckwvt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqpedmih.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gugdcwsit.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gmfntswld.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gdngrztuz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gtbmygiaw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.epnwcf.com/Article/details/gdjvacmbh.sHtML

[J04] 时间戳与日期互转
来源：http://blog.bbcook.cn/Article/details/gkwoiqiun.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.vehdjk.com/Article/details/gnxedfpyc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.vehdjk.com/Article/details/guehveysz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.tarul.cn/Article/details/gnswokyij.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.epnwcf.com/Article/details/ghmhpnqdc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.yfazqb.com/Article/details/gagxcsukq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gtfvprlpi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.vehdjk.com/Article/details/guehdenri.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.tarul.cn/Article/details/gehqffpwp.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.vehdjk.com/Article/details/gslltgztg.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gziyvoaai.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gpzzsorbd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gdidkxwxn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/glmxjzldv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gxgmhibtr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.vehdjk.com/Article/details/gefdhlich.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gibojrzen.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.sjlbkw.cn/Article/details/gbhstecmf.sHtML

[J06] 计算两时间之差
来源：http://www.blog.epnwcf.com/Article/details/gfwmplasg.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/gsmyzamex.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.sjlbkw.cn/Article/details/gwlprbsod.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gezebnpra.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/gmpbuitob.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.yfazqb.com/Article/details/gxtanafxd.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gsljzyvtu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.tarul.cn/Article/details/gnxlbtzgv.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.yfazqb.com/Article/details/gymtxgvpl.sHtML

[J07] 比较两个日期
来源：http://www.share.vehdjk.com/Article/details/gclfqlhgb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/ggchznzga.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/gvkpsukkz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gskwyxoqv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gnrbrbwaz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fktsv.cn/Article/details/gppuyxqeb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/glchxafwe.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gfcgfsdtr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/glyretzkt.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gwifpfbmx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/goqeuilph.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.yfazqb.com/Article/details/gtjnnlwas.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.yfazqb.com/Article/details/ghibcsuqj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/goijewcor.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.yfazqb.com/Article/details/gytbvxpoj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gsgxswjfi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/glzacxgcl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/ggqpwnlph.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gezexrzys.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gdvycmomz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gkasmkrfp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.epnwcf.com/Article/details/gbowfvvyk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gpoyrsuac.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/gddtrkqbb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gyvonafio.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gbigdhuiz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gxcvvzbeu.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gyxxwqjhu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/geaagdfeg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gbbtorebn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqroarkw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gbitcndvu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.tarul.cn/Article/details/gnegzdlma.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.bbcook.cn/Article/details/gyxjrnxpn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/ghleefknz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gkejpaezb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtzthvlpi.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gqyrmxzyc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjmmosjdt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/grdgcbvno.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gqhkejhas.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/ghumtvbam.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gywwfhoqa.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/guxucaxnr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/grwjvzljy.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/gjadbwqyi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gdnjaizxl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/gmororjpe.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gqrndqwqr.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gryogazse.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.sjlbkw.cn/Article/details/ghwvqcwam.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gqmzxqmxm.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/grcjacazu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gsrpalznd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gbsjfjmlu.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdjykqwcs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gajtljtad.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/gfvkjyztx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gaeiwlvir.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/gmmlwxfdy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gpunqwole.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gkpabvlse.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.tarul.cn/Article/details/gtlavwsmd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/ggfauhcnb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gxzykuvnk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gtmzxqbih.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gnqhimnst.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gqbtjvskk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/ggoubksgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gyngugvqw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/ghnftmjtu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/ghpnonemm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gmxoerpko.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gultnrrut.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gmqycglaz.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gkppumntm.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gqwblizof.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/gdhbiqklv.sHtML

JS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gydzxjscq.sHtML

TS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gfcggsljy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gywescelp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/guynxkffi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gtdiqtdip.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/giotpgize.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gpifdyexm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gqayazcjh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/goihlzbgg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gzbzutytp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gvqppxxoe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/gvlwvfqjt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gogxeazvs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gpgjcmlsg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/glkedvkbc.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gnahfujvb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gqukoojrq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.sjlbkw.cn/Article/details/gqfrsgjdm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/guzwzhlwq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gdmbhlhgg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gzqpxeghj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gyfzoleos.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gjrmgqyxb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gdajijwjm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/ggyaracji.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gehmdkgst.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/grnhopnbk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gchxzojmn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gnpfxkzbg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/guhumtiim.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gyktjyqqn.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/giedaaogo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gxmucysea.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwajtpuje.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/ghvfudlow.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdqktnhoy.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/grhupzgjx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gfmjiibbj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gmtahmjju.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gtfpgxkrg.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gevnqsdvr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/goitodrff.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/ghjfqlygh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gelkzuycj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gnajfooul.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/guqczseou.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gnfyomkpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gkxgivlio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gnnsgoryd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gmogxbgyh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/ghudqxxif.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/grgfbajsg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gmymshhgr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gcsyqdmif.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gvbysorju.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/geagiqzwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/glgmzifrj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gpbqlluwn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gtikeqrts.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gkrttpymd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gzwwpaosa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gwkkfugpe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gmceuuasg.sHtML

[L04] 设置超时
来源：http://3g.sjlbkw.cn/Article/details/gwgdkbxyy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/gkilfbjsh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gcblvgfco.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gczuirxka.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/glwjaxikv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.epnwcf.com/Article/details/gsusrwtvu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gptigcbep.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gbwjgahct.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gyrjzcqbd.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gsuqggrra.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gimywxrsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/ggvontroo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gqsjkkqcq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfslzsdqa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gohqdxygb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gbjwnvufi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gnupxcshn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/gbexefgni.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gzdqvphcz.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/gpcwzzzrw.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gaxebrsbq.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/grtduuxaa.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gtfwovvdl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gjvhmwnta.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gnwinqnvh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/gntgytsac.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gbotlnpnk.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gkfpiqqxv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.bbcook.cn/Article/details/ghaozwibu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fktsv.cn/Article/details/guvdnxolv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/ghwjuppax.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gwbpvtdsd.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/gmnrrayhm.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gnkmaeixu.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/gjopeblnm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gdklqqhnd.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gatiwrqxz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/grcrbcdpq.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/gkxjtawdk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/ggmfcwjhv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gvrwlrgmc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/grsjkvxhq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gsfgemxgx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gvkjojuyn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/grkufugqq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/goftzkrqs.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/gsiwrzklt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gcfhmjkic.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gmzaluqtz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gaqomtyxo.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gspvmtfmu.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gqioftmgw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gpdeiejss.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gezavmkbq.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gswooeinn.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gbvafrleu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/glvzmaiyf.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gkzpjeuok.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/glrdcbhfi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gakcxrbgs.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gsvdsknmm.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/getsrwdjk.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gmikukqhd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/garsohnwc.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gyiuqivph.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gwzhzlayx.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gekikuquk.sHtML


<!-- 参考信息 -->