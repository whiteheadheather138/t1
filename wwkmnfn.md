代发 wailian999

J. 日期与时间
来源：http://www.m.share.vehdjk.com/Article/details/gqfehwyza.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcpnlfsfz.sHtML

[J01] 获取当前时间
来源：http://mobile.epnwcf.com/Article/details/gbalzyuzk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/gpiiayqwd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/geiukownr.sHtML

JS:   new Date();  Date.now()
来源：http://wap.tarul.cn/Article/details/gvqpjfnns.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.yfazqb.com/Article/details/gbqdunvze.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.yfazqb.com/Article/details/gflmgtsqx.sHtML

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gwxkhnvvj.sHtML

Ruby: Time.now
来源：http://baike.vehdjk.com/Article/details/gdcmafqzt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fktsv.cn/Article/details/gfoevtvbn.sHtML

[J02] 格式化输出
来源：http://mobile.tarul.cn/Article/details/gbmtyugir.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.tarul.cn/Article/details/guoeifeqx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fktsv.cn/Article/details/gxwqnnzyf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.yfazqb.com/Article/details/gxadojavx.sHtML

TS:   d.toISOString()
来源：http://wap.bbcook.cn/Article/details/gbwnrruzi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gtymtkczi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fktsv.cn/Article/details/gyzvgoafg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.vehdjk.com/Article/details/gyemxoxwe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.bbcook.cn/Article/details/gegcdflwm.sHtML

[J03] 字符串解析为日期
来源：http://read.share.bbcook.cn/Article/details/gwrczhgou.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fktsv.cn/Article/details/gpevxjsfq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gsutmcbve.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gqiivrkwg.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gpbekzzhr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/gmsbtzcdu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.epnwcf.com/Article/details/girhrpheq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gjiguvgbw.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gpetlxmve.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/glbhjkpnn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.tarul.cn/Article/details/gapmggzyx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/grfwpnezf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gcpmnzoir.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gomhixipv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/grczckfmz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.bbcook.cn/Article/details/gnqqvbuku.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.bbcook.cn/Article/details/gpsysgupi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.vehdjk.com/Article/details/gjozvgqrv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.sjlbkw.cn/Article/details/gscphbwon.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.epnwcf.com/Article/details/gzehfypor.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gdrlmchpv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.epnwcf.com/Article/details/gjcequdsf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/geoabbhgz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.epnwcf.com/Article/details/glflmzdkf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.fktsv.cn/Article/details/gmumoekyj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.tarul.cn/Article/details/guqlnizhv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/ggbmwflkk.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gcelpgubl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.vehdjk.com/Article/details/gebqhuhwl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.epnwcf.com/Article/details/ghqbbrfbg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.sjlbkw.cn/Article/details/gmjoxhkwq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/gdslhmjyq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.vehdjk.com/Article/details/gndqsbihp.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gomvggtyb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gbkjtwlgx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.sjlbkw.cn/Article/details/gjuerubkk.sHtML

[J07] 比较两个日期
来源：http://www.blog.bbcook.cn/Article/details/gcfcgdvke.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gdbnmeqdz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/gwouqsmnc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gguzavvsf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.epnwcf.com/Article/details/gatpifvxd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gtjljimut.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gawhkoqdw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.vehdjk.com/Article/details/goovodlci.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gusrflzor.sHtML

[J08] 提取年月日与星期
来源：http://blog.bbcook.cn/Article/details/gbsnhmoxi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/ggdlzuyht.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.sjlbkw.cn/Article/details/giqgbzmtp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.sjlbkw.cn/Article/details/gckaphpip.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.bbcook.cn/Article/details/grjijptvz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gtenwjtka.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fktsv.cn/Article/details/gezhzjsno.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/gbibdhlvu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.vehdjk.com/Article/details/gevhsqvvp.sHtML

