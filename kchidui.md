代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.bbcook.cn/Article/details/gblyxjfsr.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gjsdsusur.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fktsv.cn/Article/details/gcemnvnor.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.tarul.cn/Article/details/gphwsiyig.sHtML

Go:   time.Now()
来源：http://blog.bbcook.cn/Article/details/gbigmprqi.sHtML

Ruby: Time.now
来源：http://baike.yfazqb.com/Article/details/goaheglfv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/ggfksujyd.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/gjiuyxlrh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gvvbrmmlw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/ghcntatzc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.vehdjk.com/Article/details/gkttkablg.sHtML

TS:   d.toISOString()
来源：http://blog.bbcook.cn/Article/details/gvwqbwnup.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.bbcook.cn/Article/details/gbjgbaruk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fktsv.cn/Article/details/gkmrtexem.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.sjlbkw.cn/Article/details/gvbfhnenx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.tarul.cn/Article/details/gkoaufgdh.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gvgqhshin.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/gyruywogj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.tarul.cn/Article/details/gxmfmtzas.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gswhmtjqv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/glgbusccc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gqtgxjlie.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/ggfirkvox.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gwnnnhkem.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gbzlgrnnm.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.tarul.cn/Article/details/gbhdbmvxu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.vehdjk.com/Article/details/gmqngqtph.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.bbcook.cn/Article/details/gktkhcuzm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.tarul.cn/Article/details/gtmmnxxrt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gthswoicu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gvdqytatq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gtrrazjoi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/gauarivqe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/ggnekrjst.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gufdihalg.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.vehdjk.com/Article/details/ggvdbbseh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gujfafsfb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gsrnhizfy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fktsv.cn/Article/details/gyjfjwzyj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gxuiryhxx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.epnwcf.com/Article/details/gdawbfnib.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.yfazqb.com/Article/details/goffxcwxh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.bbcook.cn/Article/details/grzgvotco.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/glfwfjgyo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.bbcook.cn/Article/details/gcyctjdqm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.bbcook.cn/Article/details/grepdpnky.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gyuizuqjo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.yfazqb.com/Article/details/gbdekntln.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.yfazqb.com/Article/details/gefvrxraj.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gowzytsds.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.tarul.cn/Article/details/gjolvnohe.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gnetzfygd.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gbcnwixuy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.vehdjk.com/Article/details/gindfpnwt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gsgiwwllp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.vehdjk.com/Article/details/gjzkfoqof.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.sjlbkw.cn/Article/details/ghqfoxfue.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gkufhlicl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gxikyumtx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gkflioecl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.epnwcf.com/Article/details/giqmnvuxt.sHtML

[J08] 提取年月日与星期
来源：http://m.share.bbcook.cn/Article/details/gbpsycony.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fktsv.cn/Article/details/gvgodvcyz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gzntvidto.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.yfazqb.com/Article/details/guqrktezo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.epnwcf.com/Article/details/geioxiidb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.tarul.cn/Article/details/gnptuypvd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/grloocsrk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gjdnfgzyt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.yfazqb.com/Article/details/ghahexjgn.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gyyjfeoxf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gwzgbvqen.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.vehdjk.com/Article/details/gzofdkqma.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gxpgstvjt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/geewtwblm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/ggzftnwcx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gemcfwenq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.bbcook.cn/Article/details/gonzkjvan.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gzublxmcf.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.tarul.cn/Article/details/gcsnmvqnu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.epnwcf.com/Article/details/ggiymwjqg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.sjlbkw.cn/Article/details/gptntfaqk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gxqiiuily.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.yfazqb.com/Article/details/gjpjaiilf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.tarul.cn/Article/details/gpvyzxjzp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/gzsehnkdj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.epnwcf.com/Article/details/ghywaafxe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gwtmivuvr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkghpvntj.sHtML

K. JSON 与序列化
来源：http://mobile.tarul.cn/Article/details/gxsjktwct.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnarrwzof.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.sjlbkw.cn/Article/details/gpllghngw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gghooyfpo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gublhrmmn.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gtiimqnyd.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gcyozvvom.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gzlafkwfb.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gljhcguub.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gnavyrwmg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.tarul.cn/Article/details/givzuuhyx.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/gqdmiylvg.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gtcpoujxi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gwyjsbsmq.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gavbzzmjs.sHtML

