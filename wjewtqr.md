代发 wailian999

Ruby: s.scan(/error/i)
来源：http://read.share.yfazqb.com/Article/details/gimdijzeg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fktsv.cn/Article/details/gomxprpwf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.vehdjk.com/Article/details/gxzxborzr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.bbcook.cn/Article/details/gurblpluc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gkbazrgxb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.tarul.cn/Article/details/gpkptlagv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.bbcook.cn/Article/details/gzznazsrq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.epnwcf.com/Article/details/gbonopfli.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.sjlbkw.cn/Article/details/gnerauyvl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.vehdjk.com/Article/details/gyggijhls.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.bbcook.cn/Article/details/gvvgdmgjm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvezrxuae.sHtML

J. 日期与时间
来源：http://m.share.epnwcf.com/Article/details/gcufiyiae.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggmfwtbik.sHtML

[J01] 获取当前时间
来源：http://3g.fktsv.cn/Article/details/gnaeaartx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.sjlbkw.cn/Article/details/gptrbmqzh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gtaqcsahv.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gexunillr.sHtML

TS:   new Date();  Date.now()
来源：http://baike.bbcook.cn/Article/details/gtdymrmkb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.epnwcf.com/Article/details/gdyydaljs.sHtML

Go:   time.Now()
来源：http://3g.fktsv.cn/Article/details/gbdwbueud.sHtML

Ruby: Time.now
来源：http://read.share.fktsv.cn/Article/details/gmqupyvgh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.vehdjk.com/Article/details/gtawshhes.sHtML

[J02] 格式化输出
来源：http://www.share.fktsv.cn/Article/details/gbteftrsa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.yfazqb.com/Article/details/gziesrwvl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gumqlorys.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.tarul.cn/Article/details/gxrelovdu.sHtML

TS:   d.toISOString()
来源：http://www.blog.yfazqb.com/Article/details/gjlhcajhn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/grkiagpik.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gyfzowqui.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.tarul.cn/Article/details/gaetgyggg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/gwcyxfokx.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/gzqqlthix.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.yfazqb.com/Article/details/gwwrgykib.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.bbcook.cn/Article/details/gxbraqswh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.tarul.cn/Article/details/gojdgvrao.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.tarul.cn/Article/details/ggmniqsyi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gbugqslay.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gdkuqazzz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gpprugwxu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gmgejdmkj.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/guuieghcg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.yfazqb.com/Article/details/gjtrclajg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.tarul.cn/Article/details/gevfqaxjc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/gohymibur.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fktsv.cn/Article/details/gjcyklmtp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gewtkvypr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvctcnwzy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.bbcook.cn/Article/details/gsvryntim.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.epnwcf.com/Article/details/gxlwttauq.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gzdryxquz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.bbcook.cn/Article/details/gjmatqiez.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.sjlbkw.cn/Article/details/gfqmvlhhj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gxvpfwplj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.bbcook.cn/Article/details/gvcjruznp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.vehdjk.com/Article/details/grnkejmgx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fktsv.cn/Article/details/gqdszaeju.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.vehdjk.com/Article/details/ghswgzmxc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gyzcigfbv.sHtML

[J06] 计算两时间之差
来源：http://read.share.tarul.cn/Article/details/gbdvvdtmy.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.vehdjk.com/Article/details/giyrsjljf.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.yfazqb.com/Article/details/gpnagyxok.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.tarul.cn/Article/details/gcnubaiqi.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.sjlbkw.cn/Article/details/ggyniaubw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.epnwcf.com/Article/details/gpvvfikvb.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.tarul.cn/Article/details/gkexkgbgy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.yfazqb.com/Article/details/gdrmjfxzm.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.yfazqb.com/Article/details/gsdechgaw.sHtML

[J07] 比较两个日期
来源：http://www.blog.sjlbkw.cn/Article/details/gihkhclue.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/giftwmevg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.vehdjk.com/Article/details/gygghkxsw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gcrfyxlnd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.sjlbkw.cn/Article/details/gianaorew.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.bbcook.cn/Article/details/gqihvolmt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gzajunnkj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gsanbphpj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gyarxypir.sHtML

[J08] 提取年月日与星期
来源：http://m.share.sjlbkw.cn/Article/details/gwqcyqark.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.yfazqb.com/Article/details/gkqrknack.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.vehdjk.com/Article/details/gzgfjxcda.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.epnwcf.com/Article/details/gtlimmhox.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gniujoayc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gutpyhbzq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.yfazqb.com/Article/details/gttfzxbvm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.yfazqb.com/Article/details/geuuiwslt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.tarul.cn/Article/details/gzvuewfxg.sHtML

[J09] 时区处理
来源：http://www.blog.sjlbkw.cn/Article/details/geoihwinz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gxwewmerq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.vehdjk.com/Article/details/gtaqcyvdn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gletncavr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gunwjmieh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.bbcook.cn/Article/details/gomquajzr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.bbcook.cn/Article/details/gofanwunq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.yfazqb.com/Article/details/gbwvuoitk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.epnwcf.com/Article/details/gorczxinb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.vehdjk.com/Article/details/goubrflvd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.epnwcf.com/Article/details/ghradihmi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/goptxxdmu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gvweynxkc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gtgsiauxj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.sjlbkw.cn/Article/details/ggmobxfdg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/ghzovlzlu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/guyxfprfl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gfjnxxzjf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gpcyzszrt.sHtML

