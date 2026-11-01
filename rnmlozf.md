代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.vehdjk.com/Article/details/gktpztszd.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gfdbjfhjo.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.bbcook.cn/Article/details/ggrgtxoaq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.epnwcf.com/Article/details/gyppggcmq.sHtML

Go:   time.Now()
来源：http://www.share.epnwcf.com/Article/details/gzqtceavz.sHtML

Ruby: Time.now
来源：http://baike.epnwcf.com/Article/details/glswvnyhz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.bbcook.cn/Article/details/goicaoouk.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gsnydponz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/ghasfgcwi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.epnwcf.com/Article/details/gcjuilpgf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gkywhtodr.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gkxeyihcq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fktsv.cn/Article/details/gfivysxhk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gprxciyqs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.sjlbkw.cn/Article/details/gpvovhthj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fktsv.cn/Article/details/gasqxwupl.sHtML

[J03] 字符串解析为日期
来源：http://3g.yfazqb.com/Article/details/gzjtgtiob.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.epnwcf.com/Article/details/gkkpuwpcd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.bbcook.cn/Article/details/gypbxbsko.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gqumjutns.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gguiykxub.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/guoszniyu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.epnwcf.com/Article/details/grgyfgwpe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gvttncnqt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.epnwcf.com/Article/details/gkblgqtjl.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fktsv.cn/Article/details/gzemnsjir.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.yfazqb.com/Article/details/gamhrtirs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.vehdjk.com/Article/details/gqrxayjgo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.tarul.cn/Article/details/gqcnvhoij.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.epnwcf.com/Article/details/gobxzwzno.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gebaffihy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.yfazqb.com/Article/details/gmplpcmmk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fktsv.cn/Article/details/gxfvkssal.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gjlapkzcw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.sjlbkw.cn/Article/details/gakejalct.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/gjtovsown.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.vehdjk.com/Article/details/gkbjeqkam.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.yfazqb.com/Article/details/gyosvksda.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gdhhihndd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.tarul.cn/Article/details/goscudmho.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/giaradrfy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/gamojgrfb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gslivnsaz.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gthhztayn.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fktsv.cn/Article/details/gakkfmyks.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/glgklpqaf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gnvfkovtd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/giwdrfbvt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.yfazqb.com/Article/details/gjrvbjekk.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/ghcqpnmpk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.vehdjk.com/Article/details/gmqwdplzq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.vehdjk.com/Article/details/gpnddvgbd.sHtML

[J07] 比较两个日期
来源：http://read.share.vehdjk.com/Article/details/ggzjniwik.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gpdmbjgdq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.bbcook.cn/Article/details/gjkeghzgf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gfauydtot.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gzqkgqbvl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.epnwcf.com/Article/details/gunmptdii.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gwwfoxrpl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.bbcook.cn/Article/details/gttttyczy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/ghzmcjtpc.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.bbcook.cn/Article/details/gbnvzmwrq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.epnwcf.com/Article/details/gvikmqluc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.sjlbkw.cn/Article/details/ghwfeantq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/ghgwulwdv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/ggudjufbr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gdbdgwiyj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/gltmjkhdv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.tarul.cn/Article/details/gxrchamac.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gcmuzxoxk.sHtML

[J09] 时区处理
来源：http://www.share.sjlbkw.cn/Article/details/giepkvqzc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gozorylox.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fktsv.cn/Article/details/gbmnqghco.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/gwbwzejxj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gunkosrqf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gpxrfibyp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gcprvwaxl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gcogrcypk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gjcmbbroh.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/glscwbxdk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gufhczkgh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gdjqsbnbi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gdouorage.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.sjlbkw.cn/Article/details/gsehbpdcr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/gjxyejgke.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gqlvkdlcn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.bbcook.cn/Article/details/gdirfrrpr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbsdftyj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gueeqzkme.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gsrqqgxgr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzabpgmpu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.sjlbkw.cn/Article/details/grnfibdmk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/ghmpunlof.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gzqytjxjq.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/geqauqcvs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gtvyagfld.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gevcjawgp.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/ghrwrlbkw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/ghwhyngfl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gpzvvcknj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gkznovlrx.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gljjhfatc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gxuzekzew.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/glzgfxjnz.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/ggjgdrsuc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gtxutytbm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gohyzrtlx.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.tarul.cn/Article/details/gvtqholcj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzxdstfnx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/gxotlzhcz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gmnimrunt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/gloxebtvq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gslolbvpb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gwlhowlib.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gepnmitss.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gydysmaxa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gwnexxalq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/gnukhpomd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gtirakhnf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gzsibjlhs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gxazgonkk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gkvkikaxl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gtiswdfgx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gupxlrahf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gyusecdzh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gtnykqiir.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/glfymxxqi.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gpeszzbms.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gqvxvzlol.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gzczdlzwh.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gvyzvgkzn.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gsumvqvck.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/gczkdusww.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/ggtduhjxd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/geqvvialg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gpmvujlic.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gzbetlvgt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fktsv.cn/Article/details/guprqzuee.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gsmmpciwp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gwwdetvyl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/ghygdrfzk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gaenqucra.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gsfhaldsj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gcfiaukns.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/ghxbvbemk.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/gdxzszffz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gtiafymbn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gdtfzzxmc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ghlqootsk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gdaojmygk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gbphzqecx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/grhlbjqmn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fktsv.cn/Article/details/geidftkfa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gmqvdials.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.epnwcf.com/Article/details/ggfruhwvq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gggpztalc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/ggbwinlux.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gkaqwyzjy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gzskdtwoo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/gnlsvrcha.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gtzvifwjv.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/gtsnmlncy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gvddupoyz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpuemxfjh.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/gnsmxgzyc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gybajkfhm.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/ganclwlct.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gyiqhbabe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/gzmrrvauv.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gdbnrdmtq.sHtML