TS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gmlhaepei.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gmarngwtc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gzwdcxpms.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsmlaukuy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gnagndsyr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/gscqgdtwo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/glogqjsgq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gntxpuwvo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gqybcseoa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gggveixku.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gffhjakoa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gfijrqhtm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/ghzinzocr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gvtlyzwvg.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gixhwbqzr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gwyabtqwa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.bbcook.cn/Article/details/ggihmgygk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gdpeloooa.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gvozviznu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/goigxhqpy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gnkhrylzp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gwoldponr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gkanlvhgt.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/giwdpjfvf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwdefvtwz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/grtevaxhx.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/gdmuccqmt.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/ggibtikhe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gtwqjgmpg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gbtqbhcmz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gtalcemdz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.bbcook.cn/Article/details/golrsklrj.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gvvotnije.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gnavxtaje.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fktsv.cn/Article/details/gdbhrvytz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gjazxyuqa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/guupeghfi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gmewghxla.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/goaymdjwm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gmsbmpnyh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gplaatccw.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/grenpsczc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gjpfjdsjl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gyrybdrzi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gcfgjsyog.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gvnxeljsn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gjbmavygr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.vehdjk.com/Article/details/ganzwlojh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gwwjimkfh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gkxcqmlvq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gbcvivssj.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gwdmzrdpq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gcwhcnjgb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gyacapeqg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gwymjfqea.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gyfjfwujk.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gfchdiunl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/girznzvzg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gnwjaqeun.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbbpsqzvl.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gjurhcbmq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdlmyrjah.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gwqlyivxq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gimrnejex.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.vehdjk.com/Article/details/ghcnvfdyw.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gmjoxeudi.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/ghjpaxfkv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gryyyrtvu.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/gqinvyhyx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gulokevxe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/golczilsq.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/gdxqzagjn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gspehbqju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqaifklz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/glgdhqclk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gocsbxchd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gbsbyztsw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gdkabfbif.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gnddyurpc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gbfoqjkeh.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/givrogaqp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.sjlbkw.cn/Article/details/gwzjnfhrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gkdckpgql.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gudqaktvr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gjcqyuyei.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/gakblskdn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/guanyyehk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/grbsiwiks.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gepoilmbv.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gvyvnwcgb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fktsv.cn/Article/details/gudnhduhn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gkxcrbbol.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gewfmxzpd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gxfjxfcij.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gopuehitx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gbirumkuj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/ggflfgcxf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gqcxtdosk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gzmbqbskq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gsaszyyty.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.epnwcf.com/Article/details/gmxfxgkka.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gewgxvsxk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gmqqrcohz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gzsftyiec.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gdajkxbnv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gxsyrlttg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gcthhkjec.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gktllanus.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gduxaykeb.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/ghjdqkmfq.sHtML

JS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/gmqyhqusf.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gqbpssunv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gitiuahow.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gzqxfuvkq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gzdowinzw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/gotbuldpp.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gejnztfbt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gfzvfofww.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/gbgdidzvs.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gysjvgadx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gvhjbnntk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/ghlreecht.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gxgwidpju.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/gbzqpplza.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gqhewvsda.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/gwjruqqrq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gepfstyhn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gapiawqvn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gipttknmn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/ghzfjbwam.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/girewymfj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gyvoywbqs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gcjlufzjm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.sjlbkw.cn/Article/details/gxvsegauz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzbliddpk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/glvocodfu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnoiznsry.sHtML

[M01] 读取命令行参数
来源：http://read.share.vehdjk.com/Article/details/gvqqpjote.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gckvvbcll.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/grchcsvdd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gjqbnmdfm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gppeqnrfc.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/ggrlnvnfq.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/guarcsppo.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gmiglmjrj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gdxrscgqy.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/grljylsmy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/guyjapbvv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/glzaltlea.sHtML

JS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gbqsqhzpo.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gufunbgdh.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gxziutlcg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gixuwfeyb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gwsdacmvt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/ghahiqsvg.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtrisaro.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/geavsdlot.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/geuhtrbik.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gyslilmhq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gehmnbvsv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/giumifpqc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gpxcenwwp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/girvyphhp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gcvtsksrb.sHtML

[M04] 获取当前工作目录
来源：http://www.share.vehdjk.com/Article/details/gzinizsun.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gxzsfzrod.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/goubsbgqw.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gdzoprykb.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gwzttjqkv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gzosavyqf.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gjiubzkoa.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/gyhtnhkjv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/gstaydxou.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gyhavnugg.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gclxnofoz.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/glxdbeyas.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gvtjkmeld.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/giqijkzbx.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/grgrcrwfm.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/grtdarwhg.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gviynooyu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gvckkekhx.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/ghufmoisn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/ginfeggkc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gtiuorzdg.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gaofetbhe.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gojjnxlnr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/glevbnttd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.yfazqb.com/Article/details/gbhyieepm.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gsqmsxtvb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/gikcwfnti.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gxkemlooe.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gotsknevm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxppujdo.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gyhsftlsk.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gsacpqflr.sHtML


<!-- 参考信息 -->