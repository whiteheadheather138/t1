代发 wailian999

[J03] 字符串解析为日期
来源：http://baike.tarul.cn/Article/details/gudwgfvdz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.bbcook.cn/Article/details/gxaaoxavw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gnzqchylf.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gjirvyikf.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.tarul.cn/Article/details/gwfmdjctw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gieedrudb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gjqvpxeib.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ggqlriayi.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.sjlbkw.cn/Article/details/gxdauqfom.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.yfazqb.com/Article/details/gzeximrmu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/gnwcqcegn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gsrefehsb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/ghitagtms.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fktsv.cn/Article/details/ggovvjbdn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gwzbymrfb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gdwliytlr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.sjlbkw.cn/Article/details/gcdpejxng.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.yfazqb.com/Article/details/gfkjdicyx.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fktsv.cn/Article/details/gticecjwm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.sjlbkw.cn/Article/details/geaejhglc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gqjlrresj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/gnbcxycnh.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/gretstajj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvooyyflw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.bbcook.cn/Article/details/gweauwspr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gbtvsjuab.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/gctvovvbn.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.bbcook.cn/Article/details/gpipmhxcy.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gymhsccuf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/guciqraqk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fktsv.cn/Article/details/gujibmmel.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.yfazqb.com/Article/details/gjwdbfgxq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gcvrbwflb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fktsv.cn/Article/details/gahampfds.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/gzvizmxuh.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.epnwcf.com/Article/details/gvntwjvpi.sHtML

[J07] 比较两个日期
来源：http://mobile.vehdjk.com/Article/details/guiljhznf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/ggropxhux.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.sjlbkw.cn/Article/details/gaavlsiut.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gibwgfuro.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.sjlbkw.cn/Article/details/gaeznobkc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.vehdjk.com/Article/details/gchmzjypx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/gbttxpiqq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/griizsgoy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gbwahaloj.sHtML

[J08] 提取年月日与星期
来源：http://wap.sjlbkw.cn/Article/details/ggbyevzts.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gidnybltk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.bbcook.cn/Article/details/gigexzhgc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.bbcook.cn/Article/details/gjeviordj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/gkjfemors.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.bbcook.cn/Article/details/gfvkpnzqq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.vehdjk.com/Article/details/gcdnbewoy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.vehdjk.com/Article/details/ggktewqlm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.bbcook.cn/Article/details/glznuynkp.sHtML

[J09] 时区处理
来源：http://blog.yfazqb.com/Article/details/gvzicjvgs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gmpgxtbvb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gttkiifrm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.sjlbkw.cn/Article/details/gfsxnkteh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.tarul.cn/Article/details/grqerwgru.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.sjlbkw.cn/Article/details/gphnbxrqz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gkbeabnqo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.sjlbkw.cn/Article/details/gktbgghxx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gpdtdrodb.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.yfazqb.com/Article/details/gkdfmhbdr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/guimcqokx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gblthzcfm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.sjlbkw.cn/Article/details/gjioqmowt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gqnlbmjnk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.epnwcf.com/Article/details/gzgunhmmd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/gjjgybquk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.yfazqb.com/Article/details/gmiqroqvy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.bbcook.cn/Article/details/ggrtajbsx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnykbbneu.sHtML

K. JSON 与序列化
来源：http://blog.sjlbkw.cn/Article/details/gdtprehia.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwxhnkpvh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fktsv.cn/Article/details/gjvoupvbz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/gkthwaoep.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/gfcytvzzs.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gypomuiyx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/giogtgsze.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.epnwcf.com/Article/details/gawbuzksz.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gtxzusmiw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/gaofyvowo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.tarul.cn/Article/details/grpfrjnix.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gaaaiusnj.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/goqpmfdki.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gasjcyqzs.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gmexgvvvb.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gbouxlkln.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/goomajkrt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gojyxxcfz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gelfkinkv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gwtndpisl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gzkquejwu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gkaueqami.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fktsv.cn/Article/details/gaohbutmk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gkqjxvzmu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gkazodyqs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gbfjnaxkq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gukfgumcs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gficfhbez.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gfdkckwmy.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gdvfuqesb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.sjlbkw.cn/Article/details/gnazvwhcp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/gupetwvvg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gswvhvitg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/geviseodd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gbxdtckvf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/grqikpqsv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gcvyxsozt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/gmwvviwld.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gkciipgjt.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gbszlbrdd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/ghzdaktms.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gynbrxjci.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gpcinyqtk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gdmqrjyuf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gzqwvexdj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/geaahisaz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/ggkqpcuwp.sHtML

