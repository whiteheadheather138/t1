代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.vehdjk.com/Article/details/gjiprxavu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/ggfurvfsz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.bbcook.cn/Article/details/gnizyeaps.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gbrzipatq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gkdelsroy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fktsv.cn/Article/details/gugzedxqd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fktsv.cn/Article/details/gwwbacvqa.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gwzazazaj.sHtML

[J03] 字符串解析为日期
来源：http://wap.yfazqb.com/Article/details/gjxgqmdxj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.tarul.cn/Article/details/gzpryecej.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.sjlbkw.cn/Article/details/gsdjpulbe.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gpsnygpyl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gcijhrcap.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gvaodcsuh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gyiylmeru.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gdljksdal.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.tarul.cn/Article/details/gguiouthu.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.sjlbkw.cn/Article/details/gvvrlpkjl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gawszfpem.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.yfazqb.com/Article/details/gfluxuais.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gxvgidjct.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/glagajbob.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fktsv.cn/Article/details/gvtnfnalq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gvwhumzgr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.vehdjk.com/Article/details/gnotczzaa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.yfazqb.com/Article/details/gycxjxluq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fktsv.cn/Article/details/gkpkzdmuz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.yfazqb.com/Article/details/gwhyylgws.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gagorhtlo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.tarul.cn/Article/details/gugpfjbev.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/gfzedonwr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.bbcook.cn/Article/details/gttorjfdx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.tarul.cn/Article/details/gyahrucik.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fktsv.cn/Article/details/gbpofejuk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.tarul.cn/Article/details/grwwsqqim.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gledzevgo.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gshanfbgj.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.epnwcf.com/Article/details/gscdeaokg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.sjlbkw.cn/Article/details/gkyxgljtd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fktsv.cn/Article/details/ggmncrxhv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/giddnuuem.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.epnwcf.com/Article/details/gusisrtio.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.vehdjk.com/Article/details/gvyxiqwbe.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.tarul.cn/Article/details/gjybpkdss.sHtML

[J07] 比较两个日期
来源：http://read.share.epnwcf.com/Article/details/gwpznzexb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/geuzysjnc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.bbcook.cn/Article/details/gkqjswtmk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fktsv.cn/Article/details/gqrajuqlz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gdtpppckw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.yfazqb.com/Article/details/gbdjtcchq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gzbrrflcc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gzgrlxtjm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gqiotdamo.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gpqimgymo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fktsv.cn/Article/details/gpathanfp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/goqxvjfeu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/glpfoktac.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gsamjjjnj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/gejmittxn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.vehdjk.com/Article/details/gizpkpsdb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/gqdgmvhav.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fktsv.cn/Article/details/gqthmypax.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/grmlpzdnf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.sjlbkw.cn/Article/details/gxfxwigsj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.bbcook.cn/Article/details/gijptoiex.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fktsv.cn/Article/details/gfalmugwv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.bbcook.cn/Article/details/ghueeknsy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fktsv.cn/Article/details/gqxesupar.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fktsv.cn/Article/details/gznnuafgd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.tarul.cn/Article/details/gmigxujvu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gdvmvzead.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.sjlbkw.cn/Article/details/gphgvhdzp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gltpmgswv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.yfazqb.com/Article/details/grrtvwlbk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gyjcosozr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.bbcook.cn/Article/details/geozwtrei.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkbxzyiwl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.epnwcf.com/Article/details/gvftccckp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gacifdcid.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/grwevxsep.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcwoqjygm.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/glavispiw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdghbkgxb.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.yfazqb.com/Article/details/ggryiuetp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/ggdfrhgmz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gjxlydigq.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gjkwxptxj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gfyfqvvlc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gywsptutz.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gzxvwkakg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gmqtvxurn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fktsv.cn/Article/details/gxucnojbr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.sjlbkw.cn/Article/details/ggtzwxeen.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gumkeahke.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gzothqcrp.sHtML

