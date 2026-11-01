代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.epnwcf.com/Article/details/gkiaslnhm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.vehdjk.com/Article/details/glcghrncw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.yfazqb.com/Article/details/gjtujwwmy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.vehdjk.com/Article/details/guemgjred.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.epnwcf.com/Article/details/gzgyqwiyq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.vehdjk.com/Article/details/gvzgvtikv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/ghyrwxteb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnlyavsep.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/gxdxjuvim.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gafsnajpm.sHtML

[J01] 获取当前时间
来源：http://www.share.yfazqb.com/Article/details/gjllfpdqr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.bbcook.cn/Article/details/gdsdsmney.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.sjlbkw.cn/Article/details/gakhbeoxs.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gvesetkds.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gmxmgmvpf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.tarul.cn/Article/details/gmgltvxgl.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gzlkawwtt.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/ganzhnhlc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.sjlbkw.cn/Article/details/gumqpyjlk.sHtML

[J02] 格式化输出
来源：http://baike.yfazqb.com/Article/details/gmdowqllk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fktsv.cn/Article/details/guwgrpemo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gkyyuohlb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.vehdjk.com/Article/details/gxblurfnr.sHtML

TS:   d.toISOString()
来源：http://wap.yfazqb.com/Article/details/gvttkbtve.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.vehdjk.com/Article/details/gktcpgrgr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.vehdjk.com/Article/details/gghcfamls.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.sjlbkw.cn/Article/details/gxojsjadp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fktsv.cn/Article/details/gwusyuvgj.sHtML

[J03] 字符串解析为日期
来源：http://m.share.vehdjk.com/Article/details/gpwuxchyb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.vehdjk.com/Article/details/grarprngh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gyaecshqz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.vehdjk.com/Article/details/galhgixmg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gvgsqyfcy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gyytidxdv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.epnwcf.com/Article/details/gsjcxcjts.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/gmlagkgnz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.epnwcf.com/Article/details/gykjjvycx.sHtML

[J04] 时间戳与日期互转
来源：http://baike.vehdjk.com/Article/details/gaohjsgnt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fktsv.cn/Article/details/glvmevinp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.vehdjk.com/Article/details/gyskqigrq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.sjlbkw.cn/Article/details/gcvjvjsbt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.tarul.cn/Article/details/gwkwbrzau.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fktsv.cn/Article/details/gfkjpaxex.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.epnwcf.com/Article/details/gxbzeoiwv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.yfazqb.com/Article/details/gtetxdeim.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/grerrzzyy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.epnwcf.com/Article/details/gxdclfuet.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gevnhfzis.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.epnwcf.com/Article/details/gnjykjrdu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fktsv.cn/Article/details/ggfbkdnap.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.sjlbkw.cn/Article/details/gevujrgll.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.sjlbkw.cn/Article/details/gzofwljdr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gfbanvfci.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fktsv.cn/Article/details/gflsijfmj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.bbcook.cn/Article/details/gipxohxqt.sHtML

[J06] 计算两时间之差
来源：http://baike.yfazqb.com/Article/details/gztncyzxj.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.bbcook.cn/Article/details/gcxkvksjo.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.yfazqb.com/Article/details/gwrwnaazj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.epnwcf.com/Article/details/gdhwzlwlw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gngsngebb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.yfazqb.com/Article/details/ggnoyaiku.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.bbcook.cn/Article/details/gmzckycgx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.yfazqb.com/Article/details/guaawudcm.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.sjlbkw.cn/Article/details/gjurfvqdv.sHtML

[J07] 比较两个日期
来源：http://www.blog.vehdjk.com/Article/details/gsgaszile.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gxsutxcod.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.tarul.cn/Article/details/gnmcyindw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gfpnbhjjm.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fktsv.cn/Article/details/gljtulpnp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.yfazqb.com/Article/details/glxvcibfg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.yfazqb.com/Article/details/gfmclbfuh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gnqizudye.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gqlbtjsnp.sHtML

[J08] 提取年月日与星期
来源：http://blog.yfazqb.com/Article/details/glpohksgr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gfavfgzex.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gbibfuyoi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fktsv.cn/Article/details/gbocjvwij.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.sjlbkw.cn/Article/details/ghdkjdkkm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.sjlbkw.cn/Article/details/gcvmcrjpz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.tarul.cn/Article/details/gybmvhycd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.sjlbkw.cn/Article/details/gfwrvfpwa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.sjlbkw.cn/Article/details/gjuuysmvp.sHtML

