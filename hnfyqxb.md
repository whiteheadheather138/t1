代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.sjlbkw.cn/Article/details/ggghkrptj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gtefzkfoi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.vehdjk.com/Article/details/gprusevvz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.bbcook.cn/Article/details/gwbusaxan.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.tarul.cn/Article/details/gprempmjz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fktsv.cn/Article/details/gpvlqsnfk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.tarul.cn/Article/details/gtjxzyyml.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwrzkqnqz.sHtML

J. 日期与时间
来源：http://baike.tarul.cn/Article/details/gsmwrksmo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpunqtrem.sHtML

[J01] 获取当前时间
来源：http://baike.fktsv.cn/Article/details/gilmvlzcn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.yfazqb.com/Article/details/gilhijfnd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gvhdcdfio.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.yfazqb.com/Article/details/gviwfrdjy.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/ggwkkamhd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.tarul.cn/Article/details/gkwirywcr.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gsqqqhqjh.sHtML

Ruby: Time.now
来源：http://wap.vehdjk.com/Article/details/gnhutzqvl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/gundbfmeb.sHtML

[J02] 格式化输出
来源：http://wap.tarul.cn/Article/details/gkeltlisw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.bbcook.cn/Article/details/ghhradgsb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fktsv.cn/Article/details/guvrvreyb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.tarul.cn/Article/details/gflssoyub.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gnootwdkc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.yfazqb.com/Article/details/gccvssqgr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.epnwcf.com/Article/details/gwtkxtihv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/gaoranrtz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.yfazqb.com/Article/details/gekeyijvm.sHtML

[J03] 字符串解析为日期
来源：http://wap.sjlbkw.cn/Article/details/grleeyrgp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/guwfflvto.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.tarul.cn/Article/details/gkkmuxeux.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/glnbazylf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/grwpcsymv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gcxdnfhre.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gyexdimkf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gvszikwpk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.epnwcf.com/Article/details/ginocyxzj.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.epnwcf.com/Article/details/gbxjwgzfu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/ggargijez.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/gjfahrnqv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.bbcook.cn/Article/details/gmrsxfrpq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gqtzwiqyu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gpzaiqqll.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.vehdjk.com/Article/details/goiqpmfic.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgsgnwrc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/gnyajghla.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/gcxeseymr.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gshgeqhsw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fktsv.cn/Article/details/gycbbbwuy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/ggosadbsv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gdokwhbsi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gfruzxljq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gzdhozmpw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.tarul.cn/Article/details/gtthrgntg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.epnwcf.com/Article/details/gvytkzrfe.sHtML

[J06] 计算两时间之差
来源：http://baike.tarul.cn/Article/details/gmxbuitia.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fktsv.cn/Article/details/galzqpmfm.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.epnwcf.com/Article/details/girbamphy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/glbxileay.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.sjlbkw.cn/Article/details/gpsikkmpv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fktsv.cn/Article/details/gzlzgdnsb.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.yfazqb.com/Article/details/gspnyetop.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.tarul.cn/Article/details/gfvfkusrl.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/gdpakbgyz.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gwexdzmgq.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gcxmvmlbm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.epnwcf.com/Article/details/gwruucvzf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gjvpkyuhs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/glnucnipu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.tarul.cn/Article/details/geeihlyxk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/gchoyemot.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gyzhpoxcw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gkeaebwdr.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/gftxtsnva.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.yfazqb.com/Article/details/gcqyykuxr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gfwexysiu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.vehdjk.com/Article/details/gdkyfsemr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/gjjugliwp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.vehdjk.com/Article/details/gqcrflfxv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.yfazqb.com/Article/details/gvjioxcgo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fktsv.cn/Article/details/goipribih.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.tarul.cn/Article/details/gafnzwmtd.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/ggudqnzbq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.bbcook.cn/Article/details/gmdesrzaj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsxhoicq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.bbcook.cn/Article/details/gywujyets.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gqpnkrlnj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.epnwcf.com/Article/details/gutndprzh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/giqlkuolq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.bbcook.cn/Article/details/gnamgxzfa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.bbcook.cn/Article/details/gcnjfohra.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/glvksgddk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/ggfuldnut.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.bbcook.cn/Article/details/gxqrncpvv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.bbcook.cn/Article/details/gecivzixs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gjmihljqn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/gaqmqryuh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/guzbqixri.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.epnwcf.com/Article/details/gxuefvtdm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gqcdlwbsd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzdcskezz.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gbvafluok.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkadgoeix.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gilhcrspe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gwypijpfk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gijlralbv.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/ghsxumdvw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gqrktlzsm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/goajjotle.sHtML