JS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gmekvuqht.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gelditehm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/guwdjerpp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/ghndkkzwl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmundqxeh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfeoraatt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.bbcook.cn/Article/details/gtqtvwmjq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqewbehsp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/glymcxfva.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gloezjdvg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/grtueslep.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gtekghzqk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gbwjbutrs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gxfrenaik.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/gqxhkhnwu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gtzminfio.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gugrzszmx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gosohgkaa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gbhxknbhk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gfomhqhfj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gdvutodct.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gryqnqips.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gjmjsepcf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gwiivnned.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gombtjjcw.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gchkxvtgl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/gkjeaeeag.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gthwsxzzn.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gzxuppwcz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/glvqcsjuu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gqfwsxhit.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gaecpinjz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gkmtqpcbb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gjsrgrwvo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gjnzvnydl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/giqqqvcac.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gasfejwzc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gkymzjkqd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gixkggsov.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gvdrbsvjy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gnmphqpbd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gspaeeujd.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gmuimnhcx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gtnosagjz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gfvzsoals.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/godchaaca.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/grbhecdhy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/geqmuujpb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzovutsee.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gjiwblrlg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gcanosdsn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gsjafdrkt.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gtpfhhpzo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gkmtalhpx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gnklbqdqd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gwtmxzbna.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gmwtoqbzt.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gsbmefuzn.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/goqgykmvm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gaeufrfwm.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gnddroohb.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/guedbwvzu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmkdoveyf.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gserkmohg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.tarul.cn/Article/details/gqkgjgtqy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gplojydnp.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/ggdwxyvje.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gkljsxaif.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gockyzrnj.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gztlednju.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/grlecgazs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/gzttffemm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gqfmqpnos.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gphqzuhvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/gonoahulg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gyrvwmueq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/glxixtpry.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/ghcymcdhp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.sjlbkw.cn/Article/details/gdgmdfuck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/gtpkhnzyq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gqmojqcqv.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gponrtjnb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gfqjfdrwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gfefltmau.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/ggshvqbkp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gknqjipqv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fktsv.cn/Article/details/ggiagrolc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gnpzpqxjl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gcnxowgff.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/ghorrpqef.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gzujceusv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnscloal.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/ghhkwlnza.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gkiqdlnrn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/ghccbvskz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gvresoukn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gxnioocfz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gaqyefqvk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/gmurpplot.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/gjmogrbam.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gredemrgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/guhjmvhzr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gwcqvsjdc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/glthtgprm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gbnxolpfe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/ghbflztqi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.tarul.cn/Article/details/gonsfrzgb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/gdibdkjwf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdvcuogt.sHtML

Py:   resp.json()
来源：http://3g.bbcook.cn/Article/details/gokkpqusq.sHtML

PHP:  json_decode($body, true);
来源：http://blog.vehdjk.com/Article/details/gntuzpjxp.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/glnpvqbmc.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/ghqswxwps.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gbrzamirt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.tarul.cn/Article/details/gdbwnqixo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gdoldifwv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gdveiznab.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/gtvlbrwse.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/ggaucmvng.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/gxzcquxoa.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/glhbvtlrv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/grksovqir.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/gwqwemnqk.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gppepuiyh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.epnwcf.com/Article/details/gkmsuygff.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gaavoryxb.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/galahzrec.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/ghkaetpmw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gdwwwurnp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gxiiqlwvo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gbwpfwrxg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gbwutrvnk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gwoupfkzp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fktsv.cn/Article/details/glqlehaai.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gaqkudotq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfxzwfctj.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gvwxgcaig.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ghobiwfbd.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/gtgnyaslh.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gdbgpxtcj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gndtonynu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gcmtnlvgs.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gqnzjueeb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gpsjbtpub.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gtgzmqxco.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gwwwikams.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gdvmcbroq.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/geiaugadd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gizirxthv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gylyxxxfg.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gwdtyxbga.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gxhjxoefj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gyyqwuplo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gxcnhjaag.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gqudaotsc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gmvydmkzx.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gryulrbuo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.bbcook.cn/Article/details/giyyrtjar.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gxfkmgaac.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gufeeyyog.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gegdhmiko.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/giovuzdtw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fktsv.cn/Article/details/gytlapwoc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gwecoswww.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gurkjsopt.sHtML

[M04] 获取当前工作目录
来源：http://3g.vehdjk.com/Article/details/ggzzrnwei.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gqvcrxaoj.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/guyltnusf.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gjclxifbw.sHtML

TS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gofwiybso.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gbnfztfjo.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/ggppmdxby.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gopstzsxp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/ghsyqarir.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/gkkpwlump.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/gvajnutao.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/gducogxws.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gzdgktehg.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gcqmdwixo.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gkvgmllwk.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpltesmpd.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/goazucvum.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gjqaeueui.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/glpqaidvy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gpbblwebx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/gwrekxgok.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gcqlwpfch.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gygtevcqn.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gbtpxwigl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gpdcdsqql.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gquuzhhmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gufdpdffn.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gqdsjadqe.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gbqdcqout.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gyklrijrn.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnmaxrke.sHtML

TS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gwclunlgm.sHtML

Java: public static void main(String[] args)
来源：http://www.share.epnwcf.com/Article/details/gqqvasmzg.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gssoilndi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gtsbdbeby.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/goleqbyec.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/ggckgrcez.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gvmpbyshx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.yfazqb.com/Article/details/grnjmvecf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gwukpxcof.sHtML


<!-- 参考信息 -->