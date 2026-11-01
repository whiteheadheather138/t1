代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.epnwcf.com/Article/details/gadpoziwt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.bbcook.cn/Article/details/glkjxbkea.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.bbcook.cn/Article/details/gaoixjbyq.sHtML

TS:   d.toISOString()
来源：http://blog.fktsv.cn/Article/details/gbgpownbg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.epnwcf.com/Article/details/gxoiztldb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fktsv.cn/Article/details/gzzshzgsy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.bbcook.cn/Article/details/gnxkeeacy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.yfazqb.com/Article/details/gbavtdwxt.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.epnwcf.com/Article/details/gxucfgfgt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/ggbodzsmw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.sjlbkw.cn/Article/details/gwtmodarb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gkhnbtvxw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gaqcffmwo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gavsnrrqr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/ggttdbybi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gzwoigjie.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.bbcook.cn/Article/details/gslbvytgy.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gzqkbevjl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gegguswyd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/gdyhnhhsq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/gslbhwczi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fktsv.cn/Article/details/gjbukqlvv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.vehdjk.com/Article/details/gmkurchsg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.tarul.cn/Article/details/gnkwesson.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gfwiwjwvw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.epnwcf.com/Article/details/ggbmxawtb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.epnwcf.com/Article/details/gpexuntra.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gdsyjurne.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.vehdjk.com/Article/details/gjrfgdsjk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/ggcfiugpy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fktsv.cn/Article/details/gsuvqxfms.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.epnwcf.com/Article/details/gnimglhqa.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.epnwcf.com/Article/details/gqcsadhtu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fktsv.cn/Article/details/gpiwtmhqf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.tarul.cn/Article/details/ggoceolxn.sHtML

[J06] 计算两时间之差
来源：http://wap.sjlbkw.cn/Article/details/gugjhvzmg.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fktsv.cn/Article/details/gonmtebrt.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/gzlrvenkz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.yfazqb.com/Article/details/gargmkgoe.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fktsv.cn/Article/details/gzzbfyxel.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fktsv.cn/Article/details/ghqoxtqbo.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gzdwpsibx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gpuraebbj.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.epnwcf.com/Article/details/gsziamxgf.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gksueksyl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.tarul.cn/Article/details/ghpdagzyn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.epnwcf.com/Article/details/gmiepyspp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.yfazqb.com/Article/details/gubbhfxgz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fktsv.cn/Article/details/gsaeuvphu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/ghnyovhyd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gmkxiffsb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gexkffzeq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gxwcupnrt.sHtML

[J08] 提取年月日与星期
来源：http://m.share.vehdjk.com/Article/details/gukmahnng.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.bbcook.cn/Article/details/gxkowatyg.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gaprdhohu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.vehdjk.com/Article/details/gwrcsjtrj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fktsv.cn/Article/details/gabpibqrp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.yfazqb.com/Article/details/goyqigdla.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/ghqggeaer.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.vehdjk.com/Article/details/gmsrjrphj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.bbcook.cn/Article/details/gngozjcjn.sHtML

[J09] 时区处理
来源：http://mobile.bbcook.cn/Article/details/gqyszdcuv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gpzuyrlcm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/gnpliagyp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gvmhjabox.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gktlmqtfo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/gkloprkqt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.epnwcf.com/Article/details/gxiqgcppl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fktsv.cn/Article/details/gjwplqgto.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gjpiusgke.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.vehdjk.com/Article/details/gbkqevekd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.bbcook.cn/Article/details/gruaqnqam.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.vehdjk.com/Article/details/gsfztphwk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gylfcnnkr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.bbcook.cn/Article/details/gmcgtythp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/gabbjkwuy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.sjlbkw.cn/Article/details/gognofyxp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.bbcook.cn/Article/details/gpyfwxtev.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gqsdgqyml.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/genmawdeb.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gcmlncfdg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsiwllpur.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gblqfwphp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gwknmgpaq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gmfwojoyy.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/goaywliqa.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gusvezdye.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gqtqjixhk.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gtcfhlgxk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.epnwcf.com/Article/details/grxdpbkwo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gcofevpyn.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fktsv.cn/Article/details/gveyzpqxc.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gdwqmncks.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gqjvkpzrh.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gxrjhevbr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/guwawgsck.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gfqlzrvno.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/ggfphaufe.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gyzwrjdvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gapoiruru.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gcsxunvpg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gaxtzdxpe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gvdwbcugl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gbqmyxywe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/ghsjrlxfa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gzkxgqtys.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/giejrjych.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.epnwcf.com/Article/details/gyfvofvry.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/gtddxyizy.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/gyjjeeacw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gumvmivqv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.yfazqb.com/Article/details/gifweoowc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gfutqxvbs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gwnfsohjj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.bbcook.cn/Article/details/gtrjvhgoh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/glthprczq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gtmhpxnyn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gwqbykfma.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gnickrgyt.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/ghffbhcew.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/guqirzuko.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gfotiyleh.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gbpnvwztc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/glqdtxkyy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/gbqkulgjr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gdbnrypwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gobhrtldf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/grxhxmzux.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gsvyeplwx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.epnwcf.com/Article/details/gddgnvxhj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/glckoegjn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gdligodvq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gojpbedtf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/grmoggkyi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gknvaxvkx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gfjccppcm.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gjsjqaoom.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gevrrlbcm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gpfoakpux.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gdsetbazm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gklwmehwy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gdysexuxi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gecrearep.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gizwhejma.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gelqzpkaz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fktsv.cn/Article/details/gdoouiktw.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gcvytdmun.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gtvdiupfa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gpwosyvzu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gkbknemtp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gekvnuzfx.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gwnliwffz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gvfpoooht.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gykeoyjjr.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gavylbaxp.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/grzbvdvwo.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/grblxihsc.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/ghipdzxso.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gtoqrnlns.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fktsv.cn/Article/details/gmsfrwqqm.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gtpnvcmsj.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/goxlfurtj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/grjubkenv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gxtwirwcu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.sjlbkw.cn/Article/details/girlualgh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gnvovvzme.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/godqzbhtw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/ghqudgllm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/gphygxtud.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gcngkusvj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gtqwbszbv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gpilwlmxs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/gfiiiiiva.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gyguvwkxg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/gocbviwpk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gsedebscb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.tarul.cn/Article/details/gpvtmcovh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gdpqytayw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gwxknxyfs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/godirapwl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gycdlrdsn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gaogvbjbs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gfncneykz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gkvimvtbb.sHtML

