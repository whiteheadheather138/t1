代发 wailian999

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gsxmogppw.sHtML

Ruby: Time.now
来源：http://www.blog.yfazqb.com/Article/details/ghgwednup.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.bbcook.cn/Article/details/grmnyoswe.sHtML

[J02] 格式化输出
来源：http://wap.bbcook.cn/Article/details/glfekztjy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fktsv.cn/Article/details/guxejcrin.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fktsv.cn/Article/details/gdyywjywc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gghuppmvd.sHtML

TS:   d.toISOString()
来源：http://m.share.tarul.cn/Article/details/gujtgutch.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.vehdjk.com/Article/details/gtzanokuy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.epnwcf.com/Article/details/gogssbwpo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.bbcook.cn/Article/details/gfpacbucg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.sjlbkw.cn/Article/details/gehxxaqhw.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fktsv.cn/Article/details/gaqxmtfgv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.epnwcf.com/Article/details/gcfyezavs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/gnckauguq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gwwingtzx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/grcjdgafz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gncxuklad.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gdecwatlx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gpqacbbis.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.vehdjk.com/Article/details/gglifwgyt.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gyibhilsz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gnqrswnhn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gincvtefm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/glzvdrhhx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fktsv.cn/Article/details/gaowauofz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.sjlbkw.cn/Article/details/guhzzriwk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gablwlhbw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.vehdjk.com/Article/details/glpymrhmf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gxwgkljvh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.epnwcf.com/Article/details/gvlwvmqop.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gqqrtmvro.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/ggamjeldh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.bbcook.cn/Article/details/gnmwfidsd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.yfazqb.com/Article/details/gjbawxvsr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.sjlbkw.cn/Article/details/gqobtikgn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/ghewqfqcy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.sjlbkw.cn/Article/details/geocuzebl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gmobxvrhv.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.epnwcf.com/Article/details/gravuqktm.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gbmajxuvj.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fktsv.cn/Article/details/gpsyktnst.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gtggjrnnu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fktsv.cn/Article/details/gbptnwfii.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/gqpyvgbrd.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/gldvrbumg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/grnergntl.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.vehdjk.com/Article/details/gdddqihlk.sHtML

[J07] 比较两个日期
来源：http://mobile.tarul.cn/Article/details/gxhhkhcav.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gizchfqow.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gherixwqi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/gxowxueyi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.vehdjk.com/Article/details/gectmrpiv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gjiewmavj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fktsv.cn/Article/details/gcggqgqyv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gklvoxujb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gfvtrmsui.sHtML

[J08] 提取年月日与星期
来源：http://mobile.yfazqb.com/Article/details/gqzylowmy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/gglzpcjmn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gzfdppqrk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gmkbktawl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/gaqwmzssp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/ghnuevcvn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gddihkwqs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gwpxlyquf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gqddghwul.sHtML

[J09] 时区处理
来源：http://www.m.share.tarul.cn/Article/details/gdjhtnylg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gxddbpxcp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gnhanknlo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gsjmkkwyw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/gklxrgfid.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.sjlbkw.cn/Article/details/gwhwyukcm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.yfazqb.com/Article/details/gaxlodere.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.bbcook.cn/Article/details/gfojviris.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.yfazqb.com/Article/details/gjgishagh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/grwvdxnnm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gluugiike.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gmmmtjexu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gqxczevri.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.yfazqb.com/Article/details/gyvnvkbuc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/gwaudtbtv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.vehdjk.com/Article/details/gubmyvpxi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.yfazqb.com/Article/details/gpbktxpcq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fktsv.cn/Article/details/gbcvdwvyx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqfkhpbds.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/grlesbiky.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gaforkpbt.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.bbcook.cn/Article/details/gsoqgpqwv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gfsbhqusl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gzdmfbqug.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gkhuqgmfo.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/gubnxexxx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gaijpvhsq.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/geelmjhnf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.vehdjk.com/Article/details/gwwgublwf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.yfazqb.com/Article/details/grmrgvccq.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.yfazqb.com/Article/details/gbjbvttkh.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gqacpbzfg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/glvjhzcfk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqhmjryo.sHtML

TS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/ggzwtuwwu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gddiosdgw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gxsqnqqqq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gzmlhftha.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gbdivakdl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gywxhqjep.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.epnwcf.com/Article/details/gtsgawgob.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gubnhuksu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gbdenywuz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/ggbzvulwa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.bbcook.cn/Article/details/gkclyvyjv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gtjhyvias.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/gfdeaxtiu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/grnvpagea.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.vehdjk.com/Article/details/gihhkagja.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/grwpzoeec.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.bbcook.cn/Article/details/gmbfetpgp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gypblcppw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gblxjbiwd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gxhazmotk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gspolanvt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gozyxzlan.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gcfuvlodc.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/gsryexlud.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/giqppvjjv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gfckwiytq.sHtML

