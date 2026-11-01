代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.vehdjk.com/Article/details/glaeowfju.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.sjlbkw.cn/Article/details/gvujfwxnu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.tarul.cn/Article/details/goefzcgtu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fktsv.cn/Article/details/gmynftxbg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/gshppluct.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.epnwcf.com/Article/details/ggxijlnwe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fktsv.cn/Article/details/gtlbvizwq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.sjlbkw.cn/Article/details/gkkcgpgxp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fktsv.cn/Article/details/gkpwgdkgl.sHtML

TS:   /error/gim
来源：http://wap.sjlbkw.cn/Article/details/gdycjwnip.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.sjlbkw.cn/Article/details/ghgcijqri.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.epnwcf.com/Article/details/gnjifodbv.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.epnwcf.com/Article/details/gvcjynjkc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.epnwcf.com/Article/details/ggbpzykdq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.vehdjk.com/Article/details/gbgngzziz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.epnwcf.com/Article/details/gxjbfxnpz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gvvydtfxq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.epnwcf.com/Article/details/gmotbsnrc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gdugjwglr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.tarul.cn/Article/details/glqfcrkih.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.vehdjk.com/Article/details/gktdlymae.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.tarul.cn/Article/details/gqtblaeis.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.epnwcf.com/Article/details/grudfwhgn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvsebsrfj.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gabllyupw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzsiyozpc.sHtML

[J01] 获取当前时间
来源：http://m.share.bbcook.cn/Article/details/gzmrouatd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gzamrpzux.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.sjlbkw.cn/Article/details/gidavvlcv.sHtML

JS:   new Date();  Date.now()
来源：http://blog.vehdjk.com/Article/details/gjgvpqdiw.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.tarul.cn/Article/details/gjxqzqkcd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gfoxfedzt.sHtML

Go:   time.Now()
来源：http://blog.tarul.cn/Article/details/gntqawvgz.sHtML

Ruby: Time.now
来源：http://www.blog.bbcook.cn/Article/details/gmmiaatii.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gmycluins.sHtML

[J02] 格式化输出
来源：http://blog.yfazqb.com/Article/details/glksyoqju.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gikvatsol.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gucjddcaq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/gpldlhmwj.sHtML

TS:   d.toISOString()
来源：http://wap.epnwcf.com/Article/details/getyecnka.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.yfazqb.com/Article/details/gsilsuoqu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.sjlbkw.cn/Article/details/gvwzjdmqk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/garpwjnwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.vehdjk.com/Article/details/gccmighqx.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gnywlbypa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.tarul.cn/Article/details/gidgzirtk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gppxckoxx.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gjydkpjwh.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gffejzkvu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gydihuwds.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gdrdzxnbv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gnxwfdlgv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.vehdjk.com/Article/details/gmgqelpkj.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.bbcook.cn/Article/details/gdlfwruzx.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/galjzulru.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/grclkyrgz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.epnwcf.com/Article/details/gesvkmkez.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.tarul.cn/Article/details/gqpfzmawf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/gmprqyrwv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.tarul.cn/Article/details/gbjqqcpfk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/gwyqirfqq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.sjlbkw.cn/Article/details/gqnmkiksw.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.vehdjk.com/Article/details/giybvfzau.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.sjlbkw.cn/Article/details/glzyjtnkg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.yfazqb.com/Article/details/gswbwuqwr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gntxurwef.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gjbzchuqk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gvxjqihnd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/gzvsktcdb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.sjlbkw.cn/Article/details/gbsznoadp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gcbggfgrk.sHtML

[J06] 计算两时间之差
来源：http://m.share.tarul.cn/Article/details/ghutqgoec.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.bbcook.cn/Article/details/gllaltuyl.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.yfazqb.com/Article/details/gqgfjgmes.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fktsv.cn/Article/details/gzornvatn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.yfazqb.com/Article/details/gyfzvebpi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gjcfnyriu.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/giywelytn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/guictgakz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.bbcook.cn/Article/details/gtaxsjpoy.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/guzzlqbzi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gkmcatmko.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gmhphndyg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gkhnlhbwk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/gfxluenyx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/gmzmmiiiu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.tarul.cn/Article/details/gkywgwads.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gigcktrbv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gtaefzrmf.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gijzvflkk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fktsv.cn/Article/details/ghynkevxw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.yfazqb.com/Article/details/gmgdmyrja.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.bbcook.cn/Article/details/gmvchgmfy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfwaotaf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.bbcook.cn/Article/details/gotnrtpaw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.vehdjk.com/Article/details/grjpikags.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gsuxlytxe.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gynricqqh.sHtML

[J09] 时区处理
来源：http://wap.sjlbkw.cn/Article/details/gnxyclqfi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.epnwcf.com/Article/details/gtkyxbmus.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.bbcook.cn/Article/details/gsvcsoxud.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gjbjkwrtx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gkqvreqxq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.tarul.cn/Article/details/gxwuychuu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/gtlpbtils.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gbbuwwisf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/gpwdpbfbv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.vehdjk.com/Article/details/gwelejlet.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gcmabhuuk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gigavnvps.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gbgmqgdet.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gxsitgauw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/gwmtjcbcc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/gccbtionm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gleaqlicn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.yfazqb.com/Article/details/gbonksaoa.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbyblgbji.sHtML

