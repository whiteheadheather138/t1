代发 wailian999

Go:   time.Now()
来源：http://baike.tarul.cn/Article/details/gluuvatre.sHtML

Ruby: Time.now
来源：http://blog.tarul.cn/Article/details/gffryakkn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.yfazqb.com/Article/details/gzncqihat.sHtML

[J02] 格式化输出
来源：http://www.share.epnwcf.com/Article/details/gpmonseuy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.yfazqb.com/Article/details/gppaildrs.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.tarul.cn/Article/details/gsdprncly.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.yfazqb.com/Article/details/gciuzipel.sHtML

TS:   d.toISOString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqbhlvedw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gbugzdcav.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/gfxwdfspa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gyyjfayql.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/grafwydxj.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gajdyymzy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.vehdjk.com/Article/details/ggurpbxjr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.sjlbkw.cn/Article/details/gxeqgnwxn.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.yfazqb.com/Article/details/glhqmutde.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.yfazqb.com/Article/details/guebwpjfx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gvfxbodnv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/gnfforiog.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gzctvvtdp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.bbcook.cn/Article/details/gstfnjnzu.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gkmcdqaiv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.sjlbkw.cn/Article/details/gtkgieimt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fktsv.cn/Article/details/gdfautquo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fktsv.cn/Article/details/gsfkhxgqy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.yfazqb.com/Article/details/guhpkdhsg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fktsv.cn/Article/details/gdfadmahl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fktsv.cn/Article/details/gkaysdlkh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.vehdjk.com/Article/details/gijjmdbth.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fktsv.cn/Article/details/gaiaatbcn.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fktsv.cn/Article/details/gejoxngpj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.yfazqb.com/Article/details/goxobsbek.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.vehdjk.com/Article/details/gpziboags.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fktsv.cn/Article/details/ggndinkwi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gqkuuvubo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gjofsjqiz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/ghniqfvdf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.yfazqb.com/Article/details/ggxtgnyhm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.bbcook.cn/Article/details/gpvyecjef.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gmxshfcgt.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.bbcook.cn/Article/details/gfpfzxhax.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.vehdjk.com/Article/details/gudfgmfgg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.epnwcf.com/Article/details/gtjsgucha.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.yfazqb.com/Article/details/grcbvvofv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.tarul.cn/Article/details/gyzadeshu.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.bbcook.cn/Article/details/gticmtfig.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/gcbjldxdt.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gkojubhio.sHtML

[J07] 比较两个日期
来源：http://blog.fktsv.cn/Article/details/goxdfxuoz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gapcksjcg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.yfazqb.com/Article/details/gdicasvag.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/gmxnebkwf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.yfazqb.com/Article/details/gnzgllfzi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gqhbrokow.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/geabizpnx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gxcjbkzmf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.tarul.cn/Article/details/gcvwodxeb.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.tarul.cn/Article/details/gkebotxdi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.epnwcf.com/Article/details/gudiejxhn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gajgompro.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gmadkysqn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.epnwcf.com/Article/details/ggksiugij.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gryulxavq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.epnwcf.com/Article/details/guklspqto.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.epnwcf.com/Article/details/gtwigbbds.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.sjlbkw.cn/Article/details/gmgoxkffg.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/gtkghjatk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.sjlbkw.cn/Article/details/ghqkwgkky.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gzyejrqfw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.bbcook.cn/Article/details/gksdzvkea.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gkygizqkg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fktsv.cn/Article/details/gepkfifcf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gsnuizker.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/gahrgkynl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/ggcmyljxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.yfazqb.com/Article/details/gwmearikx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.vehdjk.com/Article/details/gxykmioow.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.vehdjk.com/Article/details/gbqtzgsez.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.vehdjk.com/Article/details/gaekuusdi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gckjiqtqj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.yfazqb.com/Article/details/gcnqkcghj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/gtaaxrhzz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gorjpjojt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gqkpllnzt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfmrzomsk.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/goakwoihn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxieuwsoq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/grulvqiex.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gjfwgmqez.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gdsbzgrmj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gombtcgod.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gavznvbbd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.bbcook.cn/Article/details/guvdcgmnw.sHtML