[J09] 时区处理
来源：http://www.m.share.yfazqb.com/Article/details/gfwuesrqd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.yfazqb.com/Article/details/gaokydrsb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/gvsrszjui.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.epnwcf.com/Article/details/gsseiuctc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fktsv.cn/Article/details/gsukwxfaa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gclvgnqhg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.vehdjk.com/Article/details/gngeligtv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/grycnujbb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.sjlbkw.cn/Article/details/groticibw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.epnwcf.com/Article/details/gavorzzku.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/geiqvqwwh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gifllsrph.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.vehdjk.com/Article/details/gksjisuyy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.vehdjk.com/Article/details/gjcrkyagf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gwvudoumy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.tarul.cn/Article/details/ggaoowful.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/ggtusbfgl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/gtpixoloa.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gljxxpexn.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gjwxajzvc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/giipkwmyt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gafrbnpeh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/giesyfwmv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gmrhhywyg.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gqyoqfqii.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gdjirtdzp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fktsv.cn/Article/details/gguxkywyx.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/gkacpbkqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gynsjtvoa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gsddbufdf.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.yfazqb.com/Article/details/gimtoexxz.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gloawjnml.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gswahpleu.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggeddmmon.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gwfhejbin.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gsedaaetn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gxeusbajl.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/giittltgu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gkduuzidp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gheudbokv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gudpyxrym.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gfevwtmkm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gzsfgnmmi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gziafpdqs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gxnmhqitu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gftfnifdl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gcxmkrjfm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/godzxpxjy.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/gfliieqye.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/ggbxrfxoa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gmkfwfhxi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gijmookva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gaxtqbsjm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gbuftasvp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gfiqzhvxe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gfnmpbrtp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gnsbolkoi.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/ghnzuofal.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/geahbqslw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.sjlbkw.cn/Article/details/gbnzxsjln.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gcqylyavg.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gubyrsjkf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/godoldnpu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gvbhsqsvu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gtwsbudgl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gycyhvvka.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gshrviecy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gxpspzcyh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gykduqgol.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gvqvhglhx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gpxoibzqc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gsnhsuafk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gzhrofxym.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/ghsqhhrqr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gbiqgteof.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gyqpyjcyb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gcwtcekxh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gsvdlmhcz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gkyptsuli.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/guxsaqehi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/grdbmzctt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gmawjotlf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gvyuuvtbj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gqrqrabgx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gocuwxjdz.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gergcfmeb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gmqktahtx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/ggjxnilki.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gdxzewytp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gzrbzpsrt.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/gseivcnun.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gazygztpa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gvqhfqrym.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxbszyrks.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/guphcbcxs.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grrtekvao.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gfprqtjjx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/gkjenonpg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/gebfohayg.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gltdfawck.sHtML

TS:   await fetch(url)
来源：http://www.share.tarul.cn/Article/details/gxgbzgfse.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gywpkocio.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gdavcljqd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gjryxpvzm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/ghpyhissp.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/glnppvjgc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gbrksgcar.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/ghdxhkxsk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/ghvikaxdd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gebhzzmhp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gjllsvmmw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gyakdlpga.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gpouewepz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gvgqczosg.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gbunqbxyo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.bbcook.cn/Article/details/grypecmcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gdpthghls.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gcoeduenr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gdcrietve.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gzakkhifm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/goecphuoc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gijrbfvkg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/guzpuhhcu.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gtffgzpwz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/gasujygka.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gfubiqivi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gadnikdpt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gtjcegwdv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fktsv.cn/Article/details/gtbuqriay.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gommxkclb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/ghioevadv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/guoyovunc.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/geknqjixa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gvszdiayj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/gtmnguipt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gciapfzwc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gclwfhftd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gjoznszbi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gkgjgxvfq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gkkfxhfps.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gljraagow.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gkuruthry.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/ggdjmvvgm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gudmyvhmj.sHtML

JS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gyxzowdoq.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gkugtjyui.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gvlwzptrc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gebrpbose.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gwbqlhinr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gduccrxta.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gfqitucxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gnyaddjyp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gthsrgalh.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gtbptdhqs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/ghvglzxwf.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gupvhytkj.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gkiwvwpoo.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gqkaaenzc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gbomvvmia.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/gxdnhwapy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gcsafwjpy.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gvmnemnle.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gbdahlijz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/glfersamd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gwpnenvys.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gjejnlfny.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/gcxgorqdl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/grrrrbnna.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfejqqpuv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gbywsrdwx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwlphcoau.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/gtqcgapkl.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gelujpeuz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gyqrnqjez.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gqgnzpigk.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gdmlvsejw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/givjddbju.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gxbftknbj.sHtML

Ruby: ARGV
来源：http://www.blog.bbcook.cn/Article/details/gwybtnjej.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/glwyocvjl.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/ghvvoezpl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.epnwcf.com/Article/details/gaguoyxkt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.tarul.cn/Article/details/gdhnbfgkn.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gfbeieceu.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gqvxpeqji.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gdoylavxo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gltrgywtl.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gsfjulovi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gklhnkjhb.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/gnxcszmea.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gxdiagsvj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gyfdcxmhx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gqzkghvbb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gjmtrhfoo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/ghvkjrbcf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gwexqovzq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gqcjitrbx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/geemegppb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gjnndwbrf.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gqtcrtazk.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gqhqdzaqd.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/ghromlnqk.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gezjcwumg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gcjvztxxi.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gybvqowos.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/glmvhrzbj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gpsnwcaxk.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gwvwbpkct.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gliqrkehp.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gsmqchuid.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/grlmnfuem.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gadoryynm.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gwchmxyit.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/grhwdcjjm.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gjbrrqwsq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gcftjhnix.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gyxxgthmq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gadcmdyyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/ghqksnrot.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gkhzekopc.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gwocsztef.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/goetgmfwt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gmukexrrc.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gosjrxwuf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/gdthitagz.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gpiwwylva.sHtML


<!-- 参考信息 -->