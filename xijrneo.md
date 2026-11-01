代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gkogzojkd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrhbnmqj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gujldemlb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.yfazqb.com/Article/details/gjumjwwug.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.vehdjk.com/Article/details/gubhlnabm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.vehdjk.com/Article/details/gdcuthpuq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.epnwcf.com/Article/details/gqhqlwldb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnxsuylzz.sHtML

J. 日期与时间
来源：http://3g.fktsv.cn/Article/details/gjctfachf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gtwmmziwa.sHtML

[J01] 获取当前时间
来源：http://read.share.epnwcf.com/Article/details/gvycbungf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.tarul.cn/Article/details/gihfbzjqx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkihqczxl.sHtML

JS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gyxpcrbpg.sHtML

TS:   new Date();  Date.now()
来源：http://3g.vehdjk.com/Article/details/gmgnipbkt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.yfazqb.com/Article/details/gbibopzlb.sHtML

Go:   time.Now()
来源：http://m.share.vehdjk.com/Article/details/gajtxsjko.sHtML

Ruby: Time.now
来源：http://www.m.share.yfazqb.com/Article/details/gjmwieioj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.bbcook.cn/Article/details/glmsmktbi.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/gyqjbybxy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/gjqjhnudl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.vehdjk.com/Article/details/guveenhbw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.sjlbkw.cn/Article/details/gczbtgwqk.sHtML

TS:   d.toISOString()
来源：http://3g.fktsv.cn/Article/details/gudqpipdg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.vehdjk.com/Article/details/gerrqhvsl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gvrbuvtso.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gohfwfgpk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.yfazqb.com/Article/details/gqcsfkudh.sHtML

[J03] 字符串解析为日期
来源：http://blog.epnwcf.com/Article/details/grbgyncgf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.yfazqb.com/Article/details/gxtuoctfe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fktsv.cn/Article/details/guuzuoqdr.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gkewdprho.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/geyntjzfx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gvkyxoiyr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gpveimzet.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gwpqjydoa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gpdjhnusq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/gmvvykefi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.yfazqb.com/Article/details/geaoroubb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gecyojgog.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.vehdjk.com/Article/details/gvlzlsqzp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.epnwcf.com/Article/details/gislwfcoq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gwftujquw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.tarul.cn/Article/details/gpywcigjd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fktsv.cn/Article/details/gewmvurrx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.tarul.cn/Article/details/gnplvluuz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gjlmajllt.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/gyuysyzzb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gqlpdxrpz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gdjbvwnoc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/govmmdgqn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/gqfsinzmh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.tarul.cn/Article/details/gpwgowpfb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gxzlbzjze.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.bbcook.cn/Article/details/gdxviyaik.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.vehdjk.com/Article/details/gbghinjsf.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.sjlbkw.cn/Article/details/gysstzjog.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fktsv.cn/Article/details/ggjwyyulb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.sjlbkw.cn/Article/details/gtagsydyj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gtscdkcwi.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.vehdjk.com/Article/details/gbtiuhqzd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.yfazqb.com/Article/details/gmaxspala.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.sjlbkw.cn/Article/details/gdozzlfni.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.yfazqb.com/Article/details/glgvpoypv.sHtML

[J07] 比较两个日期
来源：http://mobile.fktsv.cn/Article/details/gnnzoksun.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gfmyjoxtq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.sjlbkw.cn/Article/details/ghdwaysmo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.yfazqb.com/Article/details/gvdeukgzv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.epnwcf.com/Article/details/glozoianx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/groajzgxw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.epnwcf.com/Article/details/gdaoxgsox.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gxvsqeiwr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.sjlbkw.cn/Article/details/ganexrszd.sHtML

[J08] 提取年月日与星期
来源：http://blog.epnwcf.com/Article/details/gyopdyvmp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.vehdjk.com/Article/details/gyinlxajb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gciozblcc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/guptehkbc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.vehdjk.com/Article/details/gvocnfjxe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.epnwcf.com/Article/details/gzfmfsman.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fktsv.cn/Article/details/gzbbzpmio.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/grrwzxccm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/gayldkibf.sHtML

