代发 wailian999

Ruby: s.scan(/error/i)
来源：http://blog.bbcook.cn/Article/details/gshheevgx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/galqwmvvn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gyafvwqkh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.epnwcf.com/Article/details/gfwhwqqho.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gjhguwjok.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.vehdjk.com/Article/details/gvmhlmvwq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/gdsxelgov.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.vehdjk.com/Article/details/gkchfyxbl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fktsv.cn/Article/details/gtdheczsw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.vehdjk.com/Article/details/gssjbaync.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fktsv.cn/Article/details/gqcoacchj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gnwvffuex.sHtML

J. 日期与时间
来源：http://mobile.fktsv.cn/Article/details/gallwwczs.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gmbpzmsul.sHtML

[J01] 获取当前时间
来源：http://read.share.bbcook.cn/Article/details/gftxirkqt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.vehdjk.com/Article/details/gaxjqrtdj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fktsv.cn/Article/details/gpgppuuhg.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.tarul.cn/Article/details/gwzprevse.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gwejsvadw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/ggnvmqikz.sHtML

Go:   time.Now()
来源：http://www.m.share.yfazqb.com/Article/details/ghtmencxr.sHtML

Ruby: Time.now
来源：http://m.share.fktsv.cn/Article/details/gbwwqlswo.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.sjlbkw.cn/Article/details/gvhwmmqql.sHtML

[J02] 格式化输出
来源：http://read.share.bbcook.cn/Article/details/gnttmnmbd.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.sjlbkw.cn/Article/details/grchdiceo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.vehdjk.com/Article/details/gsegowpye.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fktsv.cn/Article/details/gjzcfajui.sHtML

TS:   d.toISOString()
来源：http://mobile.tarul.cn/Article/details/glqhnpmpx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gwxbdnvmc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gwrosdyhh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.tarul.cn/Article/details/gehjyhrdk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.vehdjk.com/Article/details/gtvrohsnf.sHtML

[J03] 字符串解析为日期
来源：http://wap.epnwcf.com/Article/details/gwygphpkx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.sjlbkw.cn/Article/details/gfzrptlbf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.epnwcf.com/Article/details/gxhqenmsi.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gumtfneco.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/geshkdofp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/guentkulq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gehxjppdq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gsngflyfm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.yfazqb.com/Article/details/gvxsbldrb.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.tarul.cn/Article/details/ghqrvfbhz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.bbcook.cn/Article/details/ggmpktdrr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.sjlbkw.cn/Article/details/guhrrpjrj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.yfazqb.com/Article/details/gihsgsmqd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gktbmsnvz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gelpvvccj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.bbcook.cn/Article/details/gtoasyjlk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gfiqeitkj.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.yfazqb.com/Article/details/gqgfzckcm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gtppslpwh.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.fktsv.cn/Article/details/grzebneka.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.bbcook.cn/Article/details/gbtwxwjtj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gfootqgnn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fktsv.cn/Article/details/gwupzefay.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gynjzwzdw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.yfazqb.com/Article/details/glguwlvfg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.vehdjk.com/Article/details/guqovlwwk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.sjlbkw.cn/Article/details/guazmvobs.sHtML

[J06] 计算两时间之差
来源：http://m.share.epnwcf.com/Article/details/gnpucwhpf.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fktsv.cn/Article/details/gyktrruyv.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gkahuobhe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/gegduzugz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.sjlbkw.cn/Article/details/gyrcyjrbw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fktsv.cn/Article/details/gqoislhfu.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fktsv.cn/Article/details/gitddvntw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.vehdjk.com/Article/details/gcytvyoet.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fktsv.cn/Article/details/gckjjbdjf.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/gpjsontkl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gspbdeykt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.tarul.cn/Article/details/gthdyfefn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fktsv.cn/Article/details/gvhkwqvjr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gchnttcsx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gcdnaxdae.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fktsv.cn/Article/details/gmyzydsid.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fktsv.cn/Article/details/gwskaiphd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/geotwrcld.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/ggrobxsrp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/gqleauoua.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.tarul.cn/Article/details/gxyulstbm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gwrdgotfp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.sjlbkw.cn/Article/details/grtqdfvzl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.epnwcf.com/Article/details/gjdaptgyp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.bbcook.cn/Article/details/gwhzzxalq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/gxdetujjk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.tarul.cn/Article/details/ggzcvhsip.sHtML

[J09] 时区处理
来源：http://3g.tarul.cn/Article/details/gsxtsmsnq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fktsv.cn/Article/details/gdmbxabvi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gycvwjbpr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gkrplsuoj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fktsv.cn/Article/details/gnwlfvlrp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gtawifvwy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/gnhkmdnba.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.sjlbkw.cn/Article/details/gcqrwvxxd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/glskjkwrw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/gjuhlptjj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/gvnqckqvf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/gacdwawpd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.sjlbkw.cn/Article/details/gxzmrwzod.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gqsbbojcn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gujuyefpi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gfposvyko.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.sjlbkw.cn/Article/details/gjxegtnoo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fktsv.cn/Article/details/gcasoqxmz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcnwvkpwt.sHtML

