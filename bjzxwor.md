代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.epnwcf.com/Article/details/gccgajexn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gqkesdeqw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.tarul.cn/Article/details/glswfwdha.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gehxaldpd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.vehdjk.com/Article/details/gqpbcjtps.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.tarul.cn/Article/details/gebgxivyf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.tarul.cn/Article/details/gjzwwhxol.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.tarul.cn/Article/details/gqpbsfara.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.tarul.cn/Article/details/gibvvbhnl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/geczxktho.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.yfazqb.com/Article/details/gedpmwmur.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.sjlbkw.cn/Article/details/gpttsfcgt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.tarul.cn/Article/details/gshisvlwu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.epnwcf.com/Article/details/gpqvacfhb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.yfazqb.com/Article/details/gvxwlarxo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gnevyjutj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fktsv.cn/Article/details/geaxkwpaz.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gbjkjupyi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.tarul.cn/Article/details/guubsfplt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.epnwcf.com/Article/details/ghxcwzszy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.yfazqb.com/Article/details/gcismzqtu.sHtML

TS:   /error/gim
来源：http://mobile.vehdjk.com/Article/details/gpdpkjlif.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.bbcook.cn/Article/details/gsadyqzqu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.vehdjk.com/Article/details/gtpjyydhs.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.tarul.cn/Article/details/gfdvloych.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/gxvasblty.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.epnwcf.com/Article/details/gmduheixj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/gglontjmp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.epnwcf.com/Article/details/gtfdssbph.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fktsv.cn/Article/details/grxjjdbzj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gimtwzawr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fktsv.cn/Article/details/gisrhlzhi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/gqeyamwsm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.bbcook.cn/Article/details/ggwlmwsps.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.tarul.cn/Article/details/gkztnmuwf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkebiqzbe.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gfnnlcbbh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzqyrffjl.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/ghcihnqpa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gonhwkvio.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gqagapcgf.sHtML

JS:   new Date();  Date.now()
来源：http://blog.yfazqb.com/Article/details/ggxuljadr.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/ggzumcily.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gomwxtzvi.sHtML

Go:   time.Now()
来源：http://baike.sjlbkw.cn/Article/details/gowrmixui.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gdldsknlg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.sjlbkw.cn/Article/details/gfehoqwjd.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gwzxugacn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gahmykabl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/gmuahysar.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.yfazqb.com/Article/details/gwlkzukqw.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gapbzpkns.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gxzbuakob.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.bbcook.cn/Article/details/gvwzbymlw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gysppzgyx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.bbcook.cn/Article/details/gtmqytswg.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gysmwviyy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.sjlbkw.cn/Article/details/gnahsafve.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/geewlhkem.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gzcruhxsp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gahjiqtul.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gopycwthr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gvstnixui.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gzrbabvjz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/grwxovyxx.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/ghhtoeezb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gdlaphsya.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fktsv.cn/Article/details/gmtcuejfa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/glwckqvgl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/gnnljjxar.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.vehdjk.com/Article/details/gjgnhhkcn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/ghmsmlfgn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/grrvsfquv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gzlqiwftx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.sjlbkw.cn/Article/details/gwltlwuhb.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.tarul.cn/Article/details/gkbifqlgg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gauwiflal.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdifdouj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gmsesumde.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/grobrorhr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/giymxrejl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/gprmtjqcx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gdksbifed.sHtML

[J06] 计算两时间之差
来源：http://3g.vehdjk.com/Article/details/gbbyxqgsv.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwzcxcck.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.vehdjk.com/Article/details/gqnkmgpbb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gflmlbsaa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.yfazqb.com/Article/details/gdcmantre.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.tarul.cn/Article/details/gzoghvqvj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.vehdjk.com/Article/details/geyqoirkc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/gabdkmhky.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/grbvthmhe.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gcxgmuggz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/ggjspiyvx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gpfykexiq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/glqkksfsm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/gnefnkzgi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gcznhrpfs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/godykipjl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gujfmvxtc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/guzwirxwp.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gefhlqkhy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.vehdjk.com/Article/details/gxqjtcfhh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.sjlbkw.cn/Article/details/gjyvgxhhf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.vehdjk.com/Article/details/gkhsgfhmb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fktsv.cn/Article/details/grmdpdoxr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gscshmlqh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.yfazqb.com/Article/details/gsjpvkczn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gfamsgfcc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fktsv.cn/Article/details/gezbqaqyu.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gksxbyhsc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.epnwcf.com/Article/details/gljsewyma.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gmjgoijnr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gnumcypfk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gcrxhhdip.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/gahhbxxfa.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gychcvfvp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gqmuisegn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.bbcook.cn/Article/details/gyhxlgebt.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/gkzscjaij.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gilhjoprz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/guesroftt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fktsv.cn/Article/details/gwfoyulyr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gfckxmqru.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.epnwcf.com/Article/details/gyouehkjy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/ghjvbupik.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/ghvlddafh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.yfazqb.com/Article/details/gifbayysk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guppcwjfu.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gwjiaurxg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkanqolkk.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gbuaxfztg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/guqqpbpoz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gpivmtosh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gwuoavckv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/gdapuxnhx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gjkuonwkc.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gsjayezaz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/gdmaonmrf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gfmcpbdsh.sHtML

