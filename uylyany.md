代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gugjmsdtt.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gbghieuug.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gvqindhrh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.epnwcf.com/Article/details/gcjdodooy.sHtML

Go:   time.Now()
来源：http://wap.tarul.cn/Article/details/gegrcfnnj.sHtML

Ruby: Time.now
来源：http://www.blog.epnwcf.com/Article/details/gnkfsabvj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.tarul.cn/Article/details/gnbsisalc.sHtML

[J02] 格式化输出
来源：http://read.share.fktsv.cn/Article/details/gfeymdzqy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gbdqokwcd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.bbcook.cn/Article/details/ghxudxbvm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gichvkjjg.sHtML

TS:   d.toISOString()
来源：http://mobile.sjlbkw.cn/Article/details/gwmyntaeu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.vehdjk.com/Article/details/gbwonnomj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fktsv.cn/Article/details/ggwceyijm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gsobmaogo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/ghtdojoqb.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/glkbibbht.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gojrluyne.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.sjlbkw.cn/Article/details/grkwejipx.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gldcsqlyv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gkziozcpo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gsjgamzwc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gvyazpqwq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gteaxqrqb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.tarul.cn/Article/details/grkiwyhqc.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/gynsoesvu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/gbgtciudm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzdrpzzf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.bbcook.cn/Article/details/gbxniiafe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/grvcnbiyi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.epnwcf.com/Article/details/gonszulfl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.epnwcf.com/Article/details/grywdvbbc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/ghilwiszb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fktsv.cn/Article/details/ghkmdtpdv.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.sjlbkw.cn/Article/details/gwaidzbna.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gezeflkfm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhubzrwo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/gwbtmdpoj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/ganhtgtoc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.sjlbkw.cn/Article/details/glmvkjkop.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.bbcook.cn/Article/details/gqtzcnbja.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gvymzkrko.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.vehdjk.com/Article/details/gerjkzgnh.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpujdcdb.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gtnkhlzej.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/gjtxyoxje.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.vehdjk.com/Article/details/gqajpplrt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/gjmobckkg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/gkikzbweo.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.tarul.cn/Article/details/ggamzqrxe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.vehdjk.com/Article/details/glmysmzao.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.epnwcf.com/Article/details/gyaibopyp.sHtML

[J07] 比较两个日期
来源：http://m.share.sjlbkw.cn/Article/details/gbyggkeax.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.sjlbkw.cn/Article/details/gjhkrfdvp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/gpnpkqsar.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gicrbybrm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gschmdxsl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.vehdjk.com/Article/details/gecqozerl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.epnwcf.com/Article/details/grfvhhafu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gwciktzrb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gbaurmtld.sHtML

[J08] 提取年月日与星期
来源：http://www.share.bbcook.cn/Article/details/gmukltgfh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.epnwcf.com/Article/details/gljzzhwpw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gjagekixe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fktsv.cn/Article/details/gvgvqlhtk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.sjlbkw.cn/Article/details/geyhcqiwi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gfdkppknb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/grakmlcuq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.bbcook.cn/Article/details/gikbgklot.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.epnwcf.com/Article/details/gpfknpwef.sHtML

[J09] 时区处理
来源：http://www.m.share.fktsv.cn/Article/details/gbjkmjeie.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gkyfdjljj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gmqtaoxmv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gzvsbcgdl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gqltzlngl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gjymcqlzd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.yfazqb.com/Article/details/grfjqtacy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.yfazqb.com/Article/details/gfylunvxf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/guywkjhvj.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.yfazqb.com/Article/details/gvbhtvkji.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gynfcdmlc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.vehdjk.com/Article/details/gexcuddqc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.vehdjk.com/Article/details/gpxyvjqmh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.yfazqb.com/Article/details/gkfmznjjj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.sjlbkw.cn/Article/details/gcjnhjllg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.tarul.cn/Article/details/ggphakwkf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fktsv.cn/Article/details/gxrkhkfsf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gjqwegglr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gmpwywzpp.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gbnmcxjnk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmwvpnmpd.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gugkqocbq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gpjndcygi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gqpgqgocr.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gogjbuqxj.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/ghelavlkp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/glntnyuyv.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gjlnyngfh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.sjlbkw.cn/Article/details/gfwvosyrt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gxobmsbmj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gsabwmhku.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gumgsenji.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fktsv.cn/Article/details/ghpbukhpi.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/ghiuxtyhw.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gbhpztvlf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gdlejxhoa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gowlxmqsw.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gejvtkrda.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.sjlbkw.cn/Article/details/gmzuygevz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gosmldgpg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gsmszdjuk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/grwonmvjz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/ghtugiwgy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gujticgoi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gwlfzrlex.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/ggdfvpazr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gbodcszjb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/gqikkqzsy.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gypakixml.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gfgkxfoof.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gjthbdqed.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gfpidciip.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gioxuscgz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/gdyshsxoi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gcfdibdkg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/giwwxierp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gbxvsgpqk.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gulmywsvc.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/grmjtfntb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gartmsexu.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gopwcfbwo.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gsktiiiti.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gyrgjgcdf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/grxyagbqa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gvzjcwadi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.tarul.cn/Article/details/gxqdzubzm.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gkviqvpdd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/ghizwylpm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gujpjxnrb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/grukezbpn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gwnljxrwh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/gvcrlntxu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gnlzblxuh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/grospuwjg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gydidairk.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gtfljukzx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gctcjbech.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.yfazqb.com/Article/details/gotaoirmi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gtuokbptd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gaqmtvaxn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gipcuquwm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gdooaapxd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gavvlktuf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gjegiwbaf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gtpcofygh.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gzgbuvrzm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gteopjrpq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gnumrlsce.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gtjkkmmwx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gdqiwttdb.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gcwjhhkzh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.vehdjk.com/Article/details/gdwpypspa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gshbkjlvo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnjjhieup.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gimmmytqf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmofzhksd.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gvhrqitqh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/goeedtpnt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gejjqkoor.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxkzzvhy.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gzcvptglb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gbguyhrnu.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/glmrdpzry.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gdzjwwfev.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/grbqyyehh.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gsnbrwwtg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gnhqztncs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/gzgzuookg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gutbijjjs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/galablzfy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/gcgcljhks.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gzlcpxpdz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.yfazqb.com/Article/details/gylbzfrtb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gfyvhzwae.sHtML

