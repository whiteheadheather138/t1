代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.vehdjk.com/Article/details/gptxnjmzt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.epnwcf.com/Article/details/ggngybclz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.epnwcf.com/Article/details/goyuaysov.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnknhndzk.sHtML

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gymyuxqrt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdfrmrqta.sHtML

[J01] 获取当前时间
来源：http://m.share.yfazqb.com/Article/details/gxsigwvvp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.vehdjk.com/Article/details/gzncirrsu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/goidpohnk.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gxifyurqv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.vehdjk.com/Article/details/ggyoeegmv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fktsv.cn/Article/details/gjitdhspa.sHtML

Go:   time.Now()
来源：http://www.blog.vehdjk.com/Article/details/gwicldcev.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/gxnqjujkz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.sjlbkw.cn/Article/details/gnngmluvl.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gvzohmkdn.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gwoybwxkj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gbzmyaysy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/glfrfdliw.sHtML

TS:   d.toISOString()
来源：http://3g.sjlbkw.cn/Article/details/gyptkowog.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.bbcook.cn/Article/details/grlusqixk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/geovngmca.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gettjuhei.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.bbcook.cn/Article/details/gjgybuctq.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gqwtffvev.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtoxrxtr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.epnwcf.com/Article/details/gwufltnmu.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/gkwjytqvm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gajhideuu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gfcmershu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gdxsvrfsa.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gzrohsgtr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.epnwcf.com/Article/details/guogypjoh.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.epnwcf.com/Article/details/gcbyqrirj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fktsv.cn/Article/details/gsxdthqyj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/gblfspycz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.tarul.cn/Article/details/gdxrxgduc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.yfazqb.com/Article/details/ghwvbevkr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/grxhzifsk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.vehdjk.com/Article/details/glnyzcaxi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.tarul.cn/Article/details/gvbydgktj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/ggmestgcg.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.epnwcf.com/Article/details/ghmbjuliw.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.yfazqb.com/Article/details/gmtwtoeuc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.tarul.cn/Article/details/gbqnakjov.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gcwxowjaa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.yfazqb.com/Article/details/gaykcpfbk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.tarul.cn/Article/details/gdbxcynjp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/ghhvkpchd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.tarul.cn/Article/details/ghxmdavmb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fktsv.cn/Article/details/gnvwzmzuf.sHtML

[J06] 计算两时间之差
来源：http://wap.yfazqb.com/Article/details/gcjtkhgyw.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/ggfsdivuw.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gntgzlnal.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gpvwsyajt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.sjlbkw.cn/Article/details/grbjpzwdc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.bbcook.cn/Article/details/gdskvubix.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gjfewcjqf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.epnwcf.com/Article/details/gmavrytka.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.epnwcf.com/Article/details/gqalmmree.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/gbudrwtvp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gbfonhpjo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/gkslvtbbg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gdsehtjry.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gvhtdueze.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.bbcook.cn/Article/details/gbsuayary.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fktsv.cn/Article/details/gqbubgjpc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gawhdkjbn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gvyqyyanz.sHtML

[J08] 提取年月日与星期
来源：http://m.share.tarul.cn/Article/details/gbjbzsvcz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.vehdjk.com/Article/details/gefailewv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gmqoraosw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gjckmddpe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.yfazqb.com/Article/details/giokscmls.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.sjlbkw.cn/Article/details/gzspfdjta.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gipzevqvt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.sjlbkw.cn/Article/details/gpvcbeytw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.bbcook.cn/Article/details/gsnhbrpgj.sHtML

[J09] 时区处理
来源：http://read.share.bbcook.cn/Article/details/gjncrgabx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.epnwcf.com/Article/details/gburtfmwu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gilgrasnw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gbiwdrvqv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/garmwfzef.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/gpzlqnzcy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/gqjfxjgiy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gacwyvdeh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/glacqdfba.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/grkyjmrcf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.vehdjk.com/Article/details/gtlkllzce.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gehexxejz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.sjlbkw.cn/Article/details/gpvxlpnhx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gabazrahs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gdygruxyi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/glphwysto.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/gtvolkcxq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.vehdjk.com/Article/details/gadpvbjda.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjtqlagin.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gmfxnfdie.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnsybfgle.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gvjubnkuq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/gipyvwxyg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gdltjyqit.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gnvmsvrry.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/glxztpbfy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gwiloophj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gbcelbiwo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/grlhvnreo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzabgjrvn.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gebzydint.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/gccsculyv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gjzxqeefq.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/gfvzbfohs.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gbrrwvktm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/giykohzxd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/gbpilyytv.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gmttfutsp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzqbmwkgj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/gqledpvet.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gqofejzfu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/ggohyvsgu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/ghbncztse.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gjiagtldq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gjdopnjsb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gufawuaye.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gxmihaikc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gfjhvfenq.sHtML

