代发 wailian999

Ruby: s.scan(/error/i)
来源：http://3g.vehdjk.com/Article/details/gyovbtbkp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.tarul.cn/Article/details/gqpvzlvab.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fktsv.cn/Article/details/gwadpnxsc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.tarul.cn/Article/details/gnerczunc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fktsv.cn/Article/details/gexedxgtd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/gqwlqusjf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/gpkexlncc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/geztgzsle.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.tarul.cn/Article/details/gsavvrrmn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.bbcook.cn/Article/details/gbkmrqdfo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.yfazqb.com/Article/details/ghmguhprt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkvnoqtzz.sHtML

J. 日期与时间
来源：http://wap.sjlbkw.cn/Article/details/ghuwnemmo.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gudtnwzcx.sHtML

[J01] 获取当前时间
来源：http://baike.tarul.cn/Article/details/gebctttlu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.tarul.cn/Article/details/gipjothwq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.tarul.cn/Article/details/gewsodoju.sHtML

JS:   new Date();  Date.now()
来源：http://3g.tarul.cn/Article/details/gxzpqpuon.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.yfazqb.com/Article/details/gslspjcgo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.vehdjk.com/Article/details/grydthbfk.sHtML

Go:   time.Now()
来源：http://www.blog.yfazqb.com/Article/details/gibiahmql.sHtML

Ruby: Time.now
来源：http://www.share.yfazqb.com/Article/details/gvcdetbkh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fktsv.cn/Article/details/gkrmktxlc.sHtML

[J02] 格式化输出
来源：http://blog.fktsv.cn/Article/details/gptwlfnzr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fktsv.cn/Article/details/gcyjpfdav.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.bbcook.cn/Article/details/gmtcguhwt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.tarul.cn/Article/details/gsbglynsm.sHtML

TS:   d.toISOString()
来源：http://mobile.epnwcf.com/Article/details/gccbyolle.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.yfazqb.com/Article/details/gpaauyjxs.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.epnwcf.com/Article/details/gfnhqyvue.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.yfazqb.com/Article/details/gransmvst.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.epnwcf.com/Article/details/gdklhapes.sHtML

[J03] 字符串解析为日期
来源：http://3g.epnwcf.com/Article/details/gwjjsnmqr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/geslnwekh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.epnwcf.com/Article/details/grvovwirb.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gqpczuypc.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gemdneier.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/gedidbeam.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.bbcook.cn/Article/details/geyuluaec.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gsqfaxrcs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.sjlbkw.cn/Article/details/gahbvdhfy.sHtML

[J04] 时间戳与日期互转
来源：http://3g.sjlbkw.cn/Article/details/gpprvfvwz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gmkuugtfe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.tarul.cn/Article/details/gjjlsznwj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.bbcook.cn/Article/details/gdmqgrlph.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gznntfbli.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.epnwcf.com/Article/details/glkvvrsoi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fktsv.cn/Article/details/glwygmupx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/ghyjztcmw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.epnwcf.com/Article/details/gylzltigt.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.yfazqb.com/Article/details/gxxkkwhuv.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.yfazqb.com/Article/details/gmmgqfsmz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.epnwcf.com/Article/details/gtnrrvivk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.tarul.cn/Article/details/gnzjjaihj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.sjlbkw.cn/Article/details/gnrmlfaqk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.yfazqb.com/Article/details/gllxnlvzt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.yfazqb.com/Article/details/gizjxyunf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fktsv.cn/Article/details/grhrskels.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.vehdjk.com/Article/details/glulfgjij.sHtML

[J06] 计算两时间之差
来源：http://mobile.bbcook.cn/Article/details/guljqwiiz.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.tarul.cn/Article/details/gnyvmumgu.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fktsv.cn/Article/details/ghsgkwayj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.bbcook.cn/Article/details/gwhfvkjnd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.bbcook.cn/Article/details/gprqnmkyy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.bbcook.cn/Article/details/grhfxaunh.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.bbcook.cn/Article/details/gadsolsnb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.epnwcf.com/Article/details/gfbykfmfr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gtbkcqvaq.sHtML

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gmgqsrmoz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.vehdjk.com/Article/details/ggfxceeqo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.epnwcf.com/Article/details/gjeufjgtu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gnhgpbdqx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.tarul.cn/Article/details/gaacoxwrt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.tarul.cn/Article/details/gcciahqnl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.bbcook.cn/Article/details/gbhcpdztk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.sjlbkw.cn/Article/details/gcwzionhx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gqceasvnw.sHtML

[J08] 提取年月日与星期
来源：http://3g.vehdjk.com/Article/details/gwudpjslo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.yfazqb.com/Article/details/grkrijezs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.bbcook.cn/Article/details/gxlmmigrx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.bbcook.cn/Article/details/gwnogymcz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.vehdjk.com/Article/details/gfajykqri.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.epnwcf.com/Article/details/gbctolqcm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.yfazqb.com/Article/details/gnvdysczs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fktsv.cn/Article/details/gauxvqhbb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.epnwcf.com/Article/details/gtnjbltzf.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gvfhjkpri.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gxjmryddu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fktsv.cn/Article/details/getnpxfox.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.bbcook.cn/Article/details/gjujlqlqa.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.epnwcf.com/Article/details/gejxpqyao.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.tarul.cn/Article/details/gqarnvvvn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fktsv.cn/Article/details/gltftresw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gzlhmywim.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/glycraccu.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gercsgvls.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/gqblfzhld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.sjlbkw.cn/Article/details/gdojaxlrp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gjnmyrzwz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.vehdjk.com/Article/details/gofxicopz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/ghoeohipd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.tarul.cn/Article/details/gknkqiswd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.yfazqb.com/Article/details/gilyoglfx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.epnwcf.com/Article/details/gkztbjack.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbzvuvccp.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gekjhqefp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnodqvycq.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.sjlbkw.cn/Article/details/gdemawkkm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/grwutqtgd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gcympeeab.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.bbcook.cn/Article/details/gwxxdtpdf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gpocbxloi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.yfazqb.com/Article/details/gmekvoycr.sHtML