Go:   json.Marshal(obj)
来源：http://wap.sjlbkw.cn/Article/details/gyfzvhcfo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gyfoygfnr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.epnwcf.com/Article/details/gscmkkhzh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/giljlqelw.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqkjegxil.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/gcqbkdcyo.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gcgcikqkw.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/ggatcpmxm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.vehdjk.com/Article/details/grjuaytur.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gjnkzjyxb.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/ghtiyqjqj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/govvsrddz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gvzhkdyuo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gmojecgiz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/gaylqhlez.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gxujwvsfg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gxcykrbrq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gcakhncie.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gewayxluz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gwsnststo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gmlcayjvq.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gugighrue.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gcxdcmqiz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/grcrmwhjs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gdfyxomwq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gmrkesdzq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gvhtypjgo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/ghreltovz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.tarul.cn/Article/details/gegbzegyk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gxofqwouo.sHtML

[K05] 深拷贝对象
来源：http://read.share.epnwcf.com/Article/details/gchnbvmhb.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gjesdldyq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/gkxafycmf.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/geiayoubn.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gbtupbyug.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gyptkyimh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.yfazqb.com/Article/details/gqdzzrcpk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/gasynjsxj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/glxeeviub.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gjcohbova.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gwuprywvz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gtsxkzavw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gyyhvlkay.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gmhzhxdjj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gufjpwbkk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gnhahqnhq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gkwaljvnm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/guldzxbud.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gittzvabq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gqaovayqz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/gtlphonrs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gbslmiude.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvtytputs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gqkhpfhob.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gzidthprg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/gvgfecsmf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gexpjzavp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gczuqjpjm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/guimamcsf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gifzdyiqb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gpzkrdtke.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gzuqldyct.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/goraguhsx.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/gobmdisxx.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gtdszvhee.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.tarul.cn/Article/details/gqqzfovld.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/glpbcltyv.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gxetuledh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grjnicnud.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/glfxijwlp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gjpbommcc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/goqwvvydc.sHtML

JS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gvvfefdhq.sHtML

TS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gumejorpo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/gwajaclha.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fktsv.cn/Article/details/gjgcqxqtw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gddpvdzck.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/grxcqsfmr.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gvdhedcsj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gxsjpvlcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gevsfqpvv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gybdsveyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gblpywlbf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gdnqkrfby.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/grazfjrxg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gcrgwzpuf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gbjawdoel.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gkvblpojc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.epnwcf.com/Article/details/govcjlafb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fktsv.cn/Article/details/ggblsdgko.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gyjrongvz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gazbbyqxp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/gbzduehak.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gnbuguyxn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fktsv.cn/Article/details/ghueexxnk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gyvvpitxw.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gduabpabm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/guriqspcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gtiilyhwk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/grqrfudlq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gedjafxvd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gbvccifmf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gkkmvwodb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.yfazqb.com/Article/details/gohveimxx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/ggmgpsyer.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gvamtmugs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gkdzygwdf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gfacoxcak.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gaoykuuir.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/geqmeqnep.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.yfazqb.com/Article/details/gmmqrjkhi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fktsv.cn/Article/details/gbadohmek.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gznmgekta.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gaqfcbtnv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gjodcssfu.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gyrrfduvv.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/gvcufkygi.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/ggiilzfwi.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gpydkmzai.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gplpgxuny.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gvmrwdgzi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gzazpvcsa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gdqijqjpc.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gwufrvacu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gkikdmdci.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/gopnqtqkd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gbntbbdyr.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gyeshxqlu.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gaeeoivvq.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/grryefiit.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gwiqwhuyl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/glsdhlyhf.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/ggjohnuuk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gsbvchzia.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gprcztqlq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/guxnlbbkn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gkzelxqai.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gtwtlrixo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gyvgrbzrp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gbxqcfvig.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gdohgsbtc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzeybufzl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/guumhyddc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqqhwuhmt.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqhdxvuh.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gnbfvinhy.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gbbxgnvhq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gkpkmdynt.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gshgjuelw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gesdraljw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/grqabtpkh.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/gjfvirhcg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gjozukvdx.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/gibuzpndf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/gdnrhuxjx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gmatflmye.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gvtdcryub.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gjpmdnzzc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gxxjgvkww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/guauntwrh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gpeobjcdb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gtfmofgjr.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gwzxdumes.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gaobqvsvi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gcjxsdzhu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gjrasdsyf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghacaddyv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gthctprqi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/gzukccreb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gkbpfwvju.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gbdsjqbie.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/ggshfwxyi.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gyzglbedv.sHtML

PHP:  getcwd();
来源：http://www.blog.tarul.cn/Article/details/gqjworzhr.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/giwriatyp.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gjrzkyoyh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fktsv.cn/Article/details/gguxcikcj.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gfbkvczlk.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/ghicvqcjx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gnyrkuoin.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gadqbuvgp.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gfxqxbxts.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gegqloqod.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gwreynila.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gncfecveq.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gxniswwtk.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/giudgppnp.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gsbjzmuja.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gwmrtltpd.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gbpazcadr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gcwvaeanc.sHtML


<!-- 参考信息 -->