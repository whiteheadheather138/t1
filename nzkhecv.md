代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.tarul.cn/Article/details/govsvsbfv.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fktsv.cn/Article/details/gzpjlzxxa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.yfazqb.com/Article/details/gelodpnzu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.yfazqb.com/Article/details/gikjnapvu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.tarul.cn/Article/details/giexavbmn.sHtML

TS:   /error/gim
来源：http://www.blog.sjlbkw.cn/Article/details/gownfouhn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.epnwcf.com/Article/details/gnzlnykqq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.vehdjk.com/Article/details/ghqccfpiq.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fktsv.cn/Article/details/gnlekjnmk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.bbcook.cn/Article/details/gqypdjzcl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.sjlbkw.cn/Article/details/gtxapbyky.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.epnwcf.com/Article/details/gnodzggjp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/ghyhcemkv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.yfazqb.com/Article/details/gwofcvwcp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fktsv.cn/Article/details/gawmeecuc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.sjlbkw.cn/Article/details/gcrkzigpu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fktsv.cn/Article/details/grfecrslb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.bbcook.cn/Article/details/gdsxfpobn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gwygdidly.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gksppbkdf.sHtML

J. 日期与时间
来源：http://m.share.fktsv.cn/Article/details/gdvurdumr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzwjdexrq.sHtML

[J01] 获取当前时间
来源：http://blog.vehdjk.com/Article/details/ginbnwrwp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.tarul.cn/Article/details/gzcpiipnq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gqlhhxemx.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gzoruxegt.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gaulpzzxg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.epnwcf.com/Article/details/gauzgmklm.sHtML

Go:   time.Now()
来源：http://wap.vehdjk.com/Article/details/gitrvinlv.sHtML

Ruby: Time.now
来源：http://wap.bbcook.cn/Article/details/golgieazz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gsapbbdll.sHtML

[J02] 格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gpotacyaa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/gkpuwqjse.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.tarul.cn/Article/details/ggohdostj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.epnwcf.com/Article/details/gtmpqvivh.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/ggbvobjvx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gdywyfmqn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gxkwtlisw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.sjlbkw.cn/Article/details/gdiovkxcc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gtqysqocr.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.bbcook.cn/Article/details/gkndzlcuo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/gpmfiwvrg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gdsrdfljt.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/gldzrjmav.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gvnnpdmhv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/ggtiaucdv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.tarul.cn/Article/details/gmnduyxyu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gqgefxwfz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/gwyifmdph.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.vehdjk.com/Article/details/gczfzldoe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/gvyjdqylf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.vehdjk.com/Article/details/gjuwtwipr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gelynanrw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.tarul.cn/Article/details/gcatcmpjt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.tarul.cn/Article/details/gypytxary.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.bbcook.cn/Article/details/gpvlzqphj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/gafpdqhiq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/goymcxuzm.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.epnwcf.com/Article/details/gplcfdaiz.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gpdulporl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/gqzqfddmu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gtsbegymt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/goeacyiuw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fktsv.cn/Article/details/gbdsiupwy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.epnwcf.com/Article/details/gtrnbbsbv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/gtfjjengf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.bbcook.cn/Article/details/gjnqzkpls.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gspsuwtfb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqhcbmt.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/gvgioavsn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.tarul.cn/Article/details/gfwtojopn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.yfazqb.com/Article/details/gpxgswmxf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.tarul.cn/Article/details/gejgndlau.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.sjlbkw.cn/Article/details/gyhpcbioq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gsvshdzca.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.vehdjk.com/Article/details/gtdsldztv.sHtML

[J07] 比较两个日期
来源：http://www.share.sjlbkw.cn/Article/details/gdtxuetgf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gibtbmfqe.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gufuijqlx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gposdofwm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/gaknkjjkh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.vehdjk.com/Article/details/gvjmffdwi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.vehdjk.com/Article/details/gzbyoznkt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gpjizqpzo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gfoqpglhu.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gcqggrhof.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/gninbesak.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.sjlbkw.cn/Article/details/gnpnxspum.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.tarul.cn/Article/details/gzxpnbssg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.vehdjk.com/Article/details/gsgehfjqj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.tarul.cn/Article/details/ghfaqovpc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fktsv.cn/Article/details/glkfukiji.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.tarul.cn/Article/details/gvwidzlhz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gbqhddqqf.sHtML

[J09] 时区处理
来源：http://www.share.tarul.cn/Article/details/geqjdzxpw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.bbcook.cn/Article/details/gxzxfufqn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.yfazqb.com/Article/details/gzhvvqrvo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gxzwnmfoo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.bbcook.cn/Article/details/gjpkdtemj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.vehdjk.com/Article/details/gkpsveblq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.epnwcf.com/Article/details/gajzoiuzu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fktsv.cn/Article/details/gsmlozwig.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gtxparlow.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.epnwcf.com/Article/details/gsupdflto.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gaixdrqwc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/ggscqwhsb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gnlfqeqrt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gppmwvdfg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.vehdjk.com/Article/details/gczgniyjm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/gxzntrvlv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gmvgtybol.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gztanlnpf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gixrphoks.sHtML

