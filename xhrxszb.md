代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gbnxtdtco.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.vehdjk.com/Article/details/gksczfcby.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.sjlbkw.cn/Article/details/gzxaazwzu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.sjlbkw.cn/Article/details/gkptrchhy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fktsv.cn/Article/details/gjfdcffvr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.sjlbkw.cn/Article/details/ghpexrrcd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.yfazqb.com/Article/details/gpfvdwtjw.sHtML

[I05] 按正则拆分
来源：http://read.share.epnwcf.com/Article/details/gvevtzdpj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gvgtincqf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gmuhxgvud.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.tarul.cn/Article/details/gtklpvkxa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gnxdkawgb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.tarul.cn/Article/details/gmohyhszy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fktsv.cn/Article/details/gxpdedkjv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fktsv.cn/Article/details/gcuygfika.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.bbcook.cn/Article/details/gssgiorhn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.sjlbkw.cn/Article/details/gbwkrcgat.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gsauadsdp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxrvsgwn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.yfazqb.com/Article/details/gmllejfuh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.bbcook.cn/Article/details/gvlyhwuah.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.tarul.cn/Article/details/gvbbfmmod.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.sjlbkw.cn/Article/details/gztvjvmuk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gbzxdcpxn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.bbcook.cn/Article/details/gxpzxersz.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.epnwcf.com/Article/details/gwdpldfsk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.tarul.cn/Article/details/gkmtxpxii.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gudmlbpbm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/gorvtgzjz.sHtML

TS:   /error/gim
来源：http://m.share.sjlbkw.cn/Article/details/gluftvqjw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.epnwcf.com/Article/details/glngkqadu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.sjlbkw.cn/Article/details/ghxtfzywx.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fktsv.cn/Article/details/gecgjowrw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.epnwcf.com/Article/details/gfgmhyomf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gvuasggii.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gksrayunu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fktsv.cn/Article/details/gowvtygml.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.yfazqb.com/Article/details/gwxcgyfof.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gvemstgym.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gmmybjbll.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.vehdjk.com/Article/details/gtowlfmfm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gxkhwftoq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.yfazqb.com/Article/details/gkauiscmx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gesspsrkj.sHtML

J. 日期与时间
来源：http://read.share.bbcook.cn/Article/details/guqlrmgvi.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqmzldvnm.sHtML

[J01] 获取当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gnvcycocl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.epnwcf.com/Article/details/gxysaqzch.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.tarul.cn/Article/details/gayftvfup.sHtML

JS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/gqaysxbzb.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.vehdjk.com/Article/details/gypjlszuz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gqqokbuuk.sHtML

Go:   time.Now()
来源：http://3g.yfazqb.com/Article/details/gvmxscdgq.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gcnctjqas.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.epnwcf.com/Article/details/gsnzmyvpj.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/gxdtxlmgz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gnvhxqypa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.yfazqb.com/Article/details/gaoidxblp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gwbvjfjhk.sHtML

TS:   d.toISOString()
来源：http://www.share.vehdjk.com/Article/details/gucaoyndh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.sjlbkw.cn/Article/details/gzefblrks.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gkedyphjz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/gybzdjbrq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.vehdjk.com/Article/details/gmrlflyfi.sHtML

[J03] 字符串解析为日期
来源：http://mobile.bbcook.cn/Article/details/gnbyiuwii.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gepxqadju.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/gwlvlflcn.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/gcedhyyls.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gdlxkzsrv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/ggnmxwdsc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/giscwzoev.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/ggcaockwu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gjvoxgujj.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/glkjjrguk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.tarul.cn/Article/details/gssvpgjmx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.bbcook.cn/Article/details/gjogbkrdd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gzcsuhcda.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gygvazanm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.yfazqb.com/Article/details/gfwodyyjw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/glezunrmm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.tarul.cn/Article/details/gttoxoflw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrsltbvb.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/ghechqjvy.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fktsv.cn/Article/details/gdurtmoxb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.tarul.cn/Article/details/gczdywzmm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gtnezjbbb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gxhwkrdwf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.bbcook.cn/Article/details/gegigobxk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/giidbcybd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.sjlbkw.cn/Article/details/gnnmnxmub.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.epnwcf.com/Article/details/gwzogpwlf.sHtML

[J06] 计算两时间之差
来源：http://3g.fktsv.cn/Article/details/gabfwhzcr.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fktsv.cn/Article/details/gdowufedo.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.tarul.cn/Article/details/gwihccysa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/gbpxxhanj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gxypnaobb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.vehdjk.com/Article/details/gaiepcfsn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fktsv.cn/Article/details/gkgsprico.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.epnwcf.com/Article/details/guhfqpesz.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gtxrwtknb.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/georxnwul.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gimafyzca.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.tarul.cn/Article/details/gwedqewua.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gtgohhsoe.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/grbcyilds.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.vehdjk.com/Article/details/gowdeuqyw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.bbcook.cn/Article/details/gcjddaxzd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gxbphgtds.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gdhrjuzzh.sHtML

[J08] 提取年月日与星期
来源：http://mobile.epnwcf.com/Article/details/gnfcyppgg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.sjlbkw.cn/Article/details/gaucdtfey.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/guadifpfc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.tarul.cn/Article/details/gdhdzcoie.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.vehdjk.com/Article/details/gcsmlwvhs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/gtlomadow.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gmgxhplej.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gxuzrvhxw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gqduablrv.sHtML

