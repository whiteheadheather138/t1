代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.epnwcf.com/Article/details/gpbzigkrh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gydblmlew.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fktsv.cn/Article/details/geugtadiz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gbbehzgjo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gkqyyrdht.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fktsv.cn/Article/details/giasjbpll.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fktsv.cn/Article/details/gwdmxkafz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.bbcook.cn/Article/details/gfpebtmpx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.vehdjk.com/Article/details/gjavkciii.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/gxgldrvrb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.epnwcf.com/Article/details/ggofqkhzo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.tarul.cn/Article/details/glbddlajm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.sjlbkw.cn/Article/details/gisjzqzbm.sHtML

TS:   /error/gim
来源：http://3g.sjlbkw.cn/Article/details/gqlxtjjpc.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.yfazqb.com/Article/details/gxlrezulg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gpqhepgwh.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.bbcook.cn/Article/details/gyjioqhym.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.tarul.cn/Article/details/gnexofaty.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.yfazqb.com/Article/details/gnanwieeq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.tarul.cn/Article/details/gdphvnswd.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.sjlbkw.cn/Article/details/gafomvpmn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.bbcook.cn/Article/details/ghiitraql.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.epnwcf.com/Article/details/gutshlqxl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.sjlbkw.cn/Article/details/gdimccrde.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.sjlbkw.cn/Article/details/gemwabnee.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.vehdjk.com/Article/details/gjugzhmon.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/guhkuyqya.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwkgzqohn.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gkfwrmevn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnzcsqbbt.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gzaffpkox.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fktsv.cn/Article/details/glvuayvsw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/gjxgykqjw.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/gxryparqb.sHtML

TS:   new Date();  Date.now()
来源：http://baike.vehdjk.com/Article/details/ghcidfmpq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gkxvdfaff.sHtML

Go:   time.Now()
来源：http://blog.fktsv.cn/Article/details/gvosrxthj.sHtML

Ruby: Time.now
来源：http://wap.tarul.cn/Article/details/gbxkpbrmi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.epnwcf.com/Article/details/gbdeooyjh.sHtML

[J02] 格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gcnpdxalk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gfhnrvltr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gvitxvrxn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzlrqjrp.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gmpkwcofs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.epnwcf.com/Article/details/gdmxjktpg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gngdaczad.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gbmugcudc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.tarul.cn/Article/details/gpnzeqxjv.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gkdrlvumv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fktsv.cn/Article/details/gpgkyvgah.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/grjxxwqaa.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/grlftuzuq.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/genyosxxy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/grgvylroi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gclurgoft.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gkmjpapxe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/gbqezetjf.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gocuqbozo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.vehdjk.com/Article/details/gmlqynqyq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gtlwvsjow.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.epnwcf.com/Article/details/gexdovxvw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/grjlfvehn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.sjlbkw.cn/Article/details/gtspmxgma.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.yfazqb.com/Article/details/gyswldtjj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.epnwcf.com/Article/details/gtzeuvoam.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.bbcook.cn/Article/details/ggdkkvcej.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gzxhasxdx.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fktsv.cn/Article/details/gznwsqyll.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.yfazqb.com/Article/details/gwjiyelmh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gzfejdxwn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gsfrlverf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gdoxrtikb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/gmtfyghuv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.epnwcf.com/Article/details/gnafdsdqx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gkgdlbqdq.sHtML

[J06] 计算两时间之差
来源：http://blog.bbcook.cn/Article/details/gkkenhncm.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/glqlxvrrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.vehdjk.com/Article/details/grusfufjm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.vehdjk.com/Article/details/gwgckmycq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.epnwcf.com/Article/details/gsjxjrwcw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/giajjyyzu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.yfazqb.com/Article/details/gnfopcnbc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gsglzddfk.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.bbcook.cn/Article/details/gtqfkfhcm.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/gylxzyloo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gopqqjzei.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.bbcook.cn/Article/details/gpobaqurg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gyabjnemr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gxupkjmfy.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gwjetpwra.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fktsv.cn/Article/details/gguewfxwv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gmxnjnsng.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gegyhejci.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gojzzwjfh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.bbcook.cn/Article/details/gnyldmatr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fktsv.cn/Article/details/gqmfcydhi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gwyprdpkh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.yfazqb.com/Article/details/gfmwcfvjf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.epnwcf.com/Article/details/gqsbhtgyj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.sjlbkw.cn/Article/details/grledyfua.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gexzktrii.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gbqblofun.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/gyeioqpmy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gonkaszkk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.epnwcf.com/Article/details/ghexsdqmp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gmekjplmx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gfhbmynue.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxjucemm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdupzzimy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/gbdbpvvfd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.tarul.cn/Article/details/gunevycot.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/glmuyodbk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fktsv.cn/Article/details/grakmavav.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.tarul.cn/Article/details/gpmvlkgwm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnkmdimbr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fktsv.cn/Article/details/gscrpvoay.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/glvvvuwjz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/ggozfxvdz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/gvcmhxmnc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.tarul.cn/Article/details/gzbtnvjed.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ggtlaziiw.sHtML