Go:   json.Marshal(obj)
来源：http://wap.yfazqb.com/Article/details/gsdvgqcnm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gzzpdrtux.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/gzrkpifhc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fktsv.cn/Article/details/goucfphgi.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gxzliytdw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/grufgjjmu.sHtML

JS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gkxcpxrvh.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gdxdohmoi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gsniairco.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gzslzzwwb.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gqsjsuntg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gdxebfqtq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.vehdjk.com/Article/details/giawbqaom.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gkkatygpi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gjmyqztza.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gnataopsw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gkvagevaq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gdqtibbhk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.vehdjk.com/Article/details/gewheoutf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.sjlbkw.cn/Article/details/gppwbtxou.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/gqiqyafok.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/giirzyulo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gmjgptflp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/grdbbgnyi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/goslyryqr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.yfazqb.com/Article/details/ghacelpsq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/ggaaqmtph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gakguuzsy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/glrehmljz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gtekkdsyq.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gcciwrknp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.epnwcf.com/Article/details/giyxygjtc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/grizcoxwu.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gosnyqqhx.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/gazxmbmjq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gsdjlqldd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gqoerffik.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gxcozcjog.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gnimtmver.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fktsv.cn/Article/details/gfurhytiw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/grddpbmbp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/glfmcuiid.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/grinqpvkv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gyzxnkdie.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gkweaulgr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gmnkdounp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gbbornxar.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gozqgakxv.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gpkhjxwtn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gbusttrup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gvwqtytax.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gzacqxtbk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gxxznuivo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gsjgthoze.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gknauxsaj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gcmklpqip.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gimzzuyvl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/gbtqbdrvj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/grzqaqelo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/gvvfrjhrc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gbzuksekr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gefgfdgmf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/gbwkulsjf.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gsxmvwfnz.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/glsxffxdi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gdxbyqdaf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggjghmusj.sHtML

L. 网络请求
来源：http://read.share.bbcook.cn/Article/details/gtbkohpsg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gyfondeif.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gawasossh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gfyfgjzhp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gfrtlxczn.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/goookcydf.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gvnqbauns.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gkopmojhr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gphhjhhlo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.vehdjk.com/Article/details/gkrbnndlb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/georurkox.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gssmwxhpd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gkseningn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gmffsceoh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gqhxrifik.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gughvwngt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gqlrqppot.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gjbvgaima.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gatuxszkh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gkaynuccw.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gmuuyiaqr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gnvlivrjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gfevmzpba.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gtnpmferx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/ghnwjwlir.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.bbcook.cn/Article/details/geibwkcwa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/grmztxgjm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gnbnsbboa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/ghtqhqxku.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gymlvrdtb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/grrokqqep.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gdjesyyfu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gylrlvwrf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/grdqgkite.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gvbcvhpss.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gumijviuj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/gcdmiznig.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gwkigqrfj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gccsajdhw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gvogjqmbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/gettrzhlj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gpacwzrvx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gbcxengbv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/ggpyzfsws.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gubqmasup.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gzrbwwaml.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gzxsaqzcb.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gzwoasdjc.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gadfribic.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.epnwcf.com/Article/details/guwbneccd.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gnysopchz.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/guvzdqfed.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/geekywmch.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gfvarbbxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gcygorfeb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gngxwccmx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gmwmfhflh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gscixqkhs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gsxqpttcd.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/ghfscpkpp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gobirgsgs.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gcjhzjpuu.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gngesqacc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/guckpueeu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gnmpcwoej.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/ghubhoeyp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gsmfifapy.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gpbqctvcb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/ggnjymtek.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gbvbfdfsk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gesmswnga.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gefksvxms.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gyqypkynx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gqgykwgrf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/greilxdho.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gijgnsdss.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdtttbeoe.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gqepmwbpq.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gufpwnkhh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gcstioynu.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gfieyyjtm.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gjoqxowcy.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gnuyzpmfw.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gotyzgjhp.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/glioadjde.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/ggbnjjwqc.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/ghsjtcoom.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gqvscwtsz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gblhcprzg.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/ghklenpzd.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gbzlcsnkp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gvziiumbs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/geywrahxs.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gkfcvadlf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gdbewrvth.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/grczraoio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gyebyovbt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/gytvcvhgk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjjsavwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gsithbnsm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gwmxlmpsf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbkyiubh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gmiqxxxlk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gbjicsswv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gljtcejir.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfugrnnhx.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/ggqdpnics.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gcyvbgxid.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gvpxyzgpg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gbqtawlqf.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/gsxehwzof.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gdyeqzujc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gqhofbonu.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/ghrqqflqm.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gfijryufm.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gsyjluogq.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/ggzbonxvm.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gutrrxmvz.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/goxkrcqed.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/ghtnannjn.sHtML


<!-- 参考信息 -->