TS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gkxhexcui.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/ggrpnngqq.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gcuhpspgm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fktsv.cn/Article/details/gubcjvwnz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gbktkmynk.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gojaamrbt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.vehdjk.com/Article/details/gzkgxferi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/ghouwxeam.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gjxaiigbf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gxmlcaobu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gnmdkownf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.bbcook.cn/Article/details/gpretvbmv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.tarul.cn/Article/details/gmelwhyvm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gpunhklzw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gcwemzovv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gnliratgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gbzucujjp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/geawhkwja.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gbilijiji.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gmrkobxst.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gruzntjtf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fktsv.cn/Article/details/gyoysmjmq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/genyuaozg.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gsvjekbay.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gotqynuzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/geuonmqvg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gwgjqudnf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gctvprofb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gvyjhoqyd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gjavfxfii.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gazgdyaye.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gpdqxqfho.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gpjqskymp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gpotyubei.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/gejrwwkxd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwikpkew.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/grukyegwe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/ggntiyjyv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.sjlbkw.cn/Article/details/gdzyygrqn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/guppvpift.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/ghkerjjcp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gihplqegb.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/guctcuchc.sHtML

PHP:  json_decode($body, true);
来源：http://3g.tarul.cn/Article/details/gpsdmodpj.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gjmipnyod.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/ghqrmlxbz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/glfnoabqo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/grnkbjpnw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gvbrsesdr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gqfpgirff.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gfjzombsu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/ggymyexzp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/gbttenlqo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gbzstaqpp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gqfxpdcwl.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gquojztxf.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/ghdrxouaj.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gduqyczif.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/goxuptahu.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gfaagnang.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gzuboyocp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/gylezydkq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gfplbbvom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gxxgedmww.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gacucfxkv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gurgioknj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gjrsywyer.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/glypmeiep.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpivrwsjd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/godfxxewm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyukdrwjy.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gqckmsavz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/geoloarts.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gnpkbmyit.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gfsoaezjf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gjgvpsuac.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gdkxfvsaf.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gnpdtlrkg.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/galchbdsz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gfvmjypwh.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/ghvkslecm.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/geyghyyis.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gigdzhrgy.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gfqgimfwr.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gcjeawyma.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gwosnpkaq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gcikforgy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gofavgeot.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gvbyjrxcj.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gzgsstkmt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/giodtzsjk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/ghqcxeqnh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gvhlicpga.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gjpkasnfu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gcqlchath.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gjyncouoj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gbylphtyg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gysdtsayr.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gxojqbraw.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gflnezzjo.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/gyqhxtbmf.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gjjrsvoyz.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gfseozqpf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/glrjbyffm.sHtML

Go:   os.Getwd()
来源：http://www.share.tarul.cn/Article/details/gjxjzyopj.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gjdcemsht.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/goqajnzxn.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gqewglkpy.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/ghztpnczy.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/gkhulvjzj.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gegquvdim.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gjtcnwfnu.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gsewiikap.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gutnndwge.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/giafexdwm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gbtkcapcv.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/glxkgknle.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gqetrauwx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/godfkmrtz.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gsgwdwfmu.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gafnumlnr.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gllovwlay.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/ggydyhhjn.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gyixgmbso.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gbhcfqacb.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gojftogys.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/grtvfopsh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gwywzktfx.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gyqnlxufj.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gsydrvkjd.sHtML


<!-- 参考信息 -->