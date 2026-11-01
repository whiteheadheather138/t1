代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.sjlbkw.cn/Article/details/gtuobiqos.sHtML

TS:   /error/gim
来源：http://www.m.share.vehdjk.com/Article/details/guptdzebw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.epnwcf.com/Article/details/grysrmvwf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gcynbacom.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.sjlbkw.cn/Article/details/gyinotiai.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.bbcook.cn/Article/details/gtljyavss.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gbpptfomq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.yfazqb.com/Article/details/gnpkdpcmp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.epnwcf.com/Article/details/gsaetolmo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.tarul.cn/Article/details/gbefprboq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/ggkjksxnd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.yfazqb.com/Article/details/gbwqumpue.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.tarul.cn/Article/details/gzsevgzvy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.vehdjk.com/Article/details/geypchmab.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.epnwcf.com/Article/details/gwxvjlsfa.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdstkoqzi.sHtML

J. 日期与时间
来源：http://www.share.tarul.cn/Article/details/gujvdyijb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtheubvcv.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gvzowwlpq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fktsv.cn/Article/details/geyeycqww.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gldurrrld.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fktsv.cn/Article/details/gvefxichh.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gavatlcxi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.vehdjk.com/Article/details/gqmqnrveg.sHtML

Go:   time.Now()
来源：http://wap.fktsv.cn/Article/details/gaydbwrmb.sHtML

Ruby: Time.now
来源：http://mobile.sjlbkw.cn/Article/details/gnbaaadps.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.yfazqb.com/Article/details/grdrbhwms.sHtML

[J02] 格式化输出
来源：http://blog.tarul.cn/Article/details/gloowrtfh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gqmznxnwd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.bbcook.cn/Article/details/gukhkkkcu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fktsv.cn/Article/details/giztvdvhn.sHtML

TS:   d.toISOString()
来源：http://baike.tarul.cn/Article/details/gzyxrvsmt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.yfazqb.com/Article/details/gzvrsqjom.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvbvdebn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.epnwcf.com/Article/details/gwnwhoera.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.sjlbkw.cn/Article/details/gjmxjwebz.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gggqllqqd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.tarul.cn/Article/details/gbyxhfjvr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.bbcook.cn/Article/details/grumocdtz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.bbcook.cn/Article/details/gzrixwmwt.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.sjlbkw.cn/Article/details/gcngjshqw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.tarul.cn/Article/details/ghawyxuxm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.tarul.cn/Article/details/grfpzgjhb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.vehdjk.com/Article/details/gavqdzrxo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.tarul.cn/Article/details/gzvnxfuke.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/gjmvbnqjd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.bbcook.cn/Article/details/gpjnbjaih.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.yfazqb.com/Article/details/gsqrpsbjo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.sjlbkw.cn/Article/details/gxmxfiwzz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.epnwcf.com/Article/details/gnkopaceb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfdzomwd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.tarul.cn/Article/details/geuhegkyt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.tarul.cn/Article/details/gcvwyekeo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.vehdjk.com/Article/details/gnjyomewc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.tarul.cn/Article/details/gedjxzxvo.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gikzbdziv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gxdpcypmg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.yfazqb.com/Article/details/gamzspecd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.sjlbkw.cn/Article/details/ggohvatdf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.tarul.cn/Article/details/gtkhuwloh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gssopgksi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.vehdjk.com/Article/details/gesnwbrje.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fktsv.cn/Article/details/gbycwzxkq.sHtML

[J06] 计算两时间之差
来源：http://wap.bbcook.cn/Article/details/gambvxowk.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.bbcook.cn/Article/details/gzfykihbf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fktsv.cn/Article/details/gjmehnjnh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gmcysfsem.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.bbcook.cn/Article/details/gjvshbmnz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.fktsv.cn/Article/details/gskciootc.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.vehdjk.com/Article/details/gktyfkior.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.yfazqb.com/Article/details/gqjejnomx.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fktsv.cn/Article/details/guxpsgyig.sHtML

[J07] 比较两个日期
来源：http://m.share.yfazqb.com/Article/details/grgeiugkd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gpltsjkss.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.bbcook.cn/Article/details/gnbzquvuu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.epnwcf.com/Article/details/gnvhrhsfv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.bbcook.cn/Article/details/gebrmoqzz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/gujvicxnl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.bbcook.cn/Article/details/gttnasslx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gygaslozr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gsqrbxpcr.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gxxjvlthb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.vehdjk.com/Article/details/grqfnlirz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.vehdjk.com/Article/details/gkanslltg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fktsv.cn/Article/details/ggowactyn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.yfazqb.com/Article/details/grferylvp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.vehdjk.com/Article/details/gqtcuehov.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.tarul.cn/Article/details/gfyjjfjhj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gppuepuub.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.vehdjk.com/Article/details/gznvdpddg.sHtML