[J09] 时区处理
来源：http://m.share.vehdjk.com/Article/details/ghokvnkfv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fktsv.cn/Article/details/gpfwkztzk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gekvnjlzq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/gmxaeodap.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gmsftwngi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.tarul.cn/Article/details/gozcfwgni.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/ggyvdupdv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fktsv.cn/Article/details/gesuiupwe.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.bbcook.cn/Article/details/gtfudlhsv.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gxinpursw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gmeatudhs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/gihofkqct.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.epnwcf.com/Article/details/gngpzrgph.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.epnwcf.com/Article/details/ghkzkpzsr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.vehdjk.com/Article/details/ggqrvhlcq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/gcjhkarqc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gxxvtjjqf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.epnwcf.com/Article/details/gcnayjjxg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggwfcmclz.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gltjlhejt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfcobprve.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.vehdjk.com/Article/details/ggrfarbzn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gpjdwqapm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gtlzshvkm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gvjgutxuw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gzqgufwuw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gdgwjojof.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gtybpwlfx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/gfijvdztv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gjrdadxyh.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.vehdjk.com/Article/details/gmaykiqag.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gclcgxsmq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/gunzqjblt.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/ghbmupxet.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/graqbpudl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gdyagtsqm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gubujrgte.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gljfbqpus.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gzolcxeez.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/geaecxqwa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gpbclnyty.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gigganxja.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gxpfimbwn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gdaofaohd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/glzuwyevr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/glrxnnqej.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gitnodzgr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.tarul.cn/Article/details/gkqmhvpop.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gdawpcaxb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/gykjntete.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gvbqckvpq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gdutfnrqy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gdvslypgq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.tarul.cn/Article/details/guszhkwwf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gzmcrrafb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/giynkrkwz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gynebvjhk.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/gyzarnxxu.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/giixcbvln.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhoyvysj.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gtxmjczxl.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gxakhacms.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gfavlpxjk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gljttcfok.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gujbxehdp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gfyirofzq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gqvsddcvl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/genfrmlaf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gvicrnsso.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gadekunnc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gqqnwmqch.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gthtekgce.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gmhhswegi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gbdogzmii.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/geuxbgojw.sHtML

[K07] 进制转换
来源：http://wap.bbcook.cn/Article/details/glchkrprc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gssznypnq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.epnwcf.com/Article/details/grbqgkppp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/ggcegapup.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/ginlbjmda.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gajhzamin.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gyknujdiz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gldmwwgfp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gjyycnkpa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fktsv.cn/Article/details/gdrtlagal.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gsmdturja.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/gvmxfafwc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/ggbpnqkpn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gqnvbmbok.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/gspsadqzy.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gsfbwvtsf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/grxkugoiw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gbwuramrz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gnfhutxot.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gelulxsfl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glzqipvxj.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gchdseevd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gcupatidq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/goawnwrap.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gylkwlhrr.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gtwmjojrv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.vehdjk.com/Article/details/geaymsuyq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gronxvbzi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gslzlywtf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gqgkpsxhe.sHtML

[L02] 发送 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gtscuxezn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gsslnpbie.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/glsyydakj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gvnvyeetz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gzvjswshk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/guvkdsvpr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/ghqwhconc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gaxdybkgh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/goaqrezdn.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fktsv.cn/Article/details/gduvczoyd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/glkiwngqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.yfazqb.com/Article/details/gfypnyffl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gturtlaww.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gbxfmevwu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gqfbrxzzx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gpwtdgwux.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gaojhrhek.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gjzqcyazt.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gwpzurwiz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gvuvequrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gwcxcopek.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gahvpivmq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/guxvrvvhc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gxqjkpsyd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/gnvtsnszw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/gconxpdgc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gxsfuyvgx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gjllloxpb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/ghtfzscga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gmulwxsqb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gpgihkexv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.sjlbkw.cn/Article/details/gewrzebfl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.bbcook.cn/Article/details/gueprmhiy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gpyneuxcn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/ggjwputuv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gogmayowi.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gntjjipma.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/gllwsclar.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gwghuhesb.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gzhumvnjv.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/guzgscpar.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.tarul.cn/Article/details/gdeiefonh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/grzwdwjir.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gnhxjjjtb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.epnwcf.com/Article/details/gmxvjtwgp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gqfkqnolz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gwnmhdkkg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gdlehlpfi.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gspfdclwq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/ghbwgcgkw.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gagzlcgkz.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/ggpkukfmu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gjwddimdk.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/grcdfinnd.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gkfmpdirh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gbcesvolm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/gwjurkwii.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gttmwjxkc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gzmltwzth.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gkaghjjrv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gogtseisr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gjpiyjbmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gtxcfuuch.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkbpfsabr.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gjkdzzyro.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grspwuxap.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gmttcxpnl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gpfxiakmq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gnqsnqldr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gxybnavuj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggabrwqyg.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gxdhuwfgt.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gbeyzubgq.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gtvcjihyq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/guqqwaxec.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gmwztdaqv.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fktsv.cn/Article/details/glpckoodb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fktsv.cn/Article/details/gayyvdqlr.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gfjgmhvrj.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gbkldsvtt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gnxsftojz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/gccsdzwob.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gjbcgftxt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gtnosvidx.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gkmldpxps.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gmxiijwoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gythxsyjt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gspjbbecf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gzzyalroq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gbuwphvwh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/gwyvnplnq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/ggyujjgoz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gihdcfwqe.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gwjahrntq.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/gpxserfcx.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/ghnldltwf.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/ghszkaisi.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gulxigjhk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gynrbxirf.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gxzucidts.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gfnnawtov.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gqwmsmctj.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gynzuyrvp.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gbajghfpo.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gacaujvxb.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gkanikxwt.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gztptgpjj.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/guqlouamk.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdnzyznda.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gnnkdoqnh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gycaxvqwx.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/gejnnbitx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/grjvzczcq.sHtML


<!-- 参考信息 -->