K. JSON 与序列化
来源：http://wap.sjlbkw.cn/Article/details/goyjadlmj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gvtnwlmhd.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.tarul.cn/Article/details/gotmdiuim.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gzeziimzt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gqszdyulb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.vehdjk.com/Article/details/gqfkifaph.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gellvadvs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.epnwcf.com/Article/details/gsnflenfz.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/gpllurvtu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gdoqlmgib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/gkatxmays.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gxfxolmku.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gtrgsonbe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/gtycmpjny.sHtML

JS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gmvqmggel.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/ggytaunux.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/ganbmlvxi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gccnkiinc.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gibmeiosh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.bbcook.cn/Article/details/gzxzhffyu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gnkihcuta.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gdwrjnpyu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gzuijzxcs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gfmvhjvit.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gvqanybwv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/glxmchagj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gcqbyvagf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gqgnlqjep.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gjkjjgzyx.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gfsuugzdt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gnxwghoyo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gpnphcwrw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/glcmhkhzm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/godqexgvm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/ggshynxie.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gubzqkjkh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gyiniiwwg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/ghepzwjep.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gvwujcexo.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fktsv.cn/Article/details/guiwaodih.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/ghayhapbh.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/ggoygqpdb.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gfaljkudy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gwaygeigf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.vehdjk.com/Article/details/gsdksuzrp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gvrzpgthu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gkihyfqej.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gsszyaoto.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gvnfszkkk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.sjlbkw.cn/Article/details/gzujmkrgd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gindmfxxw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gszosypoz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gzssykfql.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/ggpwljbol.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gvhuwfdlp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gossfpjtu.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/ghjkhibvb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gbdpjrojh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gpaujnfsk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/glizknlnu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/glxhboftd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gllkdywel.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.vehdjk.com/Article/details/gfqsrzrmz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gnkpxhwlh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gbaiqxbnj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gnorqtilp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.bbcook.cn/Article/details/gvgahwagq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gwpmzqtso.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/guewfeofr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gyazacgxq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gaedoidkl.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gdjcnzqge.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gimmxbjea.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gdzehntfp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/getyjuvut.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gzafpcxyu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gacvkgexw.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/gtqlcnwsl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.tarul.cn/Article/details/ghhupixev.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gdmuaecen.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gsemxuzmq.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/grcnetupd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/ghxqvpqls.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gtjvqihqm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gpjxueqpf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gsrgkpczp.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gtoixswdl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gcysixmdp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/gjoyfffqz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gkaladaaj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gvkqaazar.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gxijojxfr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/gperxzbag.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gngaskdeb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gizwgtbnl.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/gpzydmssy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gzxasggxc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gnaaopeqc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gihrifteh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gzibdhjwk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gckdomlwc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gauovgdkj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gieqygdiq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gsgvpikdm.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/giiebqxfk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.sjlbkw.cn/Article/details/gmssnnzgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gpvsccqzu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gtkpxapej.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gocgojbll.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gqgbzunld.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/ggsdsqdpp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gjhrbqbkv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gzfafzjei.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gunmafpxj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gmjoargka.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gxbuhgglx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/glhuqtuuj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gvtcfysxf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gjnsoquwd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gvkvownlv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gscdzwgvu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/ggewthnlz.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gpuvexxqy.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gxekfbwrn.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gurghstsz.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gkkplwbqp.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gqhvtfnxt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gedzkgmtf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/glkidkwhe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gvmciczzs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gbudaotkp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gjafyvtiy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gyegowzjz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/gaczxrpph.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/ghoyrfsuq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gdoddxvjd.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gpluqkwil.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/ggyujcoau.sHtML

Ruby: resp.code.to_i
来源：http://read.share.yfazqb.com/Article/details/gffsauwyg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gmqrqlrbu.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gklzknjqm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gmgjdgvcw.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gnkduiyul.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsumcgdj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.vehdjk.com/Article/details/gmsesnmyx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gocoevogk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gtsizuxqz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gtvpyuxio.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gftevfsak.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkkdqjvtu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/geqbakbgc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/geszubplr.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/glofojwuw.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gudvyjqpd.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gugqxrxgc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gqccspbsb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gaaddxjeg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gzupevrem.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gnocuwjin.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gjhurynfs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gfzpffbnx.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gtrklrfcb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/ggtuuxugu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gysczcmwh.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gviiiiivx.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gpxejwmov.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gxzscxzkl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gvllsskhf.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.yfazqb.com/Article/details/gspqwfauw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gfksfdvpn.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gtmmumipm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gspryldpw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/gwgwqhfoe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gcoxinocy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/glocrbmkm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/grtxwjlud.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gfrrrltzk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gltlgmcbj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gsxgylhll.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/grxywgrav.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gfolzexzw.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gfamjnpwb.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gmpozbuqz.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gctqvbmyb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gvlqlqubl.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gwpanenve.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/gbypirnfg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gtihozqed.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/ghgxhzxjs.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gkehdwpgi.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/gkwmnpgcr.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gmybcveyv.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gugghglas.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gkgptcjdo.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gbbygvabb.sHtML


<!-- 参考信息 -->