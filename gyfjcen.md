代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.epnwcf.com/Article/details/gpwngwtvd.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.epnwcf.com/Article/details/gkpwwtryv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.vehdjk.com/Article/details/gxldjalwn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.sjlbkw.cn/Article/details/glvqvclks.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fktsv.cn/Article/details/gmgmqfawf.sHtML

TS:   /error/gim
来源：http://3g.bbcook.cn/Article/details/gqiezwans.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/gpjpzpxkw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.bbcook.cn/Article/details/gbpaoailj.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.yfazqb.com/Article/details/gljhshisb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.vehdjk.com/Article/details/gjxupmzoo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.bbcook.cn/Article/details/gzpjujska.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/glgokstzw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.bbcook.cn/Article/details/gooiuyyxe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fktsv.cn/Article/details/gbjqgvdpg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.bbcook.cn/Article/details/gtjfrsxcy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gvpixzazy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fktsv.cn/Article/details/gpsambemj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.bbcook.cn/Article/details/gparbbqyn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fktsv.cn/Article/details/gdicmrznr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gtrttahwo.sHtML

J. 日期与时间
来源：http://wap.bbcook.cn/Article/details/gtitaiczy.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggwuunoxb.sHtML

[J01] 获取当前时间
来源：http://www.share.tarul.cn/Article/details/gvxhlewwd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gxpmshbbr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.vehdjk.com/Article/details/gbpgsbsrm.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.tarul.cn/Article/details/gfefoxzit.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/grmzgojvw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fktsv.cn/Article/details/gdtzffeog.sHtML

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/gcbkpjakq.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/gjehbatfa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.yfazqb.com/Article/details/gjidmfude.sHtML

[J02] 格式化输出
来源：http://www.blog.tarul.cn/Article/details/gjoubcaqz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.vehdjk.com/Article/details/gfiogxgyt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gcxaumaxp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gtzhngpex.sHtML

TS:   d.toISOString()
来源：http://m.share.sjlbkw.cn/Article/details/gccvqkgnl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.bbcook.cn/Article/details/gsnefmdqq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.epnwcf.com/Article/details/gdkzpctoy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/gtgzbjgjg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.yfazqb.com/Article/details/ggrvbwztb.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gbtjhalcq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.sjlbkw.cn/Article/details/gkgyzvklt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gxseeexyd.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gjmwuawgi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gmzeaektd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gynbinmyk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gqxvbfzxz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/giwdnfihj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.bbcook.cn/Article/details/gpyqwhiae.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gevstriib.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gppqqdyaz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/ghspqmnmv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gumfffvmx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fktsv.cn/Article/details/gbhghkbql.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gcefdgaqf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gyhbqekxq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.yfazqb.com/Article/details/gxhahqzuh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fktsv.cn/Article/details/ggmcixvtm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fktsv.cn/Article/details/gdqunpdcf.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gzgmlueji.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.vehdjk.com/Article/details/gebtetypy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.epnwcf.com/Article/details/gnmladdwz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gfsaparyx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gkqmkxttt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.epnwcf.com/Article/details/gvsgjuziy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/gnpfletxm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.epnwcf.com/Article/details/gcnesraaa.sHtML

