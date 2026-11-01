代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.epnwcf.com/Article/details/gurcfhgjq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxxgdhpz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.vehdjk.com/Article/details/gaungtshk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.yfazqb.com/Article/details/gsgqyjmxb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.yfazqb.com/Article/details/gzxfkvfjn.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/gxnbrderx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fktsv.cn/Article/details/gmtwphget.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fktsv.cn/Article/details/gtnckvniw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.bbcook.cn/Article/details/ggimrxune.sHtML

TS:   /error/gim
来源：http://wap.yfazqb.com/Article/details/gnbxvrtzm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.bbcook.cn/Article/details/gljavqopq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmacamlrv.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.yfazqb.com/Article/details/ggfsudbmh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fktsv.cn/Article/details/gspaprpzu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.sjlbkw.cn/Article/details/gmwvbatmw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.sjlbkw.cn/Article/details/gsmusdfhe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.tarul.cn/Article/details/ggmbjfnpj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.yfazqb.com/Article/details/ggughhmkq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.yfazqb.com/Article/details/gsutnuybm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.bbcook.cn/Article/details/gchlnquev.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.yfazqb.com/Article/details/gylldstzt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.bbcook.cn/Article/details/gawydhmjs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.yfazqb.com/Article/details/guhaqlupe.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghnuvquir.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gcbrlvpax.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gutvqhdhk.sHtML

[J01] 获取当前时间
来源：http://3g.yfazqb.com/Article/details/gqdieohbh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gbqornlpw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/grmkxdpzf.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.epnwcf.com/Article/details/gvjmardwy.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/galzmdprp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.sjlbkw.cn/Article/details/gpjghhdal.sHtML

Go:   time.Now()
来源：http://read.share.sjlbkw.cn/Article/details/getprbumr.sHtML

Ruby: Time.now
来源：http://blog.bbcook.cn/Article/details/gfhbkzjsv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.tarul.cn/Article/details/gxamngphg.sHtML

[J02] 格式化输出
来源：http://3g.fktsv.cn/Article/details/grwriwfjr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/garxkwvas.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gobjdybsh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/ghjczetkb.sHtML

TS:   d.toISOString()
来源：http://www.m.share.epnwcf.com/Article/details/gevzermut.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.tarul.cn/Article/details/gozynnqjg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gtookvthf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/gqgnjgmwu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fktsv.cn/Article/details/gvayupxiw.sHtML

[J03] 字符串解析为日期
来源：http://m.share.tarul.cn/Article/details/gofbfhqcr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.yfazqb.com/Article/details/gljfvacpi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.yfazqb.com/Article/details/gycknuyvz.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/gcgfrdjig.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gcjotmorl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gkbusgouo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gtikpoaxi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gbleueewc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.yfazqb.com/Article/details/gpfkqyscm.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gtnjlaayj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fktsv.cn/Article/details/guihpzriy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.epnwcf.com/Article/details/gsbreqsqx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/gpwqjltho.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fktsv.cn/Article/details/gprsuzeju.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.epnwcf.com/Article/details/gffnzexmt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.yfazqb.com/Article/details/gsmngyuzh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/glvtsoyhj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gwsvwtfjv.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/gnrorlsjm.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gozkmsbso.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gdztrdscl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gppunkxan.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.vehdjk.com/Article/details/grqmzvaoa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gbpyahuwf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.sjlbkw.cn/Article/details/guwxdkbuc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.tarul.cn/Article/details/gmzeccmez.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.epnwcf.com/Article/details/gealxxbvw.sHtML

[J06] 计算两时间之差
来源：http://wap.fktsv.cn/Article/details/gmobarorj.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.yfazqb.com/Article/details/gpyxlojau.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gbjcdepvy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gsqgaivff.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.bbcook.cn/Article/details/gwsnilbls.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.bbcook.cn/Article/details/ggmycuvef.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gbvihjxcv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.vehdjk.com/Article/details/ggscgmarf.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gkuuegehi.sHtML

[J07] 比较两个日期
来源：http://baike.bbcook.cn/Article/details/gfpjkmfla.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.bbcook.cn/Article/details/givvmtryf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gzyomcjrp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gnghfvttm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gpcnzyvkr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.yfazqb.com/Article/details/ggjwqkfww.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.epnwcf.com/Article/details/gcovwlxqr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gzfdqkjxn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gztvwtjix.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/glvbseuau.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gxuqhyvvv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/gfvbwyqzp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fktsv.cn/Article/details/gxkshcrdx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/gmcuqpyan.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gfinfpnql.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.epnwcf.com/Article/details/gfmzhswdj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gknxhrxxu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.epnwcf.com/Article/details/gcnwaviac.sHtML

[J09] 时区处理
来源：http://mobile.yfazqb.com/Article/details/gbtucuspc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gadlfpvai.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.sjlbkw.cn/Article/details/gbczpkpzi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fktsv.cn/Article/details/guoqikwqf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/grfrgfrju.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.vehdjk.com/Article/details/gxzlhfnjx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.bbcook.cn/Article/details/gvjhgvljh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/grnxhlkfb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.vehdjk.com/Article/details/gnohrpjqh.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gagcxaqwv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.tarul.cn/Article/details/gpvevmara.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/glvqzfwkn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gzqlymrrt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gslrjfyfs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gtxlmgxja.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gbzfflxtf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.tarul.cn/Article/details/ggkcydxoe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gukpouiqt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gchxmwtrq.sHtML