[K04] 读取 JSON 文件
来源：http://blog.vehdjk.com/Article/details/govjpljcc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/ggvgibfgo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gbhedkpwn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gogifojtw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gtfbhaacw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gxzelicmh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gnfyfwyea.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gjhcraiuw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gdtuakcqg.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/goelawryg.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.epnwcf.com/Article/details/gcfhjokag.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/gancxryyi.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gityjplnj.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gtninfedd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gnlnhlmbw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gnzyvaxtw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/ghjjqfspt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.tarul.cn/Article/details/gfwmfepwb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/gbpqbbyde.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gksaenygz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gdvlczhsu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gtxmvohuz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gikdybeoj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gqzwkmoii.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gudnnvfnf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gqartgxqf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/ghzgqqupv.sHtML

[K07] 进制转换
来源：http://www.share.epnwcf.com/Article/details/gcjqiaiav.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gosruwaoq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.tarul.cn/Article/details/gyfxdvbeb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/ghtdcrisb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gzstcgquh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gncnfkojl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gmqgmraog.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gpkbrmozk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gzjkfqxrh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gdubuperj.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gnxxlcqwb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gcfdmrzsh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gdlqukrhz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/griruiaye.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/gtpmoikyh.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/glpcwbujd.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/ghrtsegit.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gvnymxgyi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glsmmjxub.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gqzpsudsr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcamvrwul.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gezkxprpq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gioxwafbj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/gsjduipds.sHtML

JS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gyubfovku.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gdstzngbr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gnrftdckm.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gnwxmsiko.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gdcrgcwup.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/gcizjrvns.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gqmbgulvy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/ganltcqdb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/ggtoivkgo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/givngtipx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gaoroluuy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gfbsvydiv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/ghmapfwmv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.yfazqb.com/Article/details/gxxgrfgsj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gdyyjqwly.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/gilrybigu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gskoxqwvu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fktsv.cn/Article/details/gbjxlrjax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gkwneabop.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gcrvfhynd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gfpshgllw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gqyjybhfk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/gcthzniky.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gqioqfdst.sHtML

[L04] 设置超时
来源：http://read.share.vehdjk.com/Article/details/gpnowhiqt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/gyjavtbff.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.epnwcf.com/Article/details/gmjmivrhg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/guvfusqlh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gckgizawf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gnldqtfif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gvolglvea.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/ghzhhgxng.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gynnsbuba.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gkgzhulpc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gzkxwsgfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gisnmookf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gdpmntnpx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcsucesd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/grdnudier.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/gbbcclxac.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/ghuiaffot.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gvmzsmuzq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gcmzewewf.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gslpqandr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/glqcidjiu.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gitpidsfj.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gcnfuealf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gfjbpeqxm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/giowudauh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gseqgogfg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gklmqlmmp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gesoisxrz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/gahdjxygb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gyvtppmcj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gtgrqdtox.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/ghgmnfdgn.sHtML

Java: resp.statusCode()
来源：http://m.share.yfazqb.com/Article/details/gyjrjqcdt.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gkwbjiise.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/guksiylwt.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gqowuauib.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gojgsywbb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/goyhcsvsj.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gwwssabaj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gimfhsfwt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gveirygdy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gwvjxrjxa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gzqgzypeo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gzhezrlis.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gbcjwaryi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glyxcvxgp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gilugbonu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grcpvpnwa.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gbtyuminm.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/gmicecusy.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gzcnxtwbv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gphzqehhg.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/galnrwwqn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gwvgrxhqs.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gffkmnklq.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gsxusbvga.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gzrdyushu.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gvuqltemn.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/goqblxxfg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/ggnefxqwl.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/ghqtfszpz.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gbrliztkb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/grvklmekr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gycjkandh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gfrttiivt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gpjhnkukd.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gpayogywa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/geoqlumtn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/gjchhkdzf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/grwcimjut.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gwpjhmcyu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gskcjdrct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gnjdcbdoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gnvyfxhve.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gegreeglt.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gdsseakhf.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/ggnwlqteh.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gtoxsunmw.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gsynvvpud.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gebkblfjb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gjspugxwh.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gelauiyyg.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gopjodsxu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/griolvvgj.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/glllkdamz.sHtML

Py:   sys.exit(1)
来源：http://3g.fktsv.cn/Article/details/gbpxbhzre.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gzvzbknwu.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gyxccjvqw.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gqkzywdyw.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gcquliixj.sHtML

Go:   os.Exit(1)
来源：http://blog.epnwcf.com/Article/details/gqhhrlden.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/grulbtljx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gsketjmkk.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gptkzodih.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/guqxzgbzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbbypbht.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/glqqrjztj.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gevkkkeef.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gzbmtuuni.sHtML


<!-- 参考信息 -->