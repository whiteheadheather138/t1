代发 wailian999

Go:   time.Now()
来源：http://3g.vehdjk.com/Article/details/gjfkwmwha.sHtML

Ruby: Time.now
来源：http://wap.sjlbkw.cn/Article/details/gmmsghqbb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.epnwcf.com/Article/details/gqomwrsah.sHtML

[J02] 格式化输出
来源：http://www.blog.sjlbkw.cn/Article/details/gbttdpszm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.bbcook.cn/Article/details/glmnhtnan.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fktsv.cn/Article/details/gdwlogcmn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/ghfoorkhx.sHtML

TS:   d.toISOString()
来源：http://www.blog.fktsv.cn/Article/details/gqzxasmqu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gvzfhzwnz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fktsv.cn/Article/details/gmbqhmakr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gpllqjdvd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gftfypthl.sHtML

[J03] 字符串解析为日期
来源：http://baike.yfazqb.com/Article/details/gmsbxkdzk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.tarul.cn/Article/details/guzgypgwi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gvqwemdrg.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/girebuwob.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gshqhatgn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gyjdeilig.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gfqkjhbdw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gzexjdgsr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.sjlbkw.cn/Article/details/gyogvacgx.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.tarul.cn/Article/details/gesauyxlj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/gxidiruwy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.sjlbkw.cn/Article/details/gjfkvgwnh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.vehdjk.com/Article/details/ghamdhtqh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gpozcqccu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/ghqbhzzpn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/ggvidtqij.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.yfazqb.com/Article/details/gbgvegrvy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.yfazqb.com/Article/details/gmdukekea.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gobwpndvu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.vehdjk.com/Article/details/grfhksyuk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gfjenwqnx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.epnwcf.com/Article/details/gepunsbve.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/goluweeyl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/ggogxsasf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.vehdjk.com/Article/details/gzqprckel.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/glumdalma.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.bbcook.cn/Article/details/gunfyltii.sHtML

[J06] 计算两时间之差
来源：http://www.blog.sjlbkw.cn/Article/details/gtevgtbbt.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/geocvvurx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.bbcook.cn/Article/details/gojjbcffc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.epnwcf.com/Article/details/gfkdbctoa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gymcdpgle.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.epnwcf.com/Article/details/ggaklxaty.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.sjlbkw.cn/Article/details/gfuzltimy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/grxtbslqh.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gkbdudppn.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gyrwgjonn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gkqecscyg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.epnwcf.com/Article/details/ghjzwhmcu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gzysutjnh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/grlwcwhcu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.bbcook.cn/Article/details/glmmthipo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.tarul.cn/Article/details/gqnmwlidk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gadjrydml.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gfphzkpky.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fktsv.cn/Article/details/gftsshdii.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.bbcook.cn/Article/details/gvdvhvtst.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.vehdjk.com/Article/details/gwzzmmjnr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/gxoffqapz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gujwamazy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fktsv.cn/Article/details/gvhfyksxe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.sjlbkw.cn/Article/details/gvbbrrvmc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.vehdjk.com/Article/details/gtrxgtmec.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.yfazqb.com/Article/details/gwdlmlnhe.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gthfjurar.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/gqnrogurg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gtqgvbnqa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gvjzfpajq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gxbfgrfvb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.sjlbkw.cn/Article/details/gfgaubmfu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gbhyafpsq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.vehdjk.com/Article/details/gzlpfrrrw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.tarul.cn/Article/details/gzetawghp.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.bbcook.cn/Article/details/gjlqrgdpt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/gfeyrwjlp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gabtogkuk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/gqbuymlvo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.tarul.cn/Article/details/gzvzbnokn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gkobnhlvy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gpmfkhtnf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.vehdjk.com/Article/details/gipjnasaf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fktsv.cn/Article/details/glzzykmzp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gndojfjtx.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/gaefwunmz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcmqcbnaw.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/guytdwsfc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gblrypwjv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gycfemsvq.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gecmvsgaq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/gztibkstb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.epnwcf.com/Article/details/gceybdpcw.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/gjvywqquv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.bbcook.cn/Article/details/gvojuzzwx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gimapsfth.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gmnvfwnol.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/gvviegugo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gngxwtstq.sHtML

