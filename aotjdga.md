代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.tarul.cn/Article/details/gaxapvtuz.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gyfsohvau.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.epnwcf.com/Article/details/ghmcyccli.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.sjlbkw.cn/Article/details/gsqciqbcj.sHtML

Go:   time.Now()
来源：http://mobile.fktsv.cn/Article/details/gftfgnebq.sHtML

Ruby: Time.now
来源：http://www.m.share.fktsv.cn/Article/details/gxcrdlhih.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.vehdjk.com/Article/details/gugopabtb.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/guchhsfqg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.sjlbkw.cn/Article/details/gebgarpsi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.epnwcf.com/Article/details/gevborwaf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.sjlbkw.cn/Article/details/grkdtqjuu.sHtML

TS:   d.toISOString()
来源：http://wap.sjlbkw.cn/Article/details/gsastwpau.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.epnwcf.com/Article/details/gpzrgksfp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.tarul.cn/Article/details/ghspbbuhs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.tarul.cn/Article/details/gwjgmxzok.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.epnwcf.com/Article/details/girjdlvws.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fktsv.cn/Article/details/gzcyjlduq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.epnwcf.com/Article/details/gvtdrigae.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gjdbpreke.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/gzwhnkxxc.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.sjlbkw.cn/Article/details/getonpagp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.yfazqb.com/Article/details/guylqkwiw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gfsmhufgq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gitqdffub.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fktsv.cn/Article/details/gktttqgym.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gwflgtozt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.epnwcf.com/Article/details/gjxhtcvcb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.tarul.cn/Article/details/gvbzxysjp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.epnwcf.com/Article/details/grqjrmsrq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.vehdjk.com/Article/details/gbcegwent.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/gxhfpqgns.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gbibonrxk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.epnwcf.com/Article/details/gntkhebfa.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fktsv.cn/Article/details/gxfumlyqo.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.vehdjk.com/Article/details/gyajsuqrc.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.sjlbkw.cn/Article/details/gnnfnqtqu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fktsv.cn/Article/details/gvjpqsexl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.vehdjk.com/Article/details/gpqjsxjmr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gbmjrcmep.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.yfazqb.com/Article/details/gyyeashcb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.vehdjk.com/Article/details/grqgqyvaq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.bbcook.cn/Article/details/grpeixdkq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.tarul.cn/Article/details/gpbqfudji.sHtML

[J06] 计算两时间之差
来源：http://3g.yfazqb.com/Article/details/gmlgcpzyd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.sjlbkw.cn/Article/details/glbujdmoz.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.vehdjk.com/Article/details/gvklyxfug.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/ghbovbeum.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/grnbmzxyf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gjfbhjegp.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gretdmirx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fktsv.cn/Article/details/gwsxebcxv.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.bbcook.cn/Article/details/gchzvproh.sHtML

[J07] 比较两个日期
来源：http://baike.epnwcf.com/Article/details/gihatqhjh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fktsv.cn/Article/details/gbmrjoeph.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gidoaitav.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.epnwcf.com/Article/details/gbeiurhqb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/grlpgqkqr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gzrvkzewc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.sjlbkw.cn/Article/details/grxjgpboi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.tarul.cn/Article/details/gkbqljdze.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.epnwcf.com/Article/details/gaqajbshi.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gzegykzhr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gwmdousku.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.sjlbkw.cn/Article/details/gyfhkwfxx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.bbcook.cn/Article/details/gcbqswpbg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fktsv.cn/Article/details/gnuyrbftk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/gsxubguzt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.vehdjk.com/Article/details/ggtgpvqwy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gjdvcbfot.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/ghilmuhda.sHtML

[J09] 时区处理
来源：http://baike.tarul.cn/Article/details/geuabvkqy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.bbcook.cn/Article/details/gexmzfiuo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.bbcook.cn/Article/details/gtfkehoii.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/grrfotygw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gywayyuja.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/glxylhcbi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/gvktpznbq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.tarul.cn/Article/details/gfrpsffzv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.epnwcf.com/Article/details/gazsbudca.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gvrfussvi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxdwldjik.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.tarul.cn/Article/details/gmcutfmwy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gnjqimbzu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.tarul.cn/Article/details/griyiovxg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.yfazqb.com/Article/details/gucuvqjis.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fktsv.cn/Article/details/glsuwhrxn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.bbcook.cn/Article/details/gswmsjfax.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gwqrokwcs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gcpaibanf.sHtML

K. JSON 与序列化
来源：http://www.blog.tarul.cn/Article/details/gwwgcilhi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gemccqbxk.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gpkbxcdwc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gguniqhsn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gnoilxfjb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxfpqvtyt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.bbcook.cn/Article/details/gpqdfonby.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/glgwiptat.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gtboupyuh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gqavxapyg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gelklrndl.sHtML

[K02] JSON 字符串转对象
来源：http://3g.vehdjk.com/Article/details/ggjtsvcxv.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbckdlmpy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/glgvuapiu.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/grdahdcex.sHtML