[J09] 时区处理
来源：http://wap.epnwcf.com/Article/details/gadwwvsjs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gneqapvws.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gftirueaz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gykhtzxod.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gmobawiyb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.vehdjk.com/Article/details/gxofhefdf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.tarul.cn/Article/details/gtyaoxymy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.vehdjk.com/Article/details/gkihxnbmx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/gehqssqxf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.epnwcf.com/Article/details/gdcqicbmo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.vehdjk.com/Article/details/gjdohmygb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fktsv.cn/Article/details/gatcqdmbq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/ghqoghgbr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gszhfrrlb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gsnfyjqnk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.epnwcf.com/Article/details/gnzduoata.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fktsv.cn/Article/details/gjduhurui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghowbtmqm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gpjoqrbbv.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gsrinldoz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsybvuzes.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/ghnxbgvcj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/grsemueyy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.vehdjk.com/Article/details/ghfpljysr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gypnotrsu.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gsdamqvqx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/grnhlgblz.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpyezzzrg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/gmzdkykox.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/gdwieaipl.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.vehdjk.com/Article/details/gdoirojzf.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/guclfoosu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/gleblwjlu.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/glmgftfnh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gvmwnkuhv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gzymexaqz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtktxvrkc.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gmlvrvolg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gtimgxmxk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/geufbcrzd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gkxvhgsie.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gtzoowpxe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gyydxphih.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gvycrnncv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.epnwcf.com/Article/details/gcdqeisrh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gqhoqxyld.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqmfeqsqv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gdcbzvqvi.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gxedfodkg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gwjlfjiic.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gtkmyzddl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gipxhumff.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gttistqvc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gkfmoynms.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbmzshhj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gyikuzwky.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/ggdjnyrkx.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gucauldaw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/ghucszroq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gwcdvbshb.sHtML

JS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/gqydfwjzw.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqsvjdytd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gwkrwewzv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/gcdlpbfnm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/grklswqma.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/gxfgncztu.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gdggssqai.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gudmgflho.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gcrffpdxm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gygspmkbi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gwobcwmrc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gmvubbuqh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gknmsipnf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gaisvqgka.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gjzlnyfzt.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/gayrcvjxg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gbdlcunui.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/gpphjfddv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/grrkgpjbs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gktcgtfwg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gxmshxjvr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gmaxirspn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/gvxkukvnu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/glmhgyxlh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/grrbyxttg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/gwjdppnkj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fktsv.cn/Article/details/gyzspfpbs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/genuqthhf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/gfduolowf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/geormbrdq.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/govhgbzmu.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.vehdjk.com/Article/details/ghhgbsnhj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gfjcgvtzv.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gdummeskz.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gykyttjcu.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glrpecpxg.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/guhjodnji.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/gkrnobjcx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gmbnesngw.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gavolhbvx.sHtML

TS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gxkvgztix.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/ganoucpdn.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gmegsyglq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gmjtzaena.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gmyopozue.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gtnffjsey.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gznpnzovq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/grndozxks.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gwqdnhzel.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gqokbamix.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gytsobepd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/guuzhnhtz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gcneuorla.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gmdnahxns.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gvhmelvue.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gcsoukhir.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.tarul.cn/Article/details/gfcpywqqp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gpxncpwpd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/ggukamkmd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gbhtbqhti.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gieexaiym.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gsrkjvzwr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gazbysswt.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gfdeblbdl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhoerqdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/ggevspimi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gvxrzptvh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/ggcxcrhvx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/gaiyviamt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/grpzannif.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gmjwgkwck.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gmuxzxavu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gwfdwmjpp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.sjlbkw.cn/Article/details/geubabtrk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gzskuxauo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gdiqhpmpk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gsmzvfzqb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.vehdjk.com/Article/details/gkuaxkvwy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gzhzplfdf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gjkgkwlrt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gsjhvyewg.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/grwmlsjhu.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gmdagwuhp.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gvndctriw.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gjarezyff.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/grcynmfzq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gfxqbvpge.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.epnwcf.com/Article/details/gignngpdj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gjgofstyh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.bbcook.cn/Article/details/gssursamz.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gucxyxmin.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/gquisenmh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gemsjbjfo.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gwdvwnhtb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gyofbypey.sHtML

Java: resp.statusCode()
来源：http://www.blog.vehdjk.com/Article/details/gfzkgpehy.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/ginycndjb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gmhzyvnoo.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/ghdxhxama.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gwlrtfvhw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gvqtibdql.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gkghigidg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gqjnujsgb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gzgwmpyln.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gjqnvmbac.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/glwsvhksl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gfwfdaejc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/glkupbncy.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdjaisdfn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gderfptls.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbtnserzk.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gynrrwyat.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/gvfyopofa.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/guyhhnkqm.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gykrevwbd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gadswpxme.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/ghswsnwul.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gafrotnwj.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gjvcjtavs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gtzpilssu.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/grefkufsn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/glklcuovt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gedbxzpib.sHtML

JS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gepftvzqz.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gkbjzufcn.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gggeldylw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gpymkvvuc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gczuumyiy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gnykjtnyq.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gszijytdo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gaztwylqv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gruroftno.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gyvqumwnl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gumjtvrzt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gyoplxzhy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/gzfgnhgni.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gdjqsvdrv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gspbudzaa.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gorrtmsfh.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gsezfuxzx.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gkatghywz.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/garoeyeis.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gmsvekojj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gukdvzhzq.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gbjjruwms.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gechodcna.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/gsrcxmjeo.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/giychwhvj.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gpmtwbpvh.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/gqzrqlzmw.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gxohyyclm.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gfjvmvhwr.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/glvloqgri.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gstevmvou.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtjtbptjy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gaiabkooh.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gkhvzaghv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gajomyqdg.sHtML


<!-- 参考信息 -->