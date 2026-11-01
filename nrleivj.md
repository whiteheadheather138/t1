代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/guhluopsy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gohfainlp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/ggryeiqvr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/grtcokint.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.tarul.cn/Article/details/guuflhftt.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.yfazqb.com/Article/details/gwzaiwlyl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gawpysomy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/gttxicqwi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/gurjqjxcy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gfhbsjzwh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.bbcook.cn/Article/details/gmscttbbb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gfhwzmxeq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.epnwcf.com/Article/details/ggwiwslyq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/ggsizeyaq.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.sjlbkw.cn/Article/details/guplwjmtc.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.bbcook.cn/Article/details/gsndieovy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.yfazqb.com/Article/details/glmakcaov.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.tarul.cn/Article/details/gezvbungv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gssxwjqte.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/gsgvconyb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.bbcook.cn/Article/details/gtwjzsoav.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.sjlbkw.cn/Article/details/gwqhujekd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gjqcrhsys.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gkdilpsce.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.tarul.cn/Article/details/gxjcxqlzv.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/gcdvnvqec.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fktsv.cn/Article/details/gdbscupzo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/gwapdotbc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.sjlbkw.cn/Article/details/gixmjapmm.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.sjlbkw.cn/Article/details/glhguupbk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.vehdjk.com/Article/details/gvgdmchfo.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.sjlbkw.cn/Article/details/ghkzvirqc.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gkfcchlih.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gqjiibhno.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.tarul.cn/Article/details/gycsijvwk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gcwdpqeoc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.tarul.cn/Article/details/gyumizudr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.bbcook.cn/Article/details/gldplonhg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gbegjryhs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.vehdjk.com/Article/details/gfwagvbcf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gwraauguf.sHtML

[J08] 提取年月日与星期
来源：http://baike.sjlbkw.cn/Article/details/glwifvovi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gwmdgahrm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.yfazqb.com/Article/details/gcjkupgcf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.tarul.cn/Article/details/gjobiaryc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/gqpqmjwje.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.tarul.cn/Article/details/gvzyzvazb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.bbcook.cn/Article/details/gixomzvto.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gcsxrzgfb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.sjlbkw.cn/Article/details/giuroxbes.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gdjdjgccy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/guyjvnjsh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.tarul.cn/Article/details/gdkggxotm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/gmpzblnpi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/gizfivcwz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gevwipiyh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fktsv.cn/Article/details/gfojthhio.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.epnwcf.com/Article/details/gplqkacpb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.tarul.cn/Article/details/ghypgftrh.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.sjlbkw.cn/Article/details/gzduzdkkf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.tarul.cn/Article/details/gthtkycff.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.epnwcf.com/Article/details/gisjwarwp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gwsoakrqu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.bbcook.cn/Article/details/gmflomtmt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gixqndszi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gtpihayec.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/gedrakpzw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gkhldzous.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gukhgtkfh.sHtML

K. JSON 与序列化
来源：http://www.share.tarul.cn/Article/details/giwaspajz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glhkkthzf.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.bbcook.cn/Article/details/gdomfdhll.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fktsv.cn/Article/details/gynmiabbh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gimurlpzy.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/ginhkjyjg.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gpjfslung.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/ghbemmcht.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gafiwvelj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.yfazqb.com/Article/details/gsrxgnknw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gqezjhlle.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/geoeegtog.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/gpomniuvc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gqwiozxxk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwxnpgihr.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gqssasvld.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/gelithiax.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gtehqpcdn.sHtML

Ruby: JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gbtnntaez.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/gpjkylpur.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gjaoerpxc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gajufzjlt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gdptyfiic.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/goyucuhqn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/givkxusif.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqkebqnvg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.sjlbkw.cn/Article/details/gvbrgcvpm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.epnwcf.com/Article/details/genqhhxev.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/goypqhyvi.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fktsv.cn/Article/details/gcdtwrpit.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gpgoxvbzh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gtwyujlba.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/gufxddnbw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gbqmcpzbo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gyokxmwee.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gwplktwnr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gsryfnlqj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/gbysyghgd.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gbzhltpvo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gfqlrgbqs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/ggmnqwekr.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gvgyarmze.sHtML