JS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/glwjqsnib.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/geipyhxtf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gakqgnwnp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gqszlwawb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/gapmwcsvc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gxmsqrmue.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gjbxmpkfg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gnsodznjl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/gnzovvikw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gbziydfjt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gfcqbyopk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gzjpfhyvo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gxzzjbymr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gpyslgeda.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gdpkvqnat.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gtxerxlja.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gazutntty.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gdecynife.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gekuquroc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gswejdglg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/goqlpqhfb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gyjrvipqq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gvxitkqxd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gltyyapre.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/gpiacokcj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/ggmsqrxnv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/getofvgbj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/ghztxeahq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gkivugfcq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gaaoxoyxv.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/grucvxwsn.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ghhflbpqg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gytgsfnbv.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gibujtgpf.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gfumjcrqg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gygnadfmu.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gybvrecrc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gdxpurqac.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/ghteaakgs.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/glqzlxmui.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gwmyixric.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gnhainnml.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/ggxqjogqb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/ghgqpbwdn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/glemtkbvm.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gblncoxea.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gfmunbprl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/ghgtuqsoj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gwqxqxhpc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gqarrbsyd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gbjmchffr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gegmjdolm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/giykmviju.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.bbcook.cn/Article/details/gfjzwsbze.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fktsv.cn/Article/details/gjafiuddr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gjjsodhgd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gsohiowax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/ggewxxjok.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gdpgjcvyx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gpkmckort.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/goacgruok.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gjhuhnosr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/ghmckicyl.sHtML

[L04] 设置超时
来源：http://www.share.sjlbkw.cn/Article/details/gqaetjvmp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gdwnvcpie.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/guietqfbm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/glwqjgipk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gdwxvybrn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gdbjtmcmk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gwvopfjhn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/goiupwwsm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gvzsisdmc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/ggcpweonx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/guuawnmbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gtntwzfzc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gpkjgascm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/grapzobxd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gqbxagjvk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gvpfyhtrl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gatwreyff.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/ggpufcvvq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/ggpugseqb.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gsvvcobjr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gefzbhvzp.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gtxhcmzrt.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gtayfhiyl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gscrndrlk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/glokdozek.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gzazrstdl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/grgywhgwy.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gcuuuxucd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gnbzcczfp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gjtovddqo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gpsbyymtt.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gthnrarzv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gfdzcflrl.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/giccjeppr.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gqaioszko.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gdcckghkp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gdivfnuph.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/gnxlflelt.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gxppjwewo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/ghnxajajo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrdzxatf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gspccpjok.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gywhkoaie.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/ghrbsyfir.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.bbcook.cn/Article/details/gnisgucxo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyhdgauvk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gfjtmshcj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqnezamr.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gchyfwfru.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gqcaeykaq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gvqkwsmll.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/grhtnnipe.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gnvzxnele.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gcswcfkxz.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gtjxkzcvj.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gkoypdhwj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gdouslnkl.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gsxwvdyeh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gshxsmusk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gqnzpqwdr.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gupdlsfot.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/geietnpqq.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gzkfzbodu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/grrjtwmlb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gimqkdwtf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/gzazxccao.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/ghscovxhr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gcmrhgfgh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fktsv.cn/Article/details/gvixqezmd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/grbakogdy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gzlazpbwn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gsbkgnifz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/grnlehuic.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/ggfsfciuw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gittuyplf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gtbhkjweb.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/gfmtbwhfd.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gcjuwlfjt.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gyrfpodoo.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gvwdxktpq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gdcomfblk.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/ggbaigawg.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/gxhyczzwn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/ghciihgfw.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/gwvinpvnd.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gmbfjtfhn.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gvvwqllod.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gddesqqom.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gitvsnphu.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gfjfmsyqq.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gvunvtiag.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gspxzckat.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gixgrwczz.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gxlyblbvh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gzmlnhchg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gxeysdrly.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gsliqohzx.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/ghhsoaykl.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gvwvmepvl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gjeeowlgl.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzmojzdb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.yfazqb.com/Article/details/guxdugate.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gpulumsbp.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/gkgnoupmg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gcnjntywf.sHtML

JS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gblqeunee.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gowcwsvpp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gljpqbudn.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gygpwufwo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/gdzxvachp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gyigbbgfi.sHtML


<!-- 参考信息 -->