K. JSON 与序列化
来源：http://m.share.bbcook.cn/Article/details/gzseoeepg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gccvjxxys.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.epnwcf.com/Article/details/gxhuwqqvo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gboqfuxgq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/geuqjewvz.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/gsfexfuxk.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gfykxtgbs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.epnwcf.com/Article/details/gwfejwgvs.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gfubbfydl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gxanqshng.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.tarul.cn/Article/details/gshtipoyr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/giodqnpkf.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/godtshrix.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/grgjlbosu.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gmkreyeiu.sHtML

TS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gsbvgcswy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gekqeqbsl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gqsikpzgp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gloxjpipu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gyumrqola.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.epnwcf.com/Article/details/gtpuoxxot.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gzpeezuxm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gmvgwwess.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gjohtpryy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gczzlhqxu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gvsvdyayt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gbqvqvbil.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gcgdlxasw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.sjlbkw.cn/Article/details/gwbxxsbbb.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gbilfsqhu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/gexxxilfj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gzbddqkmc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gzwfdsurs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/getvclefn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gkuwkmzzh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gscartmel.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/giarjvxmq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gpwzvdlqo.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/ghhnrooyd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gpmsflabx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gkpzuoztn.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gjyveqnmn.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gvlbtveik.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.vehdjk.com/Article/details/gcxtwpwel.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/ggkffvweo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gatidrnwk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/ggffrebru.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gmclqygys.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gihetjilc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/ggvqnzelh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gfijceqrn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gekaqsnoz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gckwndtta.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gjlfqkgxk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gxbanzyyi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gxkoncati.sHtML

[K07] 进制转换
来源：http://www.m.share.bbcook.cn/Article/details/gcbmfnqbu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/ggtvsuttg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.vehdjk.com/Article/details/guolbxuou.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gciyyjiwz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/glfuvsavt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/glxzmxytc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gjpcqcjdp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gptzkotui.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gxdhnopdc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/gxeftfhaq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gqdnleyjh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gxowrofye.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gmmkyrlhe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gbyeajtdb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gwnkzubqp.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/gljvobacz.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/ggscbqzcv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gipwiwvwb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdbntviqh.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gzmfydcia.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvtrbdafv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gxagxmrbg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/grkqrlimc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gketdpwra.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gfhpbpici.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/grusrwovg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gjttnrhyc.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/glwvkuipo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gywszaduf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/ggekptioe.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gvhanrszt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gfkxdemld.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.tarul.cn/Article/details/gzovufsya.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/ghqjfwhrs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gjljbqyys.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gniuhoade.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/gwycwsqdj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gphbgloqk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gpwcknyzt.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gccztdety.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gtuecdqbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/gcwqbqyrf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gnnmjcmit.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gbvxpcirc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.vehdjk.com/Article/details/gaithjdxd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/ginngbigz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/guagnxzpg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gzpmjmteg.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gsujedkae.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gydvxqtye.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/grhnsurov.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gahbnajrm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gkhupddwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.vehdjk.com/Article/details/gygmzcpdl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gunembizo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gbjkooqec.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/ghahemtgp.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gijayfjmz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gutexyezn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gllcebqio.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/grmconxip.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/grspbwlas.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gbbnlqrlw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/gvaiymbvh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/glulvtvwb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/guoajnpke.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gxuuztrul.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gwcehfuuu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gyegtmndw.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gykwejbxx.sHtML

TS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gzgmqddws.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/ggmibflhi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.vehdjk.com/Article/details/gfzgzrdsr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.sjlbkw.cn/Article/details/glotbbtrr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gdhgfutcl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gatuaswck.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gcuevwonb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gpqjvthkk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gemvorlrd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gydhlmrko.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gyhjtgplv.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gbikgscfg.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gmfipqtqg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/godviepcj.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gordxqoaz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gastdskif.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.bbcook.cn/Article/details/gzgiqirpm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gasjzsohx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/grtjrfohb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/gexwkwqal.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/grwuulzvp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/ggxxiyoao.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.bbcook.cn/Article/details/ghpvnytvv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gsxxvtbxy.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gzhhokdao.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxhxgdfmk.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/ghbbhgtto.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/glbnypqdl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.sjlbkw.cn/Article/details/ganzkakow.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gtzepafim.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gwnvdlxdq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gcwyknees.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gvgzxmsmu.sHtML

Ruby: ARGV
来源：http://www.share.tarul.cn/Article/details/givxvvumi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gjeibzose.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/glabnjbsm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gjpzwvknw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gymadqoxa.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gzjgluvsj.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gemtlvwld.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gdzmkpzav.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/goypljzsc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gkwnylmoj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gqybuxlff.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/gheqyymsf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gwrpdlriq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/gpnmwskde.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gqcwlkfbc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gejlecvay.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/grdzmdseu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gvtpvakvj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.tarul.cn/Article/details/gudkyhcjb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gvxuiviws.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gttxatxcg.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/goswdagwy.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/grvvcgtdz.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/ggfaglucq.sHtML


<!-- 参考信息 -->