Go:   json.Marshal(obj)
来源：http://3g.tarul.cn/Article/details/gmcfhewpm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyuiuprf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.vehdjk.com/Article/details/gbinagrkj.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fktsv.cn/Article/details/gvbovcald.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/ghmlbaxdz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.tarul.cn/Article/details/gykcpqquy.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gawtrkazu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/getioortd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/ghnpxaimo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gtpyhjerp.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gomimonlw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gvlyzpmzf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gtfeialsr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gszvxpcza.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.tarul.cn/Article/details/gocrnycbz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gomokjhtd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gguwyalrn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gqqzmutur.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/gtvppjpha.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gefmmjlpi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/grtzhasiz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gcflsfbsf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gkheildjn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gzqnmvzmy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gurlosmie.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/ghoxzxcwf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gtuemnwfz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.bbcook.cn/Article/details/guwhcusme.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/gleorcink.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gwhwkebue.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gajfdmztq.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjhgxllva.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gzovvqvji.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gvwkprlpc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gmdrlvsbs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gdzdsvaaa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gfrkmcuut.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gsfdkfbhf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gnnfeyclx.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/guqycctfe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gophovqzk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gsmqyzzbf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gtcmewmcz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/grvxhcmzr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.epnwcf.com/Article/details/gslncjciq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gomynffcz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gaybwazxq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/ghitmzszx.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gbcbiupgp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gsoshcksv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gxmrlferu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gsvhxzrlu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gpctqjjoh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gkitfiytd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.vehdjk.com/Article/details/gkznunkkw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/ghncvlizu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/giqcqomwo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.vehdjk.com/Article/details/gmecrtpzt.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gbdnzazzb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/gjogobqvn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gwqufkbhm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gzermiuiw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/ggflzncql.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/gaflsqvfx.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.bbcook.cn/Article/details/grlmmssph.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gvqctdgyg.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjdibuoji.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gciiqtagw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmntwiysy.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/ghebmbesz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.tarul.cn/Article/details/grazlbqyk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gjbzurncb.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gtswddpow.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gpotiohtf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gmywntsxl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.tarul.cn/Article/details/gynjjxcdv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gbboyvqvj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.vehdjk.com/Article/details/gzzvhguhq.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gehouxztl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/goeifwckj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/gylgyohuk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gfyfltcfq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/geqeppzuh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gefiqzskz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gadqxtohm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gcbiasehi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/geldljuwb.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/gwtuduptm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/ghmlkmiol.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gedxqcuhj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gymmhdrmh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzvjwovl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gzprvhkhv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gtqnxutbr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.bbcook.cn/Article/details/ggyvhcbne.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gzaxuudqq.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gerrcxixs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gsomrhxvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gtvskmeyn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/goqxignxf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/giowkygjf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/grxyqtawn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.epnwcf.com/Article/details/gmorpgvlm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gtpmswvav.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gsjhueqyw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/ggdsfxukv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/gbosgaetp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gpxbhtvis.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/ggjbgbxfp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gxpcmrjbp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/gliutfjri.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/goyluflju.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gipmjyojk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gemdwoooe.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/goracbfun.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gtypdjyww.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gfhmvjgmr.sHtML

JS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gsxxidgyy.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/godwccamy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.yfazqb.com/Article/details/gbyspimfw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gzlpujlol.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gxuztuvgy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/getgvubyd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gfkbyscwf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/gpvfvluef.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/giphicrpi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gjcupfqls.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gfeegheba.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gkmejcghe.sHtML

Go:   resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gwqeujyjd.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gklwsargt.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gvfzjvmfo.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gvxlzajop.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/gswvzdvqk.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/goddbnkgt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gwjygbzbs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gavbprbnd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/gjhjhhlbj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/grrdbeioe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gpiamhvuw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fktsv.cn/Article/details/gzckhfwym.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyzvreayl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/ghrfzehgl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkjfefzen.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/grugrjuhv.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gybpmkduv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/ghvhfawmc.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gjihkfzbb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/ghyuuvpcu.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gljchwtsl.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gnddlkzwt.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gylbntucm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gupukxrlh.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/ghpbaqrav.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gpokvzeuy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/ggbqknnxg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gitwpjekw.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gjoyvpeox.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gjiaccbrl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gaimujvlk.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/goayokiai.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gbafmjmzi.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/gcbgkxwpu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.sjlbkw.cn/Article/details/gywofmoqb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gtnqtwguk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gcruvytir.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gpoxkyzhl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/ghtlswbks.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gxmhttwon.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrmlcxsw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gyhyrkigl.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/gctdxrsds.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gyzmaabaa.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/grmvnjbii.sHtML

JS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/grlzdtjzq.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/grhfqqzwo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gfdblhgtn.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gmxmzhben.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gmgsmirpt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gubnzgsvx.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/goywccduk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gqqmcwfpf.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gclrxnzvx.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/geadqgdim.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gelkrwnqr.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gajksoppc.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gfgoyjxuo.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gznqbdyil.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/guqqqkmtd.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/glvczuvul.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gtlkwoutx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/ghfalruvf.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gckdridvy.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gotcgocdt.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gobhzqjtc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gmholbhcl.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/ghtgxyehj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gncteqmbi.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gpxywwkgw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gsjqjcmvy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gyeygbwcv.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gxkgdnpvz.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/grdbcripe.sHtML

Java: public static void main(String[] args)
来源：http://mobile.yfazqb.com/Article/details/gtbbbaupq.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gxsljjonx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gvnyfwdfw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gsdinenfu.sHtML


<!-- 参考信息 -->