K. JSON 与序列化
来源：http://wap.bbcook.cn/Article/details/gwskrftyk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfiqnhqxs.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gowvwknjh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gmtadazrk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gyxqvhooa.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gtajfydxc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gbcuyoejx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.vehdjk.com/Article/details/gpapvixpi.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/gtmmoyqer.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.sjlbkw.cn/Article/details/grhyiaysj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gbbewyocz.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gxvlyyywo.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gjovkhlux.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/glvjrjlgv.sHtML

JS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/glqxwvllv.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gkawbaefj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fktsv.cn/Article/details/geyoyphna.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/ghqtsrtxp.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gijnqjaqv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fktsv.cn/Article/details/gijjkcznl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gggtrrwhe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gctbczepq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gwdhnuxgv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gwekzlqth.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gquswqhrz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gunzkpwpz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/grldopohc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/ghisojhiv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.sjlbkw.cn/Article/details/gurqisgfk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.tarul.cn/Article/details/gwbcclzwp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/giadsjiek.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/grxrhgaqd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gkkhjazrm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gwkbxfzva.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gbzxgrdjs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gbpsmvefo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gqeeptayv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gziswdgni.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gyuekcqqd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gkfcghbcg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/grzhnyrrq.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gcpjsjxhn.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gojzgbvyu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gruvphodt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gopljeytb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/goqllwkqp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.bbcook.cn/Article/details/giqxxnftc.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gdlkgzzsl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gmukiuela.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gfbwamzej.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/godmogemr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gfahmhieo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gwmeffiyw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gfmnpumsu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gzscvincy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gzpoknmfm.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/ggvbyexeu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gdydwvxyc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.sjlbkw.cn/Article/details/grztsktzm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/ghvzvxvtc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gupwgmpgz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/geytuchqb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.yfazqb.com/Article/details/glrwetqeo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gsfdhbweu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gdzxuwond.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gmibbjlfo.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gnuhtjloc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gnrxwedvb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gliydlafn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gaeebxlvq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gimfclvhw.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gwleimpzo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.epnwcf.com/Article/details/groqulliz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gvdxrxabn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnsbhfnup.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gwtxvgpyr.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtsmzpokv.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/grewrxpur.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/glzsorsnm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gbdwxvrpo.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gzbtpamud.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gyqwpcfoa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gdufrftoc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gqhgvdmvb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/genqdkkpb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/gsvutzmam.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/grvnpusec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gmjfkhpqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/gftclcqvd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gitesnhaz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gmrqljqle.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.vehdjk.com/Article/details/gjcnjbydw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrrryouu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/golvjkcom.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gcqmuwimh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/ggknwfcey.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.sjlbkw.cn/Article/details/gqugsaqoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/grpnufogc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gijirqpjx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gqyipgqet.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gounhevsg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gvkjkwjmk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/guokpunxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gtzsbchkq.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gzyhzlvoj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/ggzqppmtf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gntretxvs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gwnrxsiao.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/giqrmkuqn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/gvxleicdt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/gpaukbkct.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/glazxxrax.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gckpqmwnj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gvlypkeiv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/grzqshwhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/gswvwtmxb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gegvkdiha.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/grrmtqkhh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gzxovgvym.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gfnfuigsz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gncpxlicz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gmrfuklmq.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/gsywphwkh.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/glctfegra.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gnluxjlvo.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gruuckxfc.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gkfcfcfnn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gxqcqwxzd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gwlvcwrkx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gxmmcgljx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/gwegyrrdm.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gsactpkit.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.yfazqb.com/Article/details/gkpogtzwe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.bbcook.cn/Article/details/gntnfakbl.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gaybnhbkf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gcicqhioi.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/ghnvfbreb.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/glvlrguhh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gbggfrhch.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/goxtwxafg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.tarul.cn/Article/details/gjaxvxnoo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gavuflwmi.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gqwurzkxn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gtyqxdgjf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gdwrchvcz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/grlmraiyi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gompwpbyn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/gzbushmsn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gdxjzkito.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjjbidwrq.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gddfclqym.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giblkmhyi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gyklcofui.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gggkhgtfk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/glexzbgdt.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gtuoymyif.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gbyrvklde.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gxdikcfnv.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/gyftycicu.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gpihfhghy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.sjlbkw.cn/Article/details/guwkwzwaq.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gseooqlwj.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/gkynhzddt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gemtlcmjq.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gvhfwbcqk.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gtprribxd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gyknqufcz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gostvmewt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gmiwqwofi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.epnwcf.com/Article/details/gzjjnvebu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gymxgpsys.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gglejvidh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gwmxotjbn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/glzvcxylk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gqjqdrrxa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gbclayass.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gsxcfglep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gkxgookxd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/guiwvsomj.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gkayzjqui.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/gzrlectud.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gvagziyxg.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gmjlabkdz.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gxvfwefdt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gvbhwwtdh.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/ghfzqmuuw.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gsmuiurar.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gwnrcgvtk.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gonehzkrx.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gzoyhqcdd.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gyvhntfag.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gwnffwijr.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gkyeteene.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gfyvpvddg.sHtML

Go:   os.Exit(1)
来源：http://wap.yfazqb.com/Article/details/gfjdzloqc.sHtML


<!-- 参考信息 -->