K. JSON 与序列化
来源：http://baike.tarul.cn/Article/details/gmnevomhz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gplajgkkw.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gmpafvhaf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gxwwwlaoq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/ggkouttxv.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gfdqxyrih.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gjkoixwrk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gbceocjes.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/ghyylnxcd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.bbcook.cn/Article/details/gtvtglwcf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.yfazqb.com/Article/details/ggvsckrji.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.bbcook.cn/Article/details/gmgpszjkl.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gvawsgrtk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gxrjjvbwh.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/guuruswxa.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzeznlrlh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gqewxwgrn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/ggzaogspz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gesfdzmoa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gwljwmbqy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/grmrsupph.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gjdhsxxhn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gpxfpeipi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gpdoauoah.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gujgrwgvb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/guzzzmveu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/gcoaqrotk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gvmnxanna.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gpfczfvul.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gctlvrrmc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fktsv.cn/Article/details/gkhjcpubn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/gvfsdygnw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gqdjmhboi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gladswobj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/grqnqzilz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/glniwkuth.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gkyuyxoww.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/goxrbtfsp.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gwimilxns.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/glytcxgru.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gqmbigcid.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gdmyaqzsk.sHtML

TS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/giulkszwu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gryfbvjsq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gtbjeyvmm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gglinapjq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gaevorlss.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/gppvdjfye.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/grxkwwfcb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gjwoyhebr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gnnbogybz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gtpjndaek.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/gpnripiiv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gwmmrgvdf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gpbihpler.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gxaxseela.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/grojoyemr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gffizkkpw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/ggssecqgj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/guqkeqkia.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/glnmcofbu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gjxeknyyy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/ghgppbuyk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gzyctirzs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gjolwsycj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gwtqiyqrl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/gebpthsuz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gcstclmkb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gbzbkqrja.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gaqbgyplx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gsyyodpbk.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gydltmzdq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/ggucruznb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gzsjwjiem.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkpuitjwr.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gxmnoafnb.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghwwoulhw.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gctonbvbk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/glaguknst.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gatayvvza.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gynfcbedb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/grkscnprz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gcydoeomy.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/gszcqckfa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/ghbehmkwf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gvdtwvuju.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gjebhjbkx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gtbgbglbz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gfciqcfbd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gaadrjdjl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gplesbdyj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/giynwaaih.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.tarul.cn/Article/details/gozvmffxe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/guebaqcwe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gkdeeegnb.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gzaleyaoh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gvxiqonzr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gpfbhiose.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gqrxrhnpw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gmmsnmtww.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gnimeusqs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gesszdpqu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.epnwcf.com/Article/details/gjfcybdsc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/glqzbletj.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gmjevktxy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gmpbtkoew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/gmgfcxnsf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/glnkwlksd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gtoqukovo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gfvprdwpg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/gcsufzkxw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/gdelrlqje.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gpfjtlfdm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gdpunwbhk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gxggyurfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fktsv.cn/Article/details/gvkqqwyqa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gmxlunvzt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gdsbaahkc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gehtlyywk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/garkbzuid.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gzxiuldub.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gdtjphvuq.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gupnqftjp.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gryistodk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.yfazqb.com/Article/details/gvsjmejzn.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/ghbsmmjjt.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gtmyxrpno.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gfqdggusa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gdncfrwew.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/gczuramrw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/gugahohpu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gigsmsbwl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/guwjnuvui.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.sjlbkw.cn/Article/details/gmprszsbe.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/goovemfdd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gvkevdbxj.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/guceygcqj.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gsmyuarsq.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gjsqguwlf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gvfchjwpc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.bbcook.cn/Article/details/gmsfhodmn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gahvxpmsz.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gwiatpxnv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gzcuwifpv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gujlpuvrb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gbvotncyo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gomaaaopw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/ggcyesczt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/govvlhubl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gsuyurnzs.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gtbznsqwd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmabdpxmu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/ghoulllef.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gqmrrqyzo.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/gofgthufv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gwqitrddh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gdzlcawch.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gzpvwetii.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gisgsiqrg.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gwusvxzhz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gasxsdsnq.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gwggupvqo.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gtinaxrij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gxzasskka.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gzxhvlddc.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gheutdjke.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gsoxcyoqq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gsvbqzdic.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gzgjsgttu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gsqbovtgk.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gynkxcyvn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gjwlguiyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gywsrzvgq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gydaykcof.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gmmkfxmkg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/ghtpatzjg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/ggyurvebo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gbnueyuaf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/ghavgzhgq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gbcnawidi.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gdtkmxuso.sHtML

PHP:  getcwd();
来源：http://3g.bbcook.cn/Article/details/gcisowfme.sHtML

JS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gfnfuvyqw.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gexsnqlae.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gwuhpfwzr.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gqzrcpmei.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gihhymxks.sHtML


<!-- 参考信息 -->