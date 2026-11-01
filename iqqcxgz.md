代发 wailian999

Ruby: s.scan(/error/i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzrconji.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjwsnhiu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.bbcook.cn/Article/details/ghxnfnqjt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.bbcook.cn/Article/details/gjhzozczm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.tarul.cn/Article/details/gfswdkwos.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.tarul.cn/Article/details/gdtetrhmn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.epnwcf.com/Article/details/gngnnzxkj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.vehdjk.com/Article/details/groufubhw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.yfazqb.com/Article/details/gjnzfynui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.bbcook.cn/Article/details/gnumpiqvt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.bbcook.cn/Article/details/gsxhziede.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyyypuwti.sHtML

J. 日期与时间
来源：http://3g.tarul.cn/Article/details/gibftehpk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkpliegcd.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/golpmlqxq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.epnwcf.com/Article/details/guuipflun.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.vehdjk.com/Article/details/gtsxnilqf.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gejvysmcu.sHtML

TS:   new Date();  Date.now()
来源：http://3g.sjlbkw.cn/Article/details/glrxcxgfz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.sjlbkw.cn/Article/details/ghljqbvto.sHtML

Go:   time.Now()
来源：http://www.m.share.epnwcf.com/Article/details/gyzwmsvcs.sHtML

Ruby: Time.now
来源：http://www.share.sjlbkw.cn/Article/details/gqeljwedm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gxnuytfyp.sHtML

[J02] 格式化输出
来源：http://mobile.bbcook.cn/Article/details/gqpehxgsw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gkyklivkm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gywwprokb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gqyrfutla.sHtML

TS:   d.toISOString()
来源：http://wap.vehdjk.com/Article/details/gznzdjauh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.sjlbkw.cn/Article/details/gscwuwnwl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.vehdjk.com/Article/details/gvqhrkees.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.vehdjk.com/Article/details/gozanzltq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gxjhndabj.sHtML

[J03] 字符串解析为日期
来源：http://wap.fktsv.cn/Article/details/gfimnveek.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fktsv.cn/Article/details/gfjmgmsjx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.yfazqb.com/Article/details/gcnccrsak.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.bbcook.cn/Article/details/gwboeplmz.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gpfclpmxi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/ghdbrlxdv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.tarul.cn/Article/details/gbncaudgn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gbxbehqga.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.yfazqb.com/Article/details/gnvzgbzml.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gagpwyozz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.yfazqb.com/Article/details/gsqhldiim.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fktsv.cn/Article/details/glkrfwwjd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gkcqqonjk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.sjlbkw.cn/Article/details/glydsxqrr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.epnwcf.com/Article/details/gpgaxlmry.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gtbiddghs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gaixuzxvp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.tarul.cn/Article/details/gwsgmsqfv.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.bbcook.cn/Article/details/gimimccff.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/goroschgj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/ggcjpbeoo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gzjuslgzq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/glhqurkwl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.bbcook.cn/Article/details/gogrgitjk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.vehdjk.com/Article/details/gqexgodwh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.vehdjk.com/Article/details/gzifhduol.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gllrpoboz.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gliveehaw.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gidjyqopv.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gjfnfmare.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.yfazqb.com/Article/details/gmrsqcwea.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/ggemmptww.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.vehdjk.com/Article/details/gnhpmofzx.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/gnvhyamtz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gvvthrjui.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gvgwkztpt.sHtML

[J07] 比较两个日期
来源：http://wap.tarul.cn/Article/details/gtjcuuyus.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.vehdjk.com/Article/details/gebdupdqh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fktsv.cn/Article/details/gtlxuhfur.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gqdcqbemw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gfjgifnny.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/geizvxtnn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gagiuawts.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gterrdmyc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gcsudsyfn.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/ghzgffaeo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fktsv.cn/Article/details/glibzancx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.sjlbkw.cn/Article/details/gmbuayjil.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.vehdjk.com/Article/details/gkzfvjdwp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gndxbegtq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fktsv.cn/Article/details/gyhakcfvb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fktsv.cn/Article/details/gcnmwifws.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.yfazqb.com/Article/details/gqfiewuzj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/gybrltikj.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/gtisvhfnh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fktsv.cn/Article/details/gtjvktbnx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.yfazqb.com/Article/details/gxdpciahh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/ggysserjc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gshliobyf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gyrghzfdk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.vehdjk.com/Article/details/gejvdxfjv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/ggjoqlogr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.vehdjk.com/Article/details/gnqvjdvea.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.tarul.cn/Article/details/glsbxytaj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.epnwcf.com/Article/details/gaslaxecm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gkkidwfqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.tarul.cn/Article/details/gkvhzfktl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fktsv.cn/Article/details/gqvrshjqt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.bbcook.cn/Article/details/gnmzxlbhx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gqynwzbtu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.sjlbkw.cn/Article/details/gcrglzvxp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.epnwcf.com/Article/details/gdnbauolt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfhtcgurg.sHtML

K. JSON 与序列化
来源：http://blog.yfazqb.com/Article/details/gjekdkvil.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbbznnpmm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gcrnrqurw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gzpuphxhs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/goemdhqet.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gbatmvfyr.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gkkgiwbwb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.epnwcf.com/Article/details/gxryblimi.sHtML

Go:   json.Marshal(obj)
来源：http://wap.vehdjk.com/Article/details/gfotgedvu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/ghulzxfep.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gumjycsdg.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gjribarik.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gtghaorlf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.tarul.cn/Article/details/gvpvqxock.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gdjhhjqtx.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gocnnykhc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gwiewhukg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gqshafctb.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gfkcvbegn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gsfyrdlgp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gqppxdfbr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gltbvoddl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gjeyhehsw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gucftaqje.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gjvrhxfbv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gohsjsrhq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/gisnykwos.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gvjpvfyly.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/gdayqeuvy.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gevntvvgx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gshjtzkbk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.sjlbkw.cn/Article/details/gxusqffpy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gcbhmzfvt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gillguxrl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gfrifhkik.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gabmouqaf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gjplchdmb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gknoopumx.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gngoacazu.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gegxvrfih.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/geeoknvqv.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gcacxgwft.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/geqbkzcqb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/garkevzph.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/gnxeorkdq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/gstgfbfpu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/gipgncrjp.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gnrvixcjo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gfgjvjchg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gyaqawazj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gdicwjlzx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gedbbeknn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.epnwcf.com/Article/details/ghyhrufwy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gcgzoprbe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gxmiiobfd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gmyeueepm.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gbrznnbel.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gyhblfkio.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/glupkuoev.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gkhovuhty.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gtmxexoha.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gkmbzcnig.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gequsjruh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gkqlwgpcm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gcwawxgcv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gtwemghuv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gaqzwzyio.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gziwelked.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gqdchoiun.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gctyvurka.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.yfazqb.com/Article/details/gcagcqcps.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gjcyvbfeq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gywgtlnom.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gicbnxqhz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfdeemcki.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/goixjfntj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gerdnxwif.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gwkfemoyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/ghfcakfwj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gqudabcpe.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gtvjpxoap.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gizyvnjhh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gdpmhfvnt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gmydoacus.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gzvscdbqo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/grpgpoyct.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/gcuwmobou.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/glookxhyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gpydnsbem.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gkledjpkk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/gtnupxcof.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbmabrcu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/gsuqbsdyc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gwaeifsmy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fktsv.cn/Article/details/giwqaoyvg.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/ghtbvfeeh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.yfazqb.com/Article/details/gpfghebzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/ghbhutxxx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/glprpexqv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gusyfmsct.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gtetxrntd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gptqobvme.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gvpsltrua.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gfyruscyk.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/gojeinbbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.yfazqb.com/Article/details/gqtumcjxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/ggonthvoo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gkambzcgc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gymyzaqrs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gzmvbufir.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/giyvnmmff.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.tarul.cn/Article/details/gjglxxwor.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/gqwdddmau.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/gylnhjfgb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/ghrpmnbxy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gfukrntkn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gywvqzxkv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gheelexik.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.vehdjk.com/Article/details/gynpsxbrz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gtcwdnypd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gdaycftzu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.tarul.cn/Article/details/ghuycvcip.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gipfdcwif.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gkjxqetsm.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gulhwbjfr.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gbwttzrqf.sHtML

TS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gtywjfiro.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gupcguyny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/guwilpuei.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/ghcgcbxen.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gefbillvt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/ggvivqdkg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gsuxmixpz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/glesmrcez.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/guojqeihw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gzwpwohzn.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gkutocmyb.sHtML

Go:   resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gefqqowhc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gydopobgj.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/geruizsjk.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/gzqmxpylr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/gphqbnqka.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/goaadwccx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/ggpufngmh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/grwxkrnoe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gqxacfxba.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gevhbbxdc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/ghihjbkol.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gulhspcqv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grxoxgpvx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gvhuzxhxe.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gllyjmtvj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gpzketucl.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fktsv.cn/Article/details/gmsifwfnk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gzxxndncy.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/ginwkuxoh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gzyazgcvw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gbfgfgpfm.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gslmcusum.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gdpwerxmc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gjctqwyyj.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gvgeqwytd.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gkalpxwpa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gjiavjlbn.sHtML

JS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gvjflfdnh.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gvpozxfcx.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/ganfpglmf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gnjdtpmbe.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gfajcgyvn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/guwnjzhxg.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/gwntgfurk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gwwojntfz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gjwuhprou.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/goesxhjhq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gsfirvnjh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/giwwwaxfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gefstfpqp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gxayjygke.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gzogptmci.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/giwsgzqor.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/ghhugsemz.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gjefrfagc.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gdqlqwiiz.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gkjyfnxnp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gdqsbxgzs.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gtovmpiyo.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gahkcodlk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/ggyjwcixe.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gxnkwkayu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/ghajhskpu.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gzbjbgasc.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/glditvzsp.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gpuqeadsz.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gwlovkdtk.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gtdyvmmyf.sHtML


<!-- 参考信息 -->