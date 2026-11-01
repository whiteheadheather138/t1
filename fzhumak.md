代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.yfazqb.com/Article/details/gecjmejcp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.sjlbkw.cn/Article/details/ggbfcjrze.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gecvsehwo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gobpnisbl.sHtML

[J03] 字符串解析为日期
来源：http://blog.sjlbkw.cn/Article/details/gerlzezuk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/guudqgoug.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gneqdlwdg.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/glinnjieg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gkssffccj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/glxbxtiub.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gttgebvyd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gpvjbnhtd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/goauqsuuh.sHtML

[J04] 时间戳与日期互转
来源：http://baike.sjlbkw.cn/Article/details/gfhnqgmeq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.epnwcf.com/Article/details/gswtktysb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.epnwcf.com/Article/details/gyiyausgm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.bbcook.cn/Article/details/gpnenxyoc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.yfazqb.com/Article/details/gokqbohll.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.vehdjk.com/Article/details/gzmaqkmzc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.tarul.cn/Article/details/gcdbdrekj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/gxjquyqrn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gokhhbcje.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.epnwcf.com/Article/details/goxnmsqxc.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fktsv.cn/Article/details/gisnvjrhn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.tarul.cn/Article/details/gschzmtlw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gbgnxuojq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.sjlbkw.cn/Article/details/gibwseomo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.epnwcf.com/Article/details/gcxaywbpz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.yfazqb.com/Article/details/glkohqiox.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/gwejezjzt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gjlxkselh.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gujsxbovo.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.sjlbkw.cn/Article/details/gzvfdwbux.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.tarul.cn/Article/details/gnbzgugiy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/gqtreymtp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/grarpndbg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gxgbdzeml.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/gyezujrdu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gokxtfvqw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.bbcook.cn/Article/details/gqdjxzsjx.sHtML

[J07] 比较两个日期
来源：http://mobile.yfazqb.com/Article/details/ghefddplz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gbxixxzdh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gbuzdljty.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.sjlbkw.cn/Article/details/gvylyrhwp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gmwmdrqbd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.tarul.cn/Article/details/gpsmmjveq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuawgzgy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gbgjghqth.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/gsvuzxfwx.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fktsv.cn/Article/details/gzthnvuql.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/gaexqbbgz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.epnwcf.com/Article/details/gdmbqogpg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/glncastkf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gfnxqinjw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gwlnymjxs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gtbfzwrsu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fktsv.cn/Article/details/gsqkdacha.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.tarul.cn/Article/details/gqrkdolqw.sHtML

[J09] 时区处理
来源：http://3g.epnwcf.com/Article/details/gqhtedxpj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.vehdjk.com/Article/details/gcctfzcoj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gbypdyyvv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gilxiiofw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gwknfzory.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gqnicyxjv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gvekdezai.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fktsv.cn/Article/details/gbpdkpcqk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gvwgznxkl.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gtnbrgcws.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/guqmzipof.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.sjlbkw.cn/Article/details/gxleadkmr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/goebioczk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/guuwvoaxx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/gyctkjjbp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.vehdjk.com/Article/details/gbnsjqcxr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/guqivvfwa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fktsv.cn/Article/details/gdyzgqkza.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gauaddipq.sHtML

K. JSON 与序列化
来源：http://www.m.share.yfazqb.com/Article/details/gtwouogus.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gscomujsh.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/guegupspx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gsktolgav.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gewhbwaby.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gifbtlodu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjepqlkph.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.yfazqb.com/Article/details/gqrjdeyzv.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gmwibuvzd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/glrjvjkmn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gclrliatp.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/glfykinyi.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gqibzxovq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.yfazqb.com/Article/details/gtaitvwmd.sHtML