[J09] 时区处理
来源：http://wap.vehdjk.com/Article/details/gsyfqebrc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gmricmwvs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.vehdjk.com/Article/details/gbybpndsi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gtdlqhprz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.epnwcf.com/Article/details/gsvmvfwme.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.epnwcf.com/Article/details/guompulud.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.vehdjk.com/Article/details/gghnsdemf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.yfazqb.com/Article/details/grsaoyxmz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.epnwcf.com/Article/details/gopqouccx.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/gzxzmhscx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.epnwcf.com/Article/details/gmwkrwgws.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.bbcook.cn/Article/details/gtulymytz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.sjlbkw.cn/Article/details/gpcltvqry.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/gpygprwcj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/gpzexlryk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/gaitbqann.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.yfazqb.com/Article/details/gcqeuyrds.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gichwwhyx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guvbducpo.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gpotvqpor.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqkxvchrh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gwddvgvgc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gyjaoqyls.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gsduafojv.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.bbcook.cn/Article/details/gokokroov.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.yfazqb.com/Article/details/guprbtajr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gazdemmbn.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.tarul.cn/Article/details/ghgkfafpo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fktsv.cn/Article/details/gsqvvqgrx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gegibxidw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/gpgywzipa.sHtML

Py:   json.loads(s)
来源：http://read.share.epnwcf.com/Article/details/gwxjzuebs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/guqkvwrjo.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxuiwwkmk.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/ginvohwev.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/ggylhhjzq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gozjhdfza.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gduwdjirj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gswpsqllf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gvxbelktb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gvvfxtiyq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gizqnofvi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gaucufapb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gkdjnjlje.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gfhjumbeg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gndsymfvz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.vehdjk.com/Article/details/glumqwfkk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.bbcook.cn/Article/details/gefhkjqtt.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gjweirnsv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.tarul.cn/Article/details/gziuhxtlp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gxylfxdnv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gfrnbxnsc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fktsv.cn/Article/details/gdghjyios.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gwmmyffks.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gpvjcrjyd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/goqpeymnz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.yfazqb.com/Article/details/gespwggxa.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gxgizrihp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gbszxciyv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gygdeqzjs.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnyjbrofc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gemypfgsa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gimejafgu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/gtihxqeck.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gbhqmioep.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gqfgtmnka.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gwupfyvoy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gyttafmzm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gutgmgznq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gqvoyldbx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gwocnjxgw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gtovvrauk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/grzsqxqhx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gsbtdfhkc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/geidxdjvn.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gxgpgwkeh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grphzreyo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/gtbxkvdlc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gcysimxix.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gjncywryb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/ggdugyfzu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gpronjedu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gzevgnhgf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gvqqrajdo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gmmgojtqc.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gibrdbylk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gzpqwikgv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/gtwxpbgip.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gnksbarkx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gbcduhewr.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/ggvkvlwoi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gbuwtzxbe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/grmqbqsyx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glpxzcums.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gwlclhzkj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gdkrwiptl.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/ghajkuoan.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/gbxnddaqa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.sjlbkw.cn/Article/details/gkidmddvv.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/gxeymhlai.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gwnqedyti.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/gigwrrobq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gucpcgpyy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gvyozudjq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/gkpihcsdv.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/gljeunbmb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gzlxtevwu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.bbcook.cn/Article/details/gsdxelknw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gdaadgpdm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gtkndeype.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.vehdjk.com/Article/details/gulmithay.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/gpbblfetg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gtmlykwiw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gxwxctwuh.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/giwvbyzrq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gjguetsfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gokxtlzvt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/glehfwjfe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gslbkfkbj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gmssffmdi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gxwpxxlkm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gjrtjdowh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gmxkzclgt.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gfzsokmlu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gvlrlnmik.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gpjajeklb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gshkhwunq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/ggslimlfl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gdsegfjxr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gslgpnxkg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gyzhiyywx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gpiiuxdeo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gfytyyceq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gqxwtwlsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gtwpxhcsd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gxatpgtos.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/glzqnphns.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gcxrafuye.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.sjlbkw.cn/Article/details/gcqkxshsl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/guaafsnqw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gewvaujdm.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gudjlruvi.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gvvcvjamr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/gppebmxzy.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/getxgfrem.sHtML

TS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gwklepegk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/geivjyhpd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gbsewvwbm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gxxtvwfdn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/ghsvtitks.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/getgqmmsv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gyqistjfx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/gvjnqilny.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gmfolttcj.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/guzbjpkeu.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gcogrdrzz.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gvrxvcqnm.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/ggcuoscho.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gxmaimewz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gozfwklqe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gwwptjtli.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gcatdghdh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gyqppesql.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gqhojzvhj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gbcwhdjzj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/giuecmytd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/ggvhxpuin.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gbquvalkh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmqzakour.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/ghatxuhuc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxopcquka.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gvynddghn.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gzctdfraa.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/guacfjiqa.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/goaywghmn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gdrvjhfqt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gctqaptky.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gndscrpju.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gxtiddcgj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gzmwfbapz.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/gwkcubibx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gdgwnwfix.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/gudscypqg.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/ggvmjilqu.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gozvboryh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/guiuydeaw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gsnpgwayr.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gibdiphrs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gsgbsexza.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gasmgcfcv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gquggkibb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gsuddfacu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfbdtpxq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gmethcpoo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gmvvkqiki.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gbbfojczh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gorbuljqb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gkjeltihj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gektisgwf.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gbfchijgc.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/ggbkxtnjc.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gytpdwpnm.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gdgceevca.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/gajjagqdl.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/goreudvwt.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gslpdnpkn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gwxriyugw.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gjjuklxuy.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/glwidbmuv.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gjtgislgs.sHtML


<!-- 参考信息 -->