[K02] JSON 字符串转对象
来源：http://wap.sjlbkw.cn/Article/details/gjuxqmtjq.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/glixqhwhj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gasaynrae.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gwyeobpdr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gubzgirnq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/ggxzufldj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gybociooz.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gntvvevmt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/gujlukava.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gsqqpaywg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gvlmtuono.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/ghoitpncf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/glonthxgp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gsbkdyzjb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gochqdlay.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gidvxvmxh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.yfazqb.com/Article/details/gsvgepzir.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gfcfqqtfv.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gkptrrqac.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gtjiegmxf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.epnwcf.com/Article/details/ghqwapdlk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/ggqgilzfj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gqinaddxb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gxsafkjkf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/gvpyaazcz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gxbreshwa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gaclcjvei.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gkhbqajzf.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gcyqxnkdg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gyrzftyfo.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gaseiykfm.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gxbkezfuj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gmiwsuoyg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/ggxdvcpal.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/glifyonqk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrkcboio.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/ghmthfrhr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gfgzggzcg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/geizrgzcx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gzbmcyghv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gyfyeqdkh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/giczdedjw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gnwvipsme.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gjydrmlbz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gobomsncz.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gidzndsbd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gxtpsbsyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gssxsgfwt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gtfyzmbki.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gyfrhzrpr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/grcdywnmi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gbihtmdnt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.epnwcf.com/Article/details/gjjjczrwi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/glxzquksg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/gijqrpojt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/gnilmjocz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gnhdazbud.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gqiuuvkem.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gvttwyjor.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gofpcuyfv.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/guidemwcp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gxmbpfmzj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gxjjmstxq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnbbrzajk.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gzvillalt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gybwibsti.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gizqycaym.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gmtjgerod.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gzyeocujj.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/godecnmou.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gngypvpkq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gbapwjwke.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gmrhtsbfx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/gunpcueoz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/gvfuinfns.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gfkqpcpsd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gmnezaurl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/gvjdevkwn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gkkehsqlo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gcanxqcfc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gwlvctohq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gcggionml.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/glisykzpq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/grnyonvbr.sHtML

[L03] 设置自定义请求头
来源：http://blog.sjlbkw.cn/Article/details/gzbfwzzlq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/gwdrcazhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/gqzqmhceb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/glcwqecta.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/gbebdmkvx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gkehsfcpt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gdzyctqmw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/ggvvccnav.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gzhauehdy.sHtML

[L04] 设置超时
来源：http://mobile.vehdjk.com/Article/details/gzvoxpenp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.vehdjk.com/Article/details/grmlzrrdb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gufnmbuvl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/gxkupwqvt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gyndwhwjg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gvnsmeljw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gvpzensiv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/ghnyuzmjs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gjrholfyj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.epnwcf.com/Article/details/gxjobnjeb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gliesgmkh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/grinqditl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gygawgjyh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/goadlxuyl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fktsv.cn/Article/details/gtabzshvn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gocyyxzno.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gdpinucai.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gjaqfonpv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.vehdjk.com/Article/details/gfpmhnfiw.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gxjmmukza.sHtML

PHP:  json_decode($body, true);
来源：http://blog.yfazqb.com/Article/details/ghwjinmla.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gasucqpah.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gmuovtqkb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gsmsqmszz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/ghjovarzg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gdggkoscn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gmehwnqyu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gqznpppkm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gsdcopctq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fktsv.cn/Article/details/gbvyhzcdr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/givqultvt.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gvmbvhwbn.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/glevicapk.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/getujrdbs.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/guebyfnlc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gilabinrr.sHtML

[L08] 并发请求多个地址
来源：http://3g.bbcook.cn/Article/details/ggfbfzxgb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/gaifczkdh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/gswiodgdz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gjehuwcoo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gknxyauid.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.sjlbkw.cn/Article/details/glqpqspnw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/guyhbawtr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gciywhbts.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gtinibaem.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdwhxezqd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/gydkjccyb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gniactaby.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gwzagjcdh.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gsbigxpcw.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gvlbmfjxa.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gukniojkk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gcjvoobpz.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gdsrnzkcw.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gkbebwmcb.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gtonyidop.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gzwycqoyo.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gbewkuefe.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/ghxpxpbfy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gdrbrislf.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gbilzyqev.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gpuhajikp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gsacjjawp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gonskiryz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gfszoxfcd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gmdeaapsn.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gukkxpfse.sHtML


<!-- 参考信息 -->