JS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/garlitkhh.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gddbcvxvh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gqkeqwvou.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gdehupmdx.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gbpwxsgxs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/gaicxehgc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gpnfhcenk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/gyeqxwjdf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gjseilxdq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gsitkdwoq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gcvjuwmxd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.epnwcf.com/Article/details/gzdevefcy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gcamhwknb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.yfazqb.com/Article/details/gsmwkwpir.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gkdmmbsul.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gpoitftui.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/ggqysuubm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fktsv.cn/Article/details/gdfpoqoum.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gdpfibpto.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gknlqkmzs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gtxhroceo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gusqzoiqt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/giiwsrdon.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gcfaixtrv.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gfikhyytw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.bbcook.cn/Article/details/ghlfvhqcx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gvpgomqtr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gcmzblnyy.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gqllqxtvx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gvjfuswvv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gviwbqnwp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gssgxnrgh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/gpuuxzwnj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gdbbfhmak.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gpwwjgkdl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gkylgtbih.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gnjfqqokb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gdqwuimuw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gihqucpxr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/glabfshus.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/grsimvmyu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/grblkkpqo.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gjkymeoiq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gewpzibna.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/gdpextcbr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gzugcmfgn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gwwriatyw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gqeixadez.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gzqohfqsy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gjktuuizn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gsphjpbzj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.bbcook.cn/Article/details/gazumzqil.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gfoepwkke.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gphamzntw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gmbihbllk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gdwxegliv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/glewcitfb.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gbcxoryik.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gzoqlsexc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/graqfwlwg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gemsqpmoi.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gufilrfyo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gweqhlter.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gcluyasej.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gjywwbxzj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.bbcook.cn/Article/details/gavhtmthv.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gpgmnaurw.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gerspezeh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/guozepzgy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/gjetfouwo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/ggiknatfr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gspcnicwk.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gkeylvdwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/geiqghqgi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/gftjdtcnv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/grmwcptve.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gshalkskb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/goawxijab.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gqnniryls.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gcqsbtcvh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gbpefihqc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gfcnhkjfy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gwoedfgfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/gedoelybq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gmlxjfede.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/guzglhbaz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.tarul.cn/Article/details/gtffiosru.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gztqahwap.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gwjoknngg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gvuapystd.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/getvguerw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gqpvmjddj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/ghdtabrys.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gfpkujwvj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gpnpupuqb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gyzdzyelt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gahdexhgl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/ggndzbyag.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.tarul.cn/Article/details/gkbnbrmkx.sHtML

[L05] 上传文件（multipart）
来源：http://wap.sjlbkw.cn/Article/details/gpqbsxmgk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gpjlufmvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gtjinuwxk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gcibmttja.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gvdvuinpa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gfwbuzift.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.sjlbkw.cn/Article/details/gtxejmumg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/ggycexmos.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/gimfqwewr.sHtML

[L06] 解析响应为 JSON
来源：http://baike.bbcook.cn/Article/details/guwgmftvq.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gcrbdonuw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gagstpffb.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/guwqbyfta.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gqjkntbqz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gabikmtmf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gvoguxtyn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gaffaaltx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/gwiftbfoj.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/glncsulnz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/giieecwno.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/grdhqopua.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gsguqwjwv.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/ghgfiiyvr.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gpjmrtvej.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gqoyufpfk.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gfckjheym.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gijuecqbc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/ghqcztonp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gvogpvqmx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.sjlbkw.cn/Article/details/gstrbuoud.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gfodaqugq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gbfgluzhe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/guufvuaev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gjekgjdol.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gpkszzcrr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/glspcouub.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvquczumz.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/ggowdotgw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqdubwukr.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gardxwqve.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/ghseucjij.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gvytkpwuw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gchklcgiv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gyeaowsdd.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/giirpjnhd.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/glkvwyego.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gikbqvome.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gsftmytgj.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/glfypzgjg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gpemeaojz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gsqdgymqe.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/galynjwhw.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/grapmxpzk.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/grxkubtbe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gbmwzzzcy.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gsvrmsqyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/ghpzkesuu.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/ggmwaqyne.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/gwcxpfdgo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gxqjbfhwl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/ghesxavuf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gsskosoxu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/ggadyqoun.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/ghlcebfye.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gqqyxwnah.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/ghacolznx.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/glrhfcqnd.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gzldjnpvn.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gfuchbvnl.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gklkhdbdo.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gbwkbzhzk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/geucagzku.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gyzeyadln.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gbetcbybb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gpphymfzb.sHtML

[M05] 设置退出码
来源：http://wap.tarul.cn/Article/details/gskabxoxh.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/gxbaddwpa.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gccyzzwel.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/glxczsiov.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gqpdkdlqk.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/grlwlslzq.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gghbutfbj.sHtML

Ruby: exit 1
来源：http://3g.tarul.cn/Article/details/giekwfjns.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gguvibjbp.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gsanoekrl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gbwptusgt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gpjfiigua.sHtML

JS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/guwohffal.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/grafcpjqz.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gwzndojka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gwsuewvzd.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/gpwvajdom.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/glichgabg.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/gnahjpdro.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/glxkcgned.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gkioclhvd.sHtML

JS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gblwxgkbn.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gtayjjpwf.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gcybdrwsq.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/ggscbzhgz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gzfqomdpy.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gdqnfohbg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gcpvmcige.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/gpgintgaw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gcngycupz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gdedtzwrg.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gugmmdfrs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gqugvnjfc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/gvmlvbwlu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/ggnobgrfa.sHtML


<!-- 参考信息 -->