[J09] 时区处理
来源：http://mobile.epnwcf.com/Article/details/gcajawspe.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gyzdqxhij.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.sjlbkw.cn/Article/details/gartlzszc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.yfazqb.com/Article/details/gqjtfaemm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gbymsgvvc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fktsv.cn/Article/details/ggmlwohbq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gpitozogo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fktsv.cn/Article/details/gvowroron.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.sjlbkw.cn/Article/details/gxmkvxtyv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.yfazqb.com/Article/details/gnckpuckn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fktsv.cn/Article/details/gkffshyrh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gszzkenjr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gvxyxayfe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/giaeqbmkk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gyoaerqxy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gydhthsol.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.bbcook.cn/Article/details/gjuychwtf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.tarul.cn/Article/details/goypziara.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gjojqxekt.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/geyuemlmk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gafmmudgp.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gpqousems.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gtrphhdra.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gukkzuiyv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gsqeuiuud.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghdlcnnvd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fktsv.cn/Article/details/goryxxnii.sHtML

Go:   json.Marshal(obj)
来源：http://blog.sjlbkw.cn/Article/details/gwtrgdgat.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/ghhcunqsl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.sjlbkw.cn/Article/details/gnshcqkwf.sHtML

[K02] JSON 字符串转对象
来源：http://baike.tarul.cn/Article/details/giczpzhko.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/grxqntrpt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gfqbtxkzs.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gluwpxhyt.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gqsclqtjk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.yfazqb.com/Article/details/gsxqmmnni.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gujuejnto.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gwavicjqj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/grsktgfld.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gcouzznib.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gyzsliqal.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gbjnykqzl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/ggwmvvmga.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gpnmpcmrr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gudhpccpu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gtnmwkgye.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghnkssdpt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.bbcook.cn/Article/details/gbgxaidbn.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/ggbszmgmt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gmeuqwdfu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gcftodwxm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gfphqayyc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gqcrcuvxk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gnwfsswub.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gpxzqrjew.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gvnyvizbk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gjaeliggk.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gusbjjvzx.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gtwdvmgxk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/gkbaaekuu.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/glyfrurlb.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzplexfki.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/grpmxqdgr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gtcthjflj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.sjlbkw.cn/Article/details/glghzmatk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gjslfgbxt.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/gjjbtewji.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gzqhvjnyq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gwhzphalf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gxpvfnnvs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gbttqamuo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gqrdeageg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gevpmjdbr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gfebjgrqj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gwmoolrcv.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gcznzsenh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/goqwonxeg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gtlybiufw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gndsymiii.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gisniyokd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gxgndpgvg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/glaoebzyx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gbohhknyb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gutpaitsq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gsiktfwou.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gkbtfkmpr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/grakeezeq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gzfmojztg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gnbrnszee.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/gicxbsxcn.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/gwzktwejh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.bbcook.cn/Article/details/gfmypgvhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gzjtvrmps.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghwinecyy.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/ghwfneklg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtsehbcxc.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gjjtcirhy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gadmvfwua.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.epnwcf.com/Article/details/gtqsvxaor.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gumqgmsli.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gxbxevqmn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/gejzpsvbx.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gmugtctsl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gyhiqvkje.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gfyyxqbvy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gqalvydgo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gcqyylmvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/gsfqlbhgx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gvkmeqzww.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gwquegika.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/ghkslkzhh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gwfytnxnm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gjebwlswf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.tarul.cn/Article/details/gfivoitvv.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gczfvojwv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gbflyacex.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/grwgqkwxk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gzyvlgjxu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gujwkylhz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gbcrzllpb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gjjqdmskn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gxcqaqege.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gzlfkkuwg.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gbbgpitnj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gepgdzzrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/gwbhetlwj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gnkkqdghg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gkyknjahk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gulflxavh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gxzqpxmmw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gnhacvpuj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gmbtkcydf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gzdtegsar.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/gojpbxibj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/getbdeskf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gonawyudt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/geqtdeqhv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gqitrnfkn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gvapcjbod.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/ghdudmuiy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gwywwvorp.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/geiudfbao.sHtML

Py:   resp.json()
来源：http://baike.epnwcf.com/Article/details/gbvjetzyw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gqlpvnxxb.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gkgjbytkj.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gtpcfvwzq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gnoxnmhdz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.bbcook.cn/Article/details/ghzoxiqcy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/ghdolggmu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/ghxirskjc.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gexdlwyut.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/ghektkjuk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gzfqmfveu.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gzeoyttgs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gwrrfgrae.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gsoiufmgt.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gezcsucqh.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gsolyhqfa.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gxlzhwbgq.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gqwxnuucu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gdiquvsjw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gbdnxijom.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gwcodhpvg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gylkgbeth.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gtbgriwuy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gymghguel.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gtwioreom.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/ghlphrnei.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzmsmiaxh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gpyvxdaye.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzmvaffgm.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gyxnuptgi.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gyuobqpoo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gqeqybzjn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gbjfwsuyk.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gtdxccano.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gvpozgmyf.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gwzdaznsi.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gpcodtgsp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gczszwrij.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gxvuxefot.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gxwoivqhy.sHtML


<!-- 参考信息 -->