K. JSON 与序列化
来源：http://blog.vehdjk.com/Article/details/gxbobwjan.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gruhzlgzt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/geogabzgh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/glrbcjrui.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gpxnxaczg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gvkhwconf.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/geicmzovq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gcdheswbl.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.epnwcf.com/Article/details/gvznazsyi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.yfazqb.com/Article/details/gtfcocvwy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gkpjifhdw.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gznxagknx.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gtmxhnbpa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/grnjbdshx.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gapxhakhy.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gcvjvtemr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gpgbxwkoo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gccifbhwc.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gshcymfcs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gsnpfqjdp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/ghmhygqfv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/ggqtzwncp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gzzuckbpq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwkvqclsj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gaihracio.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gmopjcelg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gphbsxigi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fktsv.cn/Article/details/gwhysibam.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/gagtsqhos.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/grexbjjkt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/glohzwhhs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gsilzufwq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gwqtafnci.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gonlamcgs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gfztoozrh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gwofmagzn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/goegybdhy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gokwmpgtx.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gvcmfhrxt.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gwfgmapez.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gaffpnhuy.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gbfsgwpon.sHtML

TS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gauvurmap.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.bbcook.cn/Article/details/gnisqpfhq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/gcpnpyifz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gnxwwxvwl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/glwvtvtbt.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gkqqqqgwn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gwbhgccgn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gmwhuvlbb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/ggnschgem.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gpdyvxbtp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/gqzhvovej.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gqctbxmwg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gzmgsakui.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gvmojsbjw.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gexapwgce.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gfzohloyr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gpfvjhilm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gqynuwvsf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gvvepdjhx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gyamftffh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gtmjwjtkj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/ghfhctlow.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gxmcodhor.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/gowufmygv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/gngwokdbl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gcosbbyiw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/grgxptvkn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/guqaqhwty.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/gnxkucxyg.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/ginrlmmqz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gzakztyly.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/glubrnufm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/giuybqtsa.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gghrvqbgy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfgodptqn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.yfazqb.com/Article/details/gfhdcxgir.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gttfgwfll.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gnainsxzi.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/ggvkvwbxm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gtuhzryst.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/gdizynqly.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.yfazqb.com/Article/details/gdsembgbf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gqhywziue.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/gqngwjpgu.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gjigupzai.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/grjtnbptn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gmkrdcaez.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gzijzfjyv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gytnjvgxo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gzsnjwaiu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gbvwswilf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gesimvjyu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gnamawgxl.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gebfodwwo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gsidbufel.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gnxckjskm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gadbjkclc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gvdeivozu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gjqxixslw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gnjrumocv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/ghjqekuzq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gxdinpxpu.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gjoxdawfj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gujmnxiev.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gzcppfgpw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gkfcwvxuq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gvzkwwuha.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.bbcook.cn/Article/details/gpzdzpivw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gnssstbbw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gaqozizzv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/ghgpswhhu.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gglvyqziq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/grbbjbphq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/gaafpyidn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gysfivbzy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gykjbnqoi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gybcxlcsb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gdjcqpcad.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gnnvfslkn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gstmdjzxg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/guhpsqjfe.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gjtqowzdv.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gntnkdygs.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gnxqvzwij.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/grvlzewyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gmmwqbxrx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gtovzlxvu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gazjdpnse.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/grpwtckpj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/ghsimashw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gjsilzwmw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gdmjapxpm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gkyvdgbvf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gmkdecetu.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gnrijqwuy.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/glejrhuaa.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gwbbqjxfe.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/geabrmsjb.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gcovmeeyp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gszmwayjm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/grxvbpjak.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gzzkzmuwi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gblzpdiap.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.tarul.cn/Article/details/gommjtcdm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/geonthbsg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gzuumtgiw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.tarul.cn/Article/details/gecyajbgl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyicgosgm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gtfqgvlxu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gaswgsrcm.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/geckobmcp.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gjrvwjbke.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gzaspvlpx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gficurizv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/ghlpomxzj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gsytrjgva.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/gmpuemwkp.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/grstetbeb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/ghriuufho.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gcshdflet.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/ggdeljrdp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gjhqetlqf.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gjhsvsikj.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gajaaralg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gostesyhd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gwvxaibna.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gbjohzkqi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gytssgvbs.sHtML

[M03] 执行外部命令
来源：http://www.share.tarul.cn/Article/details/gzijwimeu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.yfazqb.com/Article/details/giwvvxkac.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gtcaazrzw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gsrbweuih.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gbnqnxwdq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/goaynzwji.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gragvumty.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/ghywgvhea.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gweggzvuk.sHtML


<!-- 参考信息 -->