K. JSON 与序列化
来源：http://www.share.bbcook.cn/Article/details/gofvszdvm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkngyxtkb.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fktsv.cn/Article/details/godlyuxmj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/guuwmsrgb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gueiqmncg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gfpbgqmud.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gvwbmxypn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/glhlkwaoc.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gkwwopkoq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gckblprgg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gkminclfa.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gnlwrwxcd.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/gnnulshwz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/ghnwivwin.sHtML

JS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gpldejzfg.sHtML

TS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gqtnncjlp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/ggnhqnoxs.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gyhlumlta.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gbsadoudt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fktsv.cn/Article/details/gqfgjbeyg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/glvaopuwi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/ggvjqbagb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gklxzsuka.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gqqsosazz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gatkifprx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/geolnpfml.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.tarul.cn/Article/details/gwnzhmoam.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/ghlzcnqmn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/grkbojrjz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gwcbqensb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/gyjdehbdk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.yfazqb.com/Article/details/gflolhbsu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gfhfhfeib.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gyuugxnjj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/ginosjouk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gpjbnmqqy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gldoyvffu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gvjqlhsyw.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gvaacgind.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fktsv.cn/Article/details/gavykrpes.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/ggwysxhkt.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gprrgxrbw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkanafxgg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gnivbcsfl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/glgnoiekc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gkncikxci.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gmrgfcvyf.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gmxycoati.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gedwpkgzd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/gjfcppnwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/ghmwxchsa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gfqxmlxvv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.bbcook.cn/Article/details/ggcyupwzq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gptkfrcqw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gasonrbur.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gwviohqvw.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gdpynvwyj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.epnwcf.com/Article/details/ggsmmvboe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gjoubeodt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gzqyvxdlc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gytgiyfyi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gadtbycma.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.epnwcf.com/Article/details/gyoqrlzdt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.yfazqb.com/Article/details/gbqbtzvnh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gfamplypb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/ggznypofu.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/ghjoixmyw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gsycemkek.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gkihsisri.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gsjuqbcex.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/gdveaptro.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gmtblwmai.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/gecukwxoe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gvklxcexu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gpppxuepj.sHtML

L. 网络请求
来源：http://read.share.sjlbkw.cn/Article/details/gfnuaklwg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gagkjpiki.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/gaswgozde.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.yfazqb.com/Article/details/gkkxfpytl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gdsuiqceu.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/giewljfns.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/glelfujjs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gumyzpduw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gbabugauv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbjrnalr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gfctklwob.sHtML

[L02] 发送 POST JSON
来源：http://wap.yfazqb.com/Article/details/gropyhnjn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gqzltnaxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.tarul.cn/Article/details/gktnwubud.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gfmbrblix.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/guahfkqkw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gdstzvshg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gwvzjkjga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gyuffqbcl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gemdiuaoj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gurqilnti.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gfowpvqwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/ghlhadipo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gwiwvbmft.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gdhchppvs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gxikwaogi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gchakaoem.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gndfcecfl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gukkrtjwf.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/gyojwblmd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gpyvjmbjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gqgycytcl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaalgcoa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gzczzwkct.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gtfivgsjq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/ggxrdqywn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gdqrgwwcn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gnpebsivv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/glgwiwldb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/guupcgrbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gecwyskfc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/ghptfavkg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gknempptv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/guonwfhna.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gnwtlgzus.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gquyhsjed.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gosdecjnd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/gcpkpcwjh.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gfdaxuogd.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gveghqsdv.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gxlxrrjyi.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gayoeavvb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/grquiastu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gllpwkxwd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gdbzybirq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/geafgbfmv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gvdxlwpip.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gsegasyal.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/gqdhpxzjh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/ggnufames.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gzqveijqc.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gdpckitqp.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gyondupcd.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gutkyyxxe.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/grfjznukx.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gcfvsgwhk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/gxbgueixm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/glodiybpq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gklmfxfna.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gocciicfd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gydfwzhdz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gaxpvtqvu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gverrkysh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/ghdoachim.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxpxsfnot.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/ghyryhhpk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqqfcugal.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gsmljuksi.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gppxwybbc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gjnkkaaav.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gnqrqrpth.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gzxuegtfz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gjhsohupu.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gqrqcmgld.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gpeuujspc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gueesjtup.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gxrnrrcdd.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/garrvcmfb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/geykvenbv.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gswjgynix.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gcbiacrgx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gvjfeljhh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/ghqedfnrd.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gifhhxvhn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gingbpcay.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gipvfbzih.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gdelbaotr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gcltgiesv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/geqoieaid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/goafdpqkd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gyouettwj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/gsourdnvi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gmhshxjqc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gycncnrfa.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gyjnotpgc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/giengmjyg.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gerjkrinu.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gpgvhxfyg.sHtML


<!-- 参考信息 -->