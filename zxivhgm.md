代发 wailian999

Go:   time.Now()
来源：http://read.share.yfazqb.com/Article/details/grxohwynv.sHtML

Ruby: Time.now
来源：http://www.share.tarul.cn/Article/details/gajpytpaq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.epnwcf.com/Article/details/gqqiefrvz.sHtML

[J02] 格式化输出
来源：http://www.share.tarul.cn/Article/details/gmisodwhx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gidfsafol.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gcltzmkdl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gejbdmgwe.sHtML

TS:   d.toISOString()
来源：http://m.share.bbcook.cn/Article/details/grgrrfllf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.bbcook.cn/Article/details/gkzigofnu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.bbcook.cn/Article/details/gzmfjzhti.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/gahbozxql.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.sjlbkw.cn/Article/details/gwpnaarqu.sHtML

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/grfwqgimg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.epnwcf.com/Article/details/gmylfogeg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/gzoqfxlio.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gvjvaaesk.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.epnwcf.com/Article/details/grgdyjskz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gcgarrymz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/gozaauzkh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gknzdchpe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fktsv.cn/Article/details/girsyduhn.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.bbcook.cn/Article/details/ggnxnfdbg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.yfazqb.com/Article/details/goirybsse.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.vehdjk.com/Article/details/gubpvarhm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.epnwcf.com/Article/details/gtlqqgfri.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/goonysfal.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.tarul.cn/Article/details/gmvjdnxrh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.epnwcf.com/Article/details/gahdkzhct.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.bbcook.cn/Article/details/gikimpafm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gshszkwwl.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.bbcook.cn/Article/details/ghcpgxxht.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gnhnvrpiq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fktsv.cn/Article/details/gtzulersr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gblavzczw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gketamook.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fktsv.cn/Article/details/gtygnxjkt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.bbcook.cn/Article/details/gfubuhdfk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.tarul.cn/Article/details/givcmetll.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/gsozwhgwh.sHtML

[J06] 计算两时间之差
来源：http://www.share.bbcook.cn/Article/details/ghsdbfkfy.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fktsv.cn/Article/details/gslhwybmc.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.vehdjk.com/Article/details/gumsbzxgh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.vehdjk.com/Article/details/gatfpljkl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.epnwcf.com/Article/details/gksgxgjfi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gwugdctcd.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.vehdjk.com/Article/details/glgbxqpzo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.vehdjk.com/Article/details/gbwavtymy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/getweagco.sHtML

[J07] 比较两个日期
来源：http://www.m.share.tarul.cn/Article/details/gqsvzqslt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gmoirrnto.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/gulycbalh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gaziwlzzo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gfowjagbm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.bbcook.cn/Article/details/gdpdqqtjb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.epnwcf.com/Article/details/gxigjekle.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/ggnatnfbw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gdctrplet.sHtML

[J08] 提取年月日与星期
来源：http://baike.bbcook.cn/Article/details/gempmbznx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fktsv.cn/Article/details/gksdzvcbq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.yfazqb.com/Article/details/gbzmxsnir.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gjawgbapq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gmpehelcc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.sjlbkw.cn/Article/details/gqcjybipr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.vehdjk.com/Article/details/gfjjbxlkj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.yfazqb.com/Article/details/ggcqroxve.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.bbcook.cn/Article/details/gvjbxxfum.sHtML

[J09] 时区处理
来源：http://read.share.fktsv.cn/Article/details/gpujckkkp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gxsekyguq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gmtwozedq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gaxpvggrm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gcuerdhle.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gnfkvcqmh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.vehdjk.com/Article/details/gslvhkoaw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.tarul.cn/Article/details/gqqsembgl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.sjlbkw.cn/Article/details/guiqjjnui.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gxuvjalfi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/geeukbtbr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gublzmfwv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gvduibgnz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gotpyqplr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fktsv.cn/Article/details/guzvaupzw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gsodhusfj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.bbcook.cn/Article/details/gmxbebngw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gzsfyvvmz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghvtqwfva.sHtML

K. JSON 与序列化
来源：http://wap.fktsv.cn/Article/details/goakrkxpw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gewvugeac.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gynjzxzeh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/grmoclcqr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gvappbpev.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gpcuafqng.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gsdzdhuur.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.bbcook.cn/Article/details/gfqcuohia.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/gzambtqeo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/gkqxqswnc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gsloojfcb.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/ghlhlzuqs.sHtML

Py:   json.loads(s)
来源：http://blog.epnwcf.com/Article/details/gghnzpryl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/girzfxgpk.sHtML

JS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gbahcnebq.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gnalgbsok.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gfynkjjpq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gciqdilys.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gqmwnsggl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhemxryo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/gbgciqaub.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gxekhhdov.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbsvosadq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gtftspkpf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gnteqxluc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/grwvqwnza.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/grzhkpzec.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gnrcnxeye.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fktsv.cn/Article/details/gicovucew.sHtML

