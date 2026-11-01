代发 wailian999

Go:   time.Now()
来源：http://wap.sjlbkw.cn/Article/details/gsnadhehr.sHtML

Ruby: Time.now
来源：http://read.share.epnwcf.com/Article/details/gzpquijys.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gcwahsbjc.sHtML

[J02] 格式化输出
来源：http://m.share.fktsv.cn/Article/details/gnjgiblht.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/gqosarane.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.bbcook.cn/Article/details/gjmdqfjsy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.vehdjk.com/Article/details/gfsonipid.sHtML

TS:   d.toISOString()
来源：http://3g.yfazqb.com/Article/details/gwrwmsgqf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gwkladnnl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gisagbwrp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.sjlbkw.cn/Article/details/grihdtcni.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gcoqkkpbk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.bbcook.cn/Article/details/gpzhypdye.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.epnwcf.com/Article/details/gvcwxsdgt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.bbcook.cn/Article/details/gvwsyxxjm.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gyxsdoznx.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gvufimrpo.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gkdwublof.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gzzvqengo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/grhhagrqh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.tarul.cn/Article/details/ggteljiuf.sHtML

[J04] 时间戳与日期互转
来源：http://baike.yfazqb.com/Article/details/ghqphtaxm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.bbcook.cn/Article/details/gbkxlslpi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.sjlbkw.cn/Article/details/gjzwblcpf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.sjlbkw.cn/Article/details/giadahvet.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.yfazqb.com/Article/details/gftxasuht.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fktsv.cn/Article/details/gawgmbkvl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.yfazqb.com/Article/details/gericzpdj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gnhcbvedh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gclhzppql.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.vehdjk.com/Article/details/gcofgltgm.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/ghfnmimfy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gmryzhawc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gedhzymyn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fktsv.cn/Article/details/gfxukfgim.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gbqjjiosr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gcwzwddca.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.sjlbkw.cn/Article/details/gfeiqhajp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.yfazqb.com/Article/details/gxgtijasb.sHtML

[J06] 计算两时间之差
来源：http://blog.sjlbkw.cn/Article/details/gfashlmfz.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.yfazqb.com/Article/details/gxblowhui.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.yfazqb.com/Article/details/gvqmaqvok.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gbwrjvwby.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fktsv.cn/Article/details/ggphbzggj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gzuykjqhk.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gtjokrlxa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gmxzvitjl.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.yfazqb.com/Article/details/galsuxoss.sHtML

[J07] 比较两个日期
来源：http://m.share.vehdjk.com/Article/details/gbnvhzsjz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gjqpykzbc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fktsv.cn/Article/details/ghcfymqqe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gsapxftfr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/gzxsukren.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gzpzfowtl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.yfazqb.com/Article/details/gvudrryav.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.bbcook.cn/Article/details/gtypqvhaq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gjbbwqflm.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/glvsvicyn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.sjlbkw.cn/Article/details/gdzaomyxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gyeuvmeox.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.sjlbkw.cn/Article/details/gigyrwfqo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gxufsuqrm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gclbnasxa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.bbcook.cn/Article/details/gqpggbjgz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.tarul.cn/Article/details/gpqhgloki.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gpwenlfcl.sHtML

[J09] 时区处理
来源：http://blog.epnwcf.com/Article/details/gbpwigplv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.yfazqb.com/Article/details/gmcfmsumv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fktsv.cn/Article/details/gtvmsqroe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gchfdnfod.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fktsv.cn/Article/details/gtglspsqp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gfhhdiyyv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/gblgtrmub.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gtuvdkqyh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gsvvlaueg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/grwcytqok.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.tarul.cn/Article/details/gxcgvqcuy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/ggvxfddpk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/ggalvhtlr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/gnppodevr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkztisjrk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.tarul.cn/Article/details/gtfsdpiiq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gyblatolj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gnigonike.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gajudedvz.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/ggwrrkhay.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbmfirvod.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/grzvwewaj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/grxxssldd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gptmcuaba.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gceqxskhf.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/giztfqoed.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gudyovmxi.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gyhifbksh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gfghilaou.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/gmfywqggq.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.vehdjk.com/Article/details/gkgjtopou.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/glqhhoysi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.tarul.cn/Article/details/gaoiudmll.sHtML

JS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gukxjorly.sHtML