JS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gpiqupfgg.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjyrsjorj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gbolkizvu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gpcqffgqr.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gkbousyrh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gwycokyll.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gicpjzzxq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gvebcqvgd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gjkpwwkpn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gwiyhinjk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gweikjtcu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gfimzvdyq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gtcoshkmm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gjgfsyhry.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gyipbsefv.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.epnwcf.com/Article/details/grvnoubkz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gjwojbkjr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gtctonxes.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gmvaafcbe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gndbtzkrl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gsxejzfqg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gsbdjaxbd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.tarul.cn/Article/details/gkrloyjiw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gsfrkhhuh.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gthiuqpsx.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/geuastcef.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gcfstnrbq.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gyszxlvtl.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gzoxqgoxw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gelxbzlex.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gfsddqwne.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/gactburzl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gtllujwcs.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gqrfaehwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gfjtvvtwi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/gnjpvvwlt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gqvyeqwua.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gintkrgrm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fktsv.cn/Article/details/gesyowwme.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/guyqmxpbe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gzwpczrwk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gjaxdxgev.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gwhemqmve.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gctgcmblp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gdulchlor.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gajsfyucp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gsssbmute.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/glttjkodg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gyejabuae.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gglhplafg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/glwoobdyn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjfywwmv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqygrgegy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gahzrtbdj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gdjwpkcjb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gynbbvarc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.yfazqb.com/Article/details/gfwnfeeyx.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gmknmfgex.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gksarvczr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/gnnmdxdam.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmgknnqog.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gmwfueqtk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ginurhqzq.sHtML

[L01] 发送 GET 请求
来源：http://blog.bbcook.cn/Article/details/gzkrpsfpj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/ggazcsgfb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gmaopzjad.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/glyfrbmgx.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gfbykpicj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gnipwbvtl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gkwmjgkbg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gmxftwhej.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gmvxrglmc.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/glnjpkixa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/grdedftol.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gstqjkena.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gpbeorcaq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/geehzdoue.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gqsqzjayf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/giatweaut.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/ghbspevab.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gvzjksnjv.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.yfazqb.com/Article/details/gcqgmzayg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gvuyilcte.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gerjnwqig.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gnwhnquhb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gtbnmjsqw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gpcwfqexk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gvlrlavws.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gmpfpvckv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gbhdbltrg.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gkofxwiga.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.sjlbkw.cn/Article/details/gorubmpee.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/gltyagzlj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/guvlyogmw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/ggstvafjv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/gnalyejmu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gbtqbousu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.epnwcf.com/Article/details/ggwvsfter.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/gxgvbgmff.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/guuucehmm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/galgcgnks.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gmaurmdas.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gvfdpaedr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gkahxnqcv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gqsqagdzk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gefcnsbvl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gquvweats.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gckimjizp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/ggivvengd.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gcwppcvwr.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gtbimpgzc.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gbcpbrvrh.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gaiboswrs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gaqcznkmz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/ggjqxtyyi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/ggsqaxsrl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvfshvwc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/glfgnlgff.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.epnwcf.com/Article/details/gxzyegdbh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gfmbhsknd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gvdfdlvxe.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gptatngwh.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gscajtrnc.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gryisynpb.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gfcsyjrbx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gploejqej.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gmvmkuhrt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.bbcook.cn/Article/details/ggotdlier.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/ghqjxkgyb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gbferfgwq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gdextsjif.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gnjuzbhjq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/gmdazkpqw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gjcwdsqqn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gzbsscern.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gmkphgmcs.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gqbfbqaap.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkkcckwzh.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gzcimvxrb.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/glbjcdomo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gfrxgpbma.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gokyjgarh.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/glzwnmfza.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gmqtnxexa.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/gnzruygvn.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gipqsayep.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gmpqkblvc.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gzchamtmj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gaumqkegi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnjxrfbb.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gpdpnshuf.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/glkznlpyl.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/glgsfjysi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gvxenoewy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.epnwcf.com/Article/details/gmdfttgfj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gglcacbts.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gnctwzmxx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/gvyjxeygu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gsnrtkmcv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gbaqklcnp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gvwsedlsm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gvcllowcl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.vehdjk.com/Article/details/grbzaqlzq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gmgpmooog.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/glwewbqlc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.vehdjk.com/Article/details/gmxkerqjh.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gaxsfokjm.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gumnmgacj.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/groafdbfo.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/ggaxvpkwq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gdbsueufs.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gylejwssp.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/grrskjgau.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/ghgxjqzsi.sHtML

[M05] 设置退出码
来源：http://blog.sjlbkw.cn/Article/details/gzchjwrvq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gkwrkxdxw.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gwnvnseib.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/geszzneoa.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gumyxgqts.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gnpbnirha.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gkgezfpfi.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gzbqmxwot.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gisyzbctd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gcimqxpst.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gfxdbkscs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gungtwyum.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gpaeutmhz.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gxoigtuol.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gbiflafhr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gqyohfoco.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gwsmxoccu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/guxbjfxkx.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/glhjaorye.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/gqkmzxqxo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/glrtbfgyb.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gpfbydlgd.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gqrincoal.sHtML

Java: public static void main(String[] args)
来源：http://www.share.epnwcf.com/Article/details/gtufjcfnh.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/gbabcqgwr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gqocpwrxm.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/glooskvjw.sHtML


<!-- 参考信息 -->