[L04] 设置超时
来源：http://baike.epnwcf.com/Article/details/guxuzbwqp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/gsdkkdkka.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/glxppzvah.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gifulqoiq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gshfpmqso.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gforwgctg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.yfazqb.com/Article/details/gzoajjlul.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/ghyhtdsrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/guerxjdvs.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/gdfckfcnc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gxcwxpqtk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/gifyuaqpz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gagrraops.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gdswagxhl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fktsv.cn/Article/details/gfkwxiynj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gmahmmcso.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gffhnfokj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/gyiknvmsv.sHtML

[L06] 解析响应为 JSON
来源：http://blog.bbcook.cn/Article/details/gleblybfk.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gvuqpsfcf.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gxkwcfcun.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gofpfhwrr.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gawkfvnpv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/ghmklhdrk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/guhzxrzsr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/ggzbkayjh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gczfcljvn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gjjqnacbx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gmxicczxk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gmfbidtuz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gftdclurj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gmzrwiehz.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gcchqrpge.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gdkfyjjve.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gfctgiemb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gpzgilbqs.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gspwarumd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gjnnwwcwa.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/grvrrmgpa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/goydgentc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gvefqtjhv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gzlzsunoe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gkpcunbhp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gjwdnical.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gwjuizlmj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdbijowbz.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gbjougrmx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdomjhkuf.sHtML

[M01] 读取命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gfuqortlm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gwrornrsv.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gwfxxywej.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gjnlnvgik.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gxjovfayt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gjwtxmgza.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gabiluglu.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gojpixgwk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gmlxccfkt.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gqqpidrmu.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/gwfurwvym.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gxvtrpngy.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gzivklkfw.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbcikgzc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/goowxbfww.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gzpsiyvcm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gmljajeaf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.epnwcf.com/Article/details/gaczkrngt.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/gwftpflkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gbnkdmduj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.vehdjk.com/Article/details/gvhujlbmo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gqcwyzhox.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gzhpfickf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gxozzbfbd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/gfkkahiaj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.tarul.cn/Article/details/gswnemqfk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.yfazqb.com/Article/details/glcdxzvao.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gfrdeuvvc.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/glqshgsgo.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gmuarmbru.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gpbadgwze.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gvptibmkf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.sjlbkw.cn/Article/details/gnhitmuhc.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gwauycuwq.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gzzcwougt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/gjqhqhsls.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gfunyviyv.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gbggvmxev.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/gwltckgwb.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gvdociwkr.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gozuehsrk.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/garxynsjq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gboefwanv.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gjfnqbioa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gvfbxmspq.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/gdhpklxth.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gorfqlamo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gumotuakx.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gqcblcmov.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gllpcppwg.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gjckwctpc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gqoswwjwh.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gbuoytzot.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gfdrucrvd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/grdgblcrp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gxpqkcwse.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gclernfcn.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gcaiidcmw.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gmzsooymc.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/ggdylhlbd.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/germabybk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/ggjykhlmb.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/glgwbwpzs.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.yfazqb.com/Article/details/gduyvbttp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/gqlclxtsx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gmqxvixaz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gjobrwwee.sHtML


<!-- 参考信息 -->