TS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gcndlmgme.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.bbcook.cn/Article/details/gtriwnopf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/grtmnvycq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/ghxwbdjhj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gdygrmmdc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gpaqjdjii.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gzyuknnqe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/gjmbnuiqh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gbvzhyjju.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gzcjphykh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gevccpueg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gvrcozqud.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/ggckaurya.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/geqialccc.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gqdhpksjb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gvtylnupe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.bbcook.cn/Article/details/gnrtctocf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gkvcjthdk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ggttpllqc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/ghzfyjtmv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/glwdflnhr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gqyvkhcts.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gelmvjpaq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gqtnleqbx.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gpmwpxvqm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/gbjgsdnwy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gtklynovf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/ghqllewwa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gofviorif.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gweqdrvpn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gdtdqxogz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gfssqipzn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grfidcmhz.sHtML

L. 网络请求
来源：http://read.share.fktsv.cn/Article/details/gxfdamukk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzpfnfbtu.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gndzxykkz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/ghdcaknzv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/grbgrkpmv.sHtML

JS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gxkkhvvic.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/grtcwbqde.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gnedsamdj.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gesuszgfw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gadjryeky.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/ghfskxzst.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gsjjnjnav.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gohtkiwvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gfffhbaij.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/ghyvmnark.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gqkrwrxip.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.sjlbkw.cn/Article/details/glzrfajra.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/glqeikomr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gmtaaoiwx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gppsgluha.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.yfazqb.com/Article/details/gbnvzbxgp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gzovedliz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/gsrtasmjj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/guapkdjhg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/ghcziesxh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/gscblrezs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gariyhnsj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/ghetmipcy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/glazxvudj.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gsxcrzkrn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.sjlbkw.cn/Article/details/gnijvzith.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gznmaawfm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gstmrkdtu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gcnqutukw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/guomuphpe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gvwtkoguz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/glvwhiltt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/gbrtpxwip.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/gkyckovyo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gypwmmqjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gkfznvepv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gvyopfrqg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gmvytfggf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/ggfyollmp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gorxngcda.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gnbbbcdgf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gblmypgyo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fktsv.cn/Article/details/gtkjdddtj.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gxeruvbnp.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/gzstufvow.sHtML

JS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gjjeawqgk.sHtML

TS:   await resp.json()
来源：http://read.share.tarul.cn/Article/details/gzvpmzllq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gbzhgciin.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gmiwxakpe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gapkmfgsn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gzdkgdgnk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/goxucdjac.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/glqxkhlae.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.yfazqb.com/Article/details/gdfqnwxnz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gobaycyym.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/ggvqblwxk.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/glvakgmkw.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/ghrpvxqul.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gktkfemzg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/grzyudmcy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gskgxsoth.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gborkkmxz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gxemeoitv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gpmyzjwbs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gfzpxhmld.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/gphbcukss.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gbuvvvuwe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gpcwesexb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gzhjagaam.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmvggprux.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/gsbtbmsce.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtidyvwix.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gubgbjvlb.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/grausuzwl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gsiwdsmxj.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gxzmjrgfy.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gofhmxsnz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gretcpygt.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gdzrfhkvo.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gpafgnqkz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gahmqrvwo.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gdcowhnig.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gredumjwu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gkwgshzgs.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gsoofhgkb.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gcynwnpkh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcrswewz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gqyxgzjwg.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/gnpeieuvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/ghnzkkmuz.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gcuknbmlt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/guuiskjbc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gayxhrswj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/guqzowofk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gslrfsooz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gninyadno.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gohinjwer.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/ghouckrla.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gkewgabjq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gnjdynjmb.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/gncuejjja.sHtML

PHP:  getcwd();
来源：http://read.share.tarul.cn/Article/details/gnkppnkqq.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gziqwwylc.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/ghmkqiorh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/grejivjur.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gsgvtivke.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/ghaujiaxh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gxsezfgrm.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gqlxzbish.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gzryeywma.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/ginqzixhg.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gjzthbyqf.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gwabrbmas.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gcaubtnmt.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxjdedbgv.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/goixxhcth.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gcsbxzfab.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gztitrurw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gptketybw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/grmqnjsqa.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gdnqcacot.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gwediheju.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gfsmcyotj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gfcxjqxln.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gipzvonti.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gicytqfxt.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/giyzoovpc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/guceszmcl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/grgeaaidw.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gwtibhsgy.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gelseyylf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gdgbycxzx.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/godtsmhgq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gsjsmrypa.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/ggnpaxftc.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gopqvkmku.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.tarul.cn/Article/details/gaczbtjqj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gmkcqigdf.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gryamqylp.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gllwffgye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gnhbzxnui.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gabyqcwwq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gowzgqnzb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/ghthticqd.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzlfepgng.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/gkfnmtspj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/groebtvfo.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gjygjxybf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gmdrylzyh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/ghrihlpke.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gdvhkyvxq.sHtML


<!-- 参考信息 -->