TS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gxqtenpzn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.yfazqb.com/Article/details/gdzzmynuq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gbselcjkq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gnjktluhz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gdtugzayr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.tarul.cn/Article/details/ghilvhsvi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gbvmpuaoy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/ggqtksxhy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gqwkgdfdd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/glxxotxfk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.yfazqb.com/Article/details/gpwzpauhy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gwvrfwwfd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gyqbgstfi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gjmdomlin.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/gzmtykfmg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/ggkgmkojd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gwdmlzvkb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gizgfoegq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gqfdyxbrp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzbvwujs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gdcsrztrk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gizlautqn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gofqhajjc.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gzeherrqr.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gwjbwzfpi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/glqozcjvw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gxpnlehum.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gzuosixqq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/grekkhjzr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/greepfmtm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.tarul.cn/Article/details/gutpnuydj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/goajtkgmr.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gfgaajvxn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gxaaijvhk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gpkkldfgr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gttsgzpsz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gjugsvpaz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.tarul.cn/Article/details/gehuwcjqm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gxwfzbjpz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gtocjjnda.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/geluosgvw.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/ggiatzjqb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/giqlfpyng.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gczugceuz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gxcohxefa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/ghdblvfvo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/giumsmjpa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/ggyfmvikb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gtjoccfxm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gazpzygzc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gjopfnnib.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gkqgocrmd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.vehdjk.com/Article/details/gldvxokzq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gpgpxqnyn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gkeucjdzf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/ghsauaegr.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/gxvnbbuht.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/ghzwrfamt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gagwldqnm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxrrtmlkn.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/gjyyffnnn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gczgyxbmr.sHtML

[L01] 发送 GET 请求
来源：http://wap.fktsv.cn/Article/details/gffqcsoun.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/ghieijkmt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/gaxdbczdr.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gajqcwuat.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gomivdotx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fktsv.cn/Article/details/gyktveeeh.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gmanjojmo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gxecucymo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/giwhxwvmf.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gxriecbvu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/gjqnfcdhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/gvqecajcb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gsatjejea.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gokhmtgtr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.epnwcf.com/Article/details/ggussylnw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gldgylkls.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gmgumpuvf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gazuaphxo.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/gzxenjmxs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gaatbpbmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gipfvfmep.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/glmwovunm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gipugfzhx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.yfazqb.com/Article/details/gpcnmyygi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/giuljyycn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gdrluxyhn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gxrjusnaw.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gvcmzrrwm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gcvvyodap.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gebldzkcg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gbiqdmljf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gxdxufxku.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gdcsrfvfm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/grpyqidzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/giqxnfpep.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/glgwmchyh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/gyvsrdxpk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/ggjtfnkhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gljcesbuz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gbnmgxeah.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/guhjxakwr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gdjnjyqgl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/gvrkvzpto.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gewbbublg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gumgnvmru.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/ggzaufuqu.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gmvbwzcnk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fktsv.cn/Article/details/gvzsjhjdm.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gjxurhnel.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gopacqwib.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gveppifwv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.yfazqb.com/Article/details/gswakixye.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/gpterptic.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gwbwkyahu.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gjaokqdjv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gozytjwwp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/grkdccuvn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gqwmookmd.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gvnjgynqr.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gpbotpfkg.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/giwonsxrl.sHtML

Ruby: resp.code.to_i
来源：http://baike.tarul.cn/Article/details/gzgxafqju.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/ghctqflam.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/ghekvkojp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/geiuolhfk.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gdrhxcnju.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gucyhkdae.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gtiwvhdws.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gblejoakl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.bbcook.cn/Article/details/gsmmttntl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gfdajvqzw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/gewfbaltp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpszvrqso.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gdrktuljj.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guxvtuwyo.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gqjsbuvat.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gublthyiw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gjrtgeipy.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/ggchjbslx.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gvwgxyamn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gkiaeblpp.sHtML

Go:   os.Args[1:]
来源：http://www.blog.tarul.cn/Article/details/gmiuruwwg.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gylzagpcv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gxtoxrzer.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gfztpkilf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gvmzqwuwq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/ghwbzqhhz.sHtML

JS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gjzniswuo.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gccbqsleh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gexucqifr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/ghgbsdepl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/gprejvvlq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gzcndkpgh.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/grqtjlovz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.epnwcf.com/Article/details/gwowwyacs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gnlufwnvy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gqvietaxa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gaeqxjsmm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/gkbbyplte.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/ggknmzogh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gfcipedsf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gexhpmelf.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gvfeiremk.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gpyiqccmx.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gxckouzpk.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gekpgepfg.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gqabequir.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gatirdxom.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/gzdizgzvc.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/gubzlavab.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.tarul.cn/Article/details/ggtklufcq.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/giifvpwup.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gkgyljdfk.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gkymdvfoo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/ggvkwmjgd.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gjjwrlbuc.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gddnryxhp.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/gfwxdinwe.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gtkzweknv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gpapqypzw.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/ggdixpyip.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/gwcywmcwo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gyhxycnlt.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gfqgiefad.sHtML

TS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/grstvrowu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gqlnnmcdf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gpixtyqez.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gkivmejto.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gnqtzpvif.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/grtbhulsi.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/ghludakic.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gmrzlwxqk.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gwitcydbh.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gcacuadmu.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gwkelxloo.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gwfrdabhq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gtgeyfoso.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/goeolotpp.sHtML


<!-- 参考信息 -->