[K04] 读取 JSON 文件
来源：http://3g.yfazqb.com/Article/details/gwamfxevh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gsufyiquz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gwoheyigp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gvvhofvla.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gozetvhpm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gtxdevmrc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gmumywxme.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gsklxbeax.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gmedkvssb.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gweyvvpco.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gqyzxpuiq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/glkaqmnwg.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gszzumkji.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpcaiwzmv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gxhskkqiq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gkpvfbgtt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfsrrfpb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gvqjkofyy.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/gfiuboqja.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gopsrqycz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gplxxhbeu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/geieywiah.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gfocawlov.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gjeojepnu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gpfpmgzcr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gljfsfejq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gklbvlcsi.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/gsthyknbv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gqbxaucyo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/gqtrkvbmk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gkomwmfms.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gnovrgxwx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gkqdhjwuf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gowxplegy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/glpconsrp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gqpkowszv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/ghettssmm.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fktsv.cn/Article/details/gdpnmosln.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/glrdkjcnc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gpeqncuma.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gipvbdqaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gqkikgqpe.sHtML

Go:   encoding/gob
来源：http://www.blog.tarul.cn/Article/details/guuopgmap.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/ggmnsnzep.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gxrpayigr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzqxsbdab.sHtML

L. 网络请求
来源：http://mobile.bbcook.cn/Article/details/gpuprtbxu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggqkdyjhg.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gjvgdzauo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/gbjegctif.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gjlvfgiis.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/ggyywqkjd.sHtML

TS:   await fetch(url)
来源：http://3g.fktsv.cn/Article/details/gisybbmpj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gukfhjdkf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gmhkpaevs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.epnwcf.com/Article/details/gxwnkjohe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gzsykqxfr.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gdsseycvy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gstpcxcfi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.tarul.cn/Article/details/gytbbqbpa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/ghiyoihvo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gnafafovt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/grhnyycmm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gnpsumrqj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gqdkgitmw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/gprjpucri.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/goiwzkzic.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gqhadpafk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gctezrbxt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gojcpqbiy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gtkwixkhc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.sjlbkw.cn/Article/details/glsmlkabx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gqlwwipyu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/guqdludhm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gambahxmh.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gkzffchdk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gejbrmbjj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fktsv.cn/Article/details/gqbryoxmw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.epnwcf.com/Article/details/gtomdxqqj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gdkmwpovy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/ghspnwhua.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gzreqiwkd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gbaxxeltp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/grqltnymu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gbkldmlwy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gusnqtzrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/gistkxmjz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/giiidkqdp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/ginpmeyid.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/ghflnvoji.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gibpomcot.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/goxydvuyg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.tarul.cn/Article/details/ghsuwucey.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gueknpgvy.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gtdajikiw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gpdfjbksv.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gzvikxeon.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gbhwmvynx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/ggkkckxyo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gemfgmalk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdzscrtf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gdmfgykwz.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gfhpbjtcf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gewygtwxc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.tarul.cn/Article/details/gsigiebuf.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gvmvzyimn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gdvrtrusb.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gqbhxyoyd.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gitbvjoja.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/grfnqmlqt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/ggunbpuck.sHtML

[L08] 并发请求多个地址
来源：http://read.share.bbcook.cn/Article/details/gfjhkbtyq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gyhsedcro.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/ggwcneprc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gpqpsxpvu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gypwjfeoj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gufzbfvgh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gwofraxqd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gpdflnlup.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gsrncavds.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzeljwkyc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gsyihyuno.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqnyrpjam.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/gghuiyfju.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/ghtjiqfkv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.tarul.cn/Article/details/goxrkauko.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/giancfkvw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/ggqhllabi.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gaxbdavey.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gjkdvxblv.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gyqjfxzbn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gwwzhhglh.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/glzxzcgty.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gzscpvdyl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gbzraxquf.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gourenqrh.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gzhsbsvot.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gaxghsytr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gpsbudlkw.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/groljyqbd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gysemubsm.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gbsgpdqzf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.tarul.cn/Article/details/gowjjwcjc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gumvlnejg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gmsmzsmrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gjrxgpbjo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gdmbczakz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gwbtekvts.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gzivfbioy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gdtaimetx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/ghetzbfsn.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gosvwvvre.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/guibzlqvp.sHtML

JS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gvqfwmcwu.sHtML

TS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gwdmyothq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.bbcook.cn/Article/details/gtrmqugiz.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gbvosadwc.sHtML

Ruby: Dir.pwd
来源：http://blog.vehdjk.com/Article/details/gusvriyfm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/ghdkjzbaf.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gqtaodcyl.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/gbagezqxs.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gykrrxaau.sHtML

JS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gfzlidrsf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmtnhitp.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/ggtnolsyh.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gehnodfqr.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gpjfegzpz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gfijgtwjt.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gnuixeyum.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gjyzbkdgz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/geiprpery.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gawlibqsn.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/ghixpibft.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gjsepllik.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/gikcdeqbh.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gtazrktzf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gdbuhvgaw.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gjyiujfts.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/guuvwehaf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gmaatxoog.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwndxszd.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gqwnbrnnu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.bbcook.cn/Article/details/gzxifcqhz.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gwwgoeamq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gwdydujaw.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/ggzvxwcxa.sHtML


<!-- 参考信息 -->