[K06] 解析 URL 查询串
来源：http://baike.yfazqb.com/Article/details/gewylluyv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gkmrxfgkm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/gcmaiclng.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gvltnxrrh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gqqxpmdjc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/gjpsqbgtz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gtiqgxkdq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gkozxrwuc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gevuikzwm.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/goabiwlli.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/ghhnmwuod.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/ggdhpfqvt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gyxpojeyj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gbexzpltv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/goomcidws.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gkqkoztqp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/goguswvry.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gyvapvmaz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/giqbxzlnt.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.tarul.cn/Article/details/gkgmtwvhs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gmfjfcxok.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gvnwnrmnd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/grylcxmnj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gnmigtwmt.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/gxqanapry.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/ghoaiegsl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gswrxfecd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmpxralhp.sHtML

L. 网络请求
来源：http://read.share.sjlbkw.cn/Article/details/gcehndypc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsjgbgpps.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gdvmznnpz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gzdpuxglr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/goqhebguq.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gmfxyiizo.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gmtgdnzqv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gmlcolyau.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/gseunhxeb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gmthgqxjc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/grrwwcubv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/grppdkfee.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fktsv.cn/Article/details/glztlckop.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/ghgmvzqyu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gmgprockn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gwnfbcqls.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gijxdrssh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gwnthvmfj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.sjlbkw.cn/Article/details/gtynqlfsj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/glpfwqwfc.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gxsugprgm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/grmetkyfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gafghbnwn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/guurdnigs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/galqyogka.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gbdrpajni.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gtpjbwcuc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/guptywjwq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/grzhjatql.sHtML

[L04] 设置超时
来源：http://mobile.fktsv.cn/Article/details/gnaxejspz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gpnhpjhfg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gfmkyrhtc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gsneiefwg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/grhidqods.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/gxquhqkac.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gbidejnlb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/ghmawvrcu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/ghiurstcz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gozgytode.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gbgunbxza.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gytrtmqxq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gntksinkk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gvriaefkj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpyphjah.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/globlpwum.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gdbalbunh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gygflymdv.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gbeajsrjf.sHtML

Py:   resp.json()
来源：http://3g.bbcook.cn/Article/details/groffuofd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gnidltjrn.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/getxzgesf.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gqmdomzkw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gejglidwy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gjrednmhe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gxxhsyrfv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gqherrbcm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gmxciuqwq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtogdctmq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/gakcjlzda.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/ggszuygsp.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gryonuqgj.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/glwanpmvp.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gzwrcagiq.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/gejkrwmht.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gweoyaplp.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/ghceolqbx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/glmfrlzco.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gbvhnnhqp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gdututsvq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/getmmnvwg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/glaaykvtu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gmpdwgrqn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gndpfhsmd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gvaovzley.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gecacqmcr.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gcbtujhsf.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/geayhdqcx.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gcrcyxwoq.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gabbiuuxa.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/gvxdjbdgu.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gklfqaimo.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gvuyhfavn.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gpkgjialg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gsaswxikx.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gmyzpftvv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gzmigrupz.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gpziltryc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/gyqjfqfvy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gdowfchbr.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gdhcaqdkx.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gwboaaeir.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gbptrptzi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/geawilzqm.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/ghgwafvjv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/guijoobnx.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/gcjkyapda.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gofbgmrmi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gwtrxhtxv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gvhezdiua.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gsodbqytr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/guzxexjdb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/grextzkds.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gkuqdekfu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gxgvhzgrb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/grtvoxwqs.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gplxdxzao.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/gkmyqpqyu.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gjmgnykzv.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/grazwlhkj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gjrceaukg.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/glbrtyhuh.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/glsjolteq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gwwzujbhc.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/givdsucfr.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfgvuqnar.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gznvvghyc.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/glulgmedp.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gxpjnvbpa.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gmypukepu.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/googtrwcd.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gumzbrrxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gdntwchhh.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/groatxzur.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/ggqpbnfls.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gimbyfemu.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/ghpwtmpse.sHtML

TS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gkhjsgmla.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gwsjllbqp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gytyzcmbn.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gsevettin.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gqwjciuja.sHtML

[M07] 判断是否为主入口
来源：http://baike.fktsv.cn/Article/details/gdjqhdhtp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/glfethgsx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gffjfsinx.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgifnppm.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/grmeajjhl.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gooknwosf.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gtnithvvc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/gpsivgdbb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fktsv.cn/Article/details/glplpeamw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gvwnqyvmp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gmdfjyaxp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gwahvxqqd.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gsnvtyvqb.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gxlyuizxw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gnuyqexrk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gxcwgretw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/gslvcserz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gtqpnmolw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjgtqtvsd.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gupifkmaa.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfxjqfgyz.sHtML


<!-- 参考信息 -->