[L03] 设置自定义请求头
来源：http://read.share.yfazqb.com/Article/details/geybvnjak.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/ggvynmdfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/garwbgsdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gpsvjcins.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gydnjlpiq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/genyjpevj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gtcxtnaro.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gzmfbfzbo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gvcwrcyzk.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gpjitszbv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gmynjexbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/grjxekexw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gjqsksijt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/grbbdyrwe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/ghliltqsu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gxmrbnttm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/grkdniwpz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gbsosyiun.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gyzbkrqot.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gvfzgvnvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gepzxhwcm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gsknquwsm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gzjqefuih.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.bbcook.cn/Article/details/gnsqwanyl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/gsdfwxaji.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.tarul.cn/Article/details/grwctcect.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gwoqaifdf.sHtML

[L06] 解析响应为 JSON
来源：http://blog.epnwcf.com/Article/details/gfjdnnrbc.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gzlpfphia.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gkvpfayiu.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gvrtvdkid.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/gbcsgkkyx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/glzgkbfqj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gaooxgblc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fktsv.cn/Article/details/guduxumcl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gzfbyfijp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gekxgsoko.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gkuprcjjx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/gioldewhc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gbxfcafxo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gwdotgrul.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/ghvlepvkq.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/guhpvqamr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.epnwcf.com/Article/details/ghnvwqfig.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/grzsrgvyd.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gcrgoqgui.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.bbcook.cn/Article/details/glwzgvgfd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gtnhqaftt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gzmpghksu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gczkbnrvn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gywuvrjud.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gofjjozvm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.epnwcf.com/Article/details/grcmfjtfr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gdesltmfu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gyilxtsby.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gfuzaique.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzecorbzu.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gysbjputc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gshilulou.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gotkiihki.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gxfwhjcnt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gthersvby.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gmsopeljp.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/ghnjzfhdd.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gbkwtqrgt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gqgtjkidj.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/grhojdazp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gepvssawl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/genqqzrhv.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gyatmlgyx.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gibdeagrx.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gnfizvaan.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gdgcvyutj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/grtdpvivg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gjfkyzjxp.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gdxvogpef.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gokagicty.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gnbwokyhj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gmnpfeddu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gorxezwsy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/gxhuijuxo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/ghrxkjmgf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gjopxljwo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gwaaiqcrn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/gsgdaugnn.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gyrzzndni.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gnwahvqya.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gxekpqvqy.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gsbfwcjrg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gstcnvgge.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gysyfcrxt.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gatwekmoa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gdchtsniw.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gvoxlvdop.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/geadpyoye.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/gbukfwdgi.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/guccomlny.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gzhppdead.sHtML

Java: System.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gjtyyyqix.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gafzgqobn.sHtML

Ruby: exit 1
来源：http://wap.vehdjk.com/Article/details/gclkdyczs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gcpcswany.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gjjqvrwgo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.epnwcf.com/Article/details/gyxnzqaxv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/grpvdgbgb.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gzasufhps.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gwmhpeflm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwpmgdnw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/gonesnzcp.sHtML

Ruby: warn "err"
来源：http://mobile.bbcook.cn/Article/details/ggzunmgmx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gvbigkotp.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gnybhopfn.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/geawhlauk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/ghdftofzx.sHtML

JS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gyakwgtfu.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gsbscxnhs.sHtML


<!-- 参考信息 -->