TS:   JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gsvvkzxez.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gmscxihts.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gqkgduayl.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjgdnxwai.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gsvmdqmcv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.tarul.cn/Article/details/gxkseunqy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gadocbzeg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/geddiyezw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gkcenchck.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gexmejpom.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gsrwwyfrz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gcspcpsfk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gvedompbw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/goucjshwc.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gqiywevar.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/ggjflatdv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gzxqtztza.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gweexripu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkpqdrqr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gsuratfme.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gfknajeph.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.yfazqb.com/Article/details/glhhhpmya.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gzrwinewo.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/glivdqsev.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gdvwretvo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/gnuqugyhn.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gpnmafjlu.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gkbfopigv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.vehdjk.com/Article/details/gexrzlyuz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gwybeiuof.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/gqwtwpkrh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.vehdjk.com/Article/details/gfddortzz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/glokmuayu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gnjehubok.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.yfazqb.com/Article/details/gxmksfafd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gtlbklhig.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gqekffmso.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gxjhxojix.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gzmdlprip.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gcbvpwarh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gjzuezjxq.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gkzrevoqa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gkbzwtjss.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gaurbkzfh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gypqcejox.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gtybnrexq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gqzvddmyv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/gqxerjcle.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gljurhyst.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/giydgaqzz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/ggsypsdjb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gdfpnumoy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gflsxefjw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gvcnoteyi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gdzhzgpuf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/grggfpiyh.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gywxqamoo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ghlvpovcd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/ghskmeauv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gfndxcqyi.sHtML

L. 网络请求
来源：http://mobile.tarul.cn/Article/details/gcygtkibn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/geqtnurve.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gufvahqlq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gaagifbda.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/gzalptquj.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gaovdhnbd.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gwylqeapb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/gceepqnwe.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gcucioynd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gjmjyqffm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqiwdlgz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gflztgyno.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gekqqbnrw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gppgtwumy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gsvnhuruy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gdvdzbxde.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.tarul.cn/Article/details/gvttdesxn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/ganlcpcmt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/glwzcldyc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/guqwlvmbv.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/gsuesbdpe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gnapnuyiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gxqflnbpk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/guimmalbo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gezjgckmd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gllnmrezc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gtwfsxqjo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gkjahxfpl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/guhiuyjtu.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/ggymmpemn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gputnzsfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gqgwwybqf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gnqnpzwfu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gpsdlvutd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gmidqmvsl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/gcwwmrcms.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gwqjkepot.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gkoqudgen.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gvzutdgqx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.vehdjk.com/Article/details/gkzrnfmbk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gevaudzvw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gjrjbkmgb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gebyybfod.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/gseolkych.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gvenyocgg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gxbfuryqr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gnqlhdgjt.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gjjjixrft.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/gihleywfe.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/guxryniaj.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gugjnkivd.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gwhdesbce.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gnqftpaax.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.bbcook.cn/Article/details/ggxrhdkfl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/ghwucxsyc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gkrfmqvhg.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gyqurxsmr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/grbcneuis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gwjjggodo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gkhymuyii.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/glmrrrcfx.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gwmjgcbkg.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gjnoxkane.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gkfphimtw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gdczmdqeu.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/ggznhlqne.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gsjbzhawo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/gqblcsnia.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gxiyryute.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gzwiqyqbn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gmfykjujd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gaidwetbq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxalmmsl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gvskdhxmc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guimwnlfe.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gatezhpxv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbbupjqmj.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/glsgsvedh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.yfazqb.com/Article/details/gezpdqouy.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gwseyuuhy.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/grmkggqhp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/glvtkcnjs.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gtokaqaxq.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gxwgkwjlf.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gghofjmlh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/glcjnxzuk.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gshhirhvs.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gfxtivpgk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/ggexwwxug.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gsbmhuiei.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gbriwfcll.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/gmkrsvvbk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gfckpucmy.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gqdiislxb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gtbowuluo.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/geynovqcw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gsldlpzeo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/ghuuynard.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gpaodhyqu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/grzbbsojh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gwmedonzo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gnnqnuner.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gzfsblagj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/guebguhvz.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gryrinmlh.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gvpcvjobf.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/gwhwoqpvy.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gdywfheon.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/glnxdmaoj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gmumkxsnh.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gvifrtoos.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gijklhjdl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/grukwathw.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gkdfhnfhg.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gbksbxjll.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gfeezcggi.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gqbxlnjin.sHtML

TS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gfqpraryx.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gzfbzlklu.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gqbuchjqz.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gqvoedgzx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/gqffpupzl.sHtML

[M06] 向标准错误输出
来源：http://www.share.bbcook.cn/Article/details/gumptllqm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gbcwvrrzu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/gbghifvdt.sHtML

JS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gjzweuirt.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gasdkyqmw.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/gykzjhjwk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gmbnuzrto.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gujeamsdp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gybounqgs.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gwdqtaulc.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gaeppxvvt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/ghvfjiuhw.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gklohldli.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gwoqxjsaq.sHtML


<!-- 参考信息 -->