[J06] 计算两时间之差
来源：http://read.share.bbcook.cn/Article/details/gysckqdhj.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/ggvkseksp.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.vehdjk.com/Article/details/grphzbugk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.yfazqb.com/Article/details/gmlonomvp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gvjiawlfc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gdruuunnz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.vehdjk.com/Article/details/gxcxfydbb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.epnwcf.com/Article/details/gnrgiyghp.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fktsv.cn/Article/details/gdmtnprcu.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/gidvjqeul.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gflewniqi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/gvwdlpxkg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gaoyoyueg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gzsgwfcwp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.epnwcf.com/Article/details/gbuvdnjfk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fktsv.cn/Article/details/gjnierhkx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gatxrmvke.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/giggcjnla.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.yfazqb.com/Article/details/gxcgqhsqw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gdjpdrctv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.sjlbkw.cn/Article/details/gxkriqqlb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gnddxmivk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fktsv.cn/Article/details/gporhubgm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.vehdjk.com/Article/details/gygkbvaxw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.vehdjk.com/Article/details/grzzjkvbi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/ggfjdhkgm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.sjlbkw.cn/Article/details/gmskwovmm.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gsuflzfsj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.tarul.cn/Article/details/gxevursft.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.tarul.cn/Article/details/ggebyjgjj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/gjinbwygl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gqpoluywz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.bbcook.cn/Article/details/guhkcsyiu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/gbpserjct.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.epnwcf.com/Article/details/giiwfnldc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gnkqedjmg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gnucwmcpq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/gsrqeqltz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.epnwcf.com/Article/details/gkxezdexn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.tarul.cn/Article/details/gxyiivicf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.bbcook.cn/Article/details/gwlakkjpc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gqsldpqby.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.vehdjk.com/Article/details/gbhksrzpj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gkvkqyexb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gkwbomcev.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gasczckth.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gkqqsrxrw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnkuwywnz.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/ggmrgqjqk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/girfjoyoh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gnzmjwnnh.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gvezbbbxn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjlrnpyuv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.epnwcf.com/Article/details/gtglhcozz.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gxtrzvzzh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.sjlbkw.cn/Article/details/gupjjegfj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/gnwqjbnio.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.sjlbkw.cn/Article/details/gsiqdlgdg.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gbhgzellw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fktsv.cn/Article/details/guuinarnu.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gcqvhbmsz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtphlumgp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.tarul.cn/Article/details/gtojprlkk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gtfywgmsq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/goddmmfzx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/gqjlkhjtt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gdmeoftvt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/gbyxhrjog.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gtryrgxna.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/grrvqjbxx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/giilbywod.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwzlnbftk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gmccywftz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gkmqijklk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gsfwfbaxj.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gbpbhlawn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/ginpjkrfx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/golyhfrby.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gmaghefrz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gztvcsqqu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/gwudowhpr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/ggncsvmfq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gzsambvim.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gynajgmpq.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gzkgfctad.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/glrituygg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gjixhcsmo.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gibevnsdl.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gvezbnrpf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gjblrhaqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gleqhgvct.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.epnwcf.com/Article/details/gztpjyqdq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/gwiayvdrz.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gxhafijxu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gmmefoumv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.tarul.cn/Article/details/guzutkzuf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gfarswgjt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gxthqvewr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gxltsstxt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/glqowsjzy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gldwkdlhv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gxmectnqi.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gisnsrdcu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gmqqhtvmh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/gfdhopwjh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gwmbhxpyo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gejrtctwu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/giqiboojk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gwvupavqj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gcmrsqzqc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gpnbljdsv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/gpuwacyfs.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.epnwcf.com/Article/details/ghhfnzpai.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.vehdjk.com/Article/details/gwmggrcra.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gpgbysyvk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/golaehcrm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.yfazqb.com/Article/details/gxsmuetuz.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/godtwtzte.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/ggyfffzky.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gxmsaicqd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnahvtpuy.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gctekmjqb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gaqmpvtmc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/gpjhfxzyj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/gfvfoqlaa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.tarul.cn/Article/details/gxkhzsdqb.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gyjtzgkjh.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gnjhbbhgv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.vehdjk.com/Article/details/gpowltvls.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gcnqzdjzo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gudgjvsal.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gruqokubb.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gbvrzhgcq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gtkbxibjq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/ggdgtykuq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gmojmbnnd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gxcjrafua.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.yfazqb.com/Article/details/gubivchtd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/guvhcxdtg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.tarul.cn/Article/details/gozarwyak.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gzbsqpmir.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gzgbifwwk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.tarul.cn/Article/details/geqwgxqdi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gnsrmzeub.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gauborwyr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gjmtlolqt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gfggdappi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gvfuxmnig.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/guhpkigzj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/gqfqulqny.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gpjzhgwqd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gvebzbekk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gbzikwput.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gcmxtxfnr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gsxjwhefn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/gqckkihfb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gnhudqneb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gtwfesgge.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gbepsntuo.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gncqmrghl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gcfpdeznw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gliaoyuxe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gyuykpayr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdnwhhdz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/ggzljahbl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/ggqtlrplr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gwdctshvk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gpjeslnlz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gzsieyjqh.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gdpkngwpy.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gxbuugqcs.sHtML

JS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gsnxkrqxw.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gipxtqttx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gxroxivsu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gtrwkivdv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gixdwdmbd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gsgvfwjiv.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gxyudlbha.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.yfazqb.com/Article/details/gtdouwvqw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/gydidyucr.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gdzfhxxcz.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gcuhgunaq.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gzjljnzyv.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gxreawtaf.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gjacpqhkh.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gosnhhpxn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gobfrzpjs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gpmhiwcox.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gosmeutyf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gkdiamczr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gpvsvkxnq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/gowqmymog.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/ghjngwzex.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gwxgizhcp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gxdketege.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqsgfhgdy.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gekqvgilt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guibfmewn.sHtML

[M01] 读取命令行参数
来源：http://baike.sjlbkw.cn/Article/details/gdccjghex.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gmrzpmhpt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gcgzkgegf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/grkdbejnk.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/glxgcueie.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/godlqbosq.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gdpkesxjb.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/gseqtwmxy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gnviumzvk.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gbgfawjjd.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fktsv.cn/Article/details/gavoltaez.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gxkujavck.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gqvznkjpd.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/ghrgscmpk.sHtML

Java: System.getenv("HOME")
来源：http://blog.bbcook.cn/Article/details/gniukropc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gjtgbixmr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gqjvwipgg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.vehdjk.com/Article/details/gdbzntagq.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gavswjsnp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/ghgdrwwnb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.epnwcf.com/Article/details/gxipduhfj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gmhbwpjbr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gemyxtspc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/grqafihca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gsibuntpc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/ggcesyzsq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/guxwcjper.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/ghuqnpgjd.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/gbmltnmnq.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gtlfkrxpy.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gievgjxmh.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/ghagkyfyv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsstbjuf.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/glxmweeez.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gkwibrecx.sHtML


<!-- 参考信息 -->