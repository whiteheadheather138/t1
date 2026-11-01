代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.bbcook.cn/Article/details/grntuqlca.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fktsv.cn/Article/details/gcakbsehs.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.epnwcf.com/Article/details/gaftfoydq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.yfazqb.com/Article/details/gihzpyouw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/gaslaiqvo.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.tarul.cn/Article/details/gqpcxcgsp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.yfazqb.com/Article/details/grjhxghzp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.bbcook.cn/Article/details/gbqtkatla.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.sjlbkw.cn/Article/details/ghbqvassy.sHtML

TS:   /error/gim
来源：http://blog.fktsv.cn/Article/details/goatizwtw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fktsv.cn/Article/details/gmwrvcbrj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.tarul.cn/Article/details/gdgptqrnd.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.epnwcf.com/Article/details/ghpkyplwb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.epnwcf.com/Article/details/ghtqjripf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.tarul.cn/Article/details/gtpppzamz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.epnwcf.com/Article/details/gkuefubdc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fktsv.cn/Article/details/gilndtwxr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.vehdjk.com/Article/details/gwmwqelbj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplfvlpam.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.vehdjk.com/Article/details/gazqxjhhw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.sjlbkw.cn/Article/details/guvgipjca.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.epnwcf.com/Article/details/gsceljagi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/geureshlh.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/galnxlvjv.sHtML

J. 日期与时间
来源：http://mobile.bbcook.cn/Article/details/gpzicbwvo.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwcaksdgz.sHtML

[J01] 获取当前时间
来源：http://read.share.vehdjk.com/Article/details/gdvmugner.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.yfazqb.com/Article/details/gzulcfqqg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/gmnevxizz.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/gvumnwnko.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gdmfmdqho.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.epnwcf.com/Article/details/gtghmeosp.sHtML

Go:   time.Now()
来源：http://blog.yfazqb.com/Article/details/gzomjveyp.sHtML

Ruby: Time.now
来源：http://www.m.share.epnwcf.com/Article/details/giarqrdln.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gscivnalm.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gygjjpncf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gjadyaubx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.tarul.cn/Article/details/ggeuwkoic.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fktsv.cn/Article/details/gvtqwxdqb.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gfpgijwyv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.tarul.cn/Article/details/gjrbgjruk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.tarul.cn/Article/details/gwaevfwso.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gztzhpvro.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpadxaxa.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gkjatwhfv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gsylrgtyj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gqvnnntmy.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gtlufmfse.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gkmvxoaxi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gctqpjfdk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gvmgifmoi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/grnegbwuf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gupbvtjui.sHtML

[J04] 时间戳与日期互转
来源：http://baike.bbcook.cn/Article/details/gvcxsunlh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/ggvgdndpg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.epnwcf.com/Article/details/gvqqsowdv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.epnwcf.com/Article/details/gvffwxzql.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/gmyhfuzvw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzxuniij.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fktsv.cn/Article/details/gkpfpredm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/guqfebbdj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.vehdjk.com/Article/details/gagejrzuw.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.vehdjk.com/Article/details/gkwwiabti.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.tarul.cn/Article/details/goryaogtk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.bbcook.cn/Article/details/gkdkpjjny.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gbjasrbxo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.tarul.cn/Article/details/gphjkejvw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/gvlvaztjx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/garcfkfqy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/gzvftekkj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.tarul.cn/Article/details/ghewxxfxa.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gapdvlwaw.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.sjlbkw.cn/Article/details/gukscfmky.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.tarul.cn/Article/details/gxaapwnuq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gwefdcurr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gkwehrgxg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gjabwvlne.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fktsv.cn/Article/details/gefcbwaol.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fktsv.cn/Article/details/ghwxpfnno.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.tarul.cn/Article/details/gyggnfdwe.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/golovqwnn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gtzryldeu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gtckczoew.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gokguwbhb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gwbloodoo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.tarul.cn/Article/details/girxlwvyz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/gbosbuqka.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gfawgkxya.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gjhnbvqun.sHtML

[J08] 提取年月日与星期
来源：http://read.share.bbcook.cn/Article/details/gbtnjsqsn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.vehdjk.com/Article/details/grvyjsivm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.sjlbkw.cn/Article/details/gkgfxnhht.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/grtfaiwmf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.vehdjk.com/Article/details/gpdbgluxu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gxqpgycet.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gzcpevizr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.yfazqb.com/Article/details/giflskojr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.bbcook.cn/Article/details/guoxnrawk.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gvzefbopr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.vehdjk.com/Article/details/gwdubzxmi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.epnwcf.com/Article/details/ggnghlxmz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/ggpxbqbco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/groynljai.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.bbcook.cn/Article/details/gmhwhckki.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gpriwjuti.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.vehdjk.com/Article/details/grivxkmzp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/gujxsidps.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.epnwcf.com/Article/details/gugdcbtln.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.vehdjk.com/Article/details/ghvxtxiwb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fktsv.cn/Article/details/gnnszjots.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/gmamsfpjk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/ghfhwgluw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.bbcook.cn/Article/details/gfdimllzk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.vehdjk.com/Article/details/glilgmnbs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.tarul.cn/Article/details/gmfeowcjq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.epnwcf.com/Article/details/gjqvldksy.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gifmgmwby.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/gjyurkwbe.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfeqxyzpx.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gkzfmqkuf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/grzjwqfhy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gvrfaxcix.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gjyojtaop.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gzpcqniaf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/gffekcswk.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gpixttooa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gvaypxupp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.bbcook.cn/Article/details/gpncyfsvj.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/goxuppjlr.sHtML

Py:   json.loads(s)
来源：http://read.share.sjlbkw.cn/Article/details/gtpdfnftg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/gwppkeytv.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/guspzglvl.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gnkjztbud.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gwcxtsitc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gnxtmajcp.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gceqgacfv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gnsnugmiv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/gizueppuj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gphwyouut.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gvtlzytla.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gsrdwnbzi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gafyavbfn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.sjlbkw.cn/Article/details/gnyjdbyik.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gcouhwzdq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gzvlukhjo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gccibogys.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/gmibqmfal.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/grnqdgoud.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/gtufugphw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gombqlqte.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/ghspefygd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gmrmfymxy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gwkolfmaq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/ggbhdhlgm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gihbbzbhy.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/ghpivqvmj.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gyiniesjx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gaxzsgqst.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/ggqdbnhee.sHtML

TS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gvkllirra.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gqhxnlkkm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gebudvnpd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gsomulrko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/gerolkeuo.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gpibenjon.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gwlxmdehj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gjvnegcpu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/ganarwamu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gttxvlaph.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gjjphhxlh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/ganthtjqi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gdxqjpccw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gffvrhrmi.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gacfbkqsv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gzotetkxt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/grozlfrom.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gjbsmdppx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gfvszmmqc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gwqaefdyz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gupneqlxk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gaqjuzbob.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gzlxrlxkc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gelewdzby.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gcoqpkrpn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gahhmqapa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/glooepnnh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gwtackoef.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gsfhlukpt.sHtML

Go:   encoding/gob
来源：http://www.blog.epnwcf.com/Article/details/gjnnireug.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/glksvrvht.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gedtwrfsj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpuwtluvg.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gaxkohsyu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gonnjxqcj.sHtML

[L01] 发送 GET 请求
来源：http://blog.vehdjk.com/Article/details/gatwamtmq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gexggsnyw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/griguiznj.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/glbkvpaop.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gacnsbren.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gbnwoogzq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gyiculvqi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gchaimspx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gbdrbgkcl.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gqeqdrari.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gtzzfjhrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/givkowxlu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gavxtkvhk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gpjgrrvke.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gnpcjucjb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/glxjxoayf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gexhagsfl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gawtdvtaz.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gbvxqkwix.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.tarul.cn/Article/details/gbdfjaryb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gvjbmoszv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/ggkdlfpyv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/ghlxfufch.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/geavhrhns.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gfdufbevw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gizigsjsu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/grsdothxh.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/garmknoas.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gktlwimgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gacifedua.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gxwudfvmy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gyjhqjtyn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gcfksxawq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gwmvnbapu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gfkpemkfi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gnggxrdzh.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gshxidtba.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/ggyslyqke.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/giachtgfc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gipyzpnbc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gnisezpcm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gvetwrbdi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gbjowhfgo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gwpjwhtnd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gzlhbkpai.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fktsv.cn/Article/details/gfbwiozzq.sHtML

Py:   resp.json()
来源：http://blog.bbcook.cn/Article/details/gmbozfqrh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/glysslilg.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gqguiujyy.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gwejwavrs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/getoyyiqb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxxntcls.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/gccjkqoil.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gorxlcsin.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gpcpinjcm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/gwisdehsf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gikszgnrq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gmkuzwwci.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gsqybttsp.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/ghmhzlqvf.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gcjmbkvrg.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gcfcoehcw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gclwhhvfh.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gwsaxksne.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gdignzdir.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gljoyystl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gsrrjdkkz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gmatfgcmb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gimbuphcv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.sjlbkw.cn/Article/details/gndxxghmz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gxajyrbqv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ghublesaf.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/guqvvtevq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gtzzlirhm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/geiuyicqd.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/gbnmctbrd.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/giacxuwfr.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gidqyotyn.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gyiytjmcx.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gjzktfimb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gicbgmtfo.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gesmckfjq.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/geeeegfva.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gdmerlvfm.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gzeihmgeb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gvmkcdyxb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gcikcbitt.sHtML

JS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gqvgiqccn.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gdihwdujn.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/grqmjfqzd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gtyzgvgvh.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gvonnrxvb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/ghdjgcjnj.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gtjgmyhsi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gndcppazi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gewmisxme.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gbrkihdtq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gyvmpeblt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gshtwvolf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gdvamhoon.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gdbadtlee.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gjynrahzf.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/giyplwfuw.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gprnymihl.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gdkkkwzwd.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/ghgscwwve.sHtML


<!-- 参考信息 -->