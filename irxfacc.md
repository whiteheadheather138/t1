代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.vehdjk.com/Article/details/gsiwsjzjf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.epnwcf.com/Article/details/gcyueftyf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.vehdjk.com/Article/details/gdginmtqi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.yfazqb.com/Article/details/ggmgcgwwb.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fktsv.cn/Article/details/gdmqlhoaj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.tarul.cn/Article/details/gmzxljiwp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.sjlbkw.cn/Article/details/gffinezsp.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqfbfuykj.sHtML

J. 日期与时间
来源：http://3g.yfazqb.com/Article/details/giobxbppz.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmuomcboq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gujpslyhi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.bbcook.cn/Article/details/gqwxexyhh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.tarul.cn/Article/details/gfychmaoe.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gprlbkuag.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.bbcook.cn/Article/details/gpbrvheis.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.sjlbkw.cn/Article/details/gztudwgdw.sHtML

Go:   time.Now()
来源：http://blog.epnwcf.com/Article/details/gnxbwwxch.sHtML

Ruby: Time.now
来源：http://www.blog.sjlbkw.cn/Article/details/gnmvrgjlp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.vehdjk.com/Article/details/gptnithyx.sHtML

[J02] 格式化输出
来源：http://read.share.sjlbkw.cn/Article/details/gtcribiwm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.epnwcf.com/Article/details/gqwvawuhk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gmpwwjims.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.bbcook.cn/Article/details/guzpxrutm.sHtML

TS:   d.toISOString()
来源：http://m.share.fktsv.cn/Article/details/gigokbytr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.yfazqb.com/Article/details/gouixkciy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/ggndipsbz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.yfazqb.com/Article/details/gjokcrufy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.bbcook.cn/Article/details/gsumbluuf.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.tarul.cn/Article/details/gnxhofgkr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/gidksiegs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/gtnvbvhfw.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gngfsgoqi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gexyrgfmb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.bbcook.cn/Article/details/gienxymqe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.vehdjk.com/Article/details/ggzbbvmiy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gqbpghryz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gwbjvbghf.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fktsv.cn/Article/details/gihnujguk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.tarul.cn/Article/details/gxzfcjxvs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.yfazqb.com/Article/details/gechbybth.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gvavvfnzt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.yfazqb.com/Article/details/glzxjtpvb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.sjlbkw.cn/Article/details/gxhzqufem.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.vehdjk.com/Article/details/ghdrykoti.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.sjlbkw.cn/Article/details/gksiguhvh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.tarul.cn/Article/details/gqathfnsx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.tarul.cn/Article/details/gvtjyaetp.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.yfazqb.com/Article/details/gwziutidz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gzdthowyd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.yfazqb.com/Article/details/gfmsufjhr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/guimjtucn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fktsv.cn/Article/details/grqzdfxpk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fktsv.cn/Article/details/glidsikyp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/gyqdnqqez.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.epnwcf.com/Article/details/gwqywarbh.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gklonfxae.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fktsv.cn/Article/details/gpzepbpql.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.tarul.cn/Article/details/gkpzqyfwm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fktsv.cn/Article/details/gvmxtwgnj.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.vehdjk.com/Article/details/grbpiusmy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gopgxlmrz.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.yfazqb.com/Article/details/gwtdsjnto.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fktsv.cn/Article/details/gbklzlvdw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fktsv.cn/Article/details/gctfquppw.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/grsfgnzyo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gjovvaezz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.tarul.cn/Article/details/gpiwcbniw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gofosisgr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.yfazqb.com/Article/details/gvakgtzsb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.tarul.cn/Article/details/ghztwrjuq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.epnwcf.com/Article/details/gaaidgnhp.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.yfazqb.com/Article/details/gvztsxman.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fktsv.cn/Article/details/gkckujgvw.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gtcnlhqyq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.tarul.cn/Article/details/gowjelbiy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gfdzokyal.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/gxisfpzlf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gbjsqvlqq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.epnwcf.com/Article/details/gjkvprcxu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.bbcook.cn/Article/details/gnybcfpwy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.sjlbkw.cn/Article/details/gtokrwuis.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fktsv.cn/Article/details/gpihcpkjb.sHtML

[J09] 时区处理
来源：http://baike.epnwcf.com/Article/details/gmqyywbzw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.tarul.cn/Article/details/gmivmpdqo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gshugbkao.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gemoliwvp.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.tarul.cn/Article/details/gjddvdffn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/geoixtfqu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.sjlbkw.cn/Article/details/gypamgwrv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.bbcook.cn/Article/details/guwwufmin.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.vehdjk.com/Article/details/gaikinysv.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.yfazqb.com/Article/details/gpxmyhtlo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/glgrmqnvn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/gakyrqbqx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/gciwjuodk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.vehdjk.com/Article/details/gqjkzpxvz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjvwuhbjc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.epnwcf.com/Article/details/grnuzxsrw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gbzzcevqr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fktsv.cn/Article/details/gjbekdguy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggdddcpeg.sHtML

K. JSON 与序列化
来源：http://www.share.epnwcf.com/Article/details/gacmybalt.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtgqqarmb.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/gompfcxsq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/grconlety.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/ghdboohuz.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gyzywbgsc.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gsnrdtwbg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gbmccifsq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.epnwcf.com/Article/details/gvlwfhvhh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/gjawyddjy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gdjxjksmy.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gtqhcqtcr.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gnmisnnkh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gttnanvxb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/grrwedbwg.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gpqfgfadn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gphbjmpgq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gheivhjjh.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gsccccvtx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.tarul.cn/Article/details/gqwzhivct.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gwuhevzwr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gwxoqtvys.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.bbcook.cn/Article/details/gkabfvlik.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/ghcnwysuk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/grlwrtxns.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gelpdsihg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.vehdjk.com/Article/details/gayslrbmz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gkeutqlgb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gqfdhtzyg.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gtpleshwe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.sjlbkw.cn/Article/details/gqcuzhzcm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fktsv.cn/Article/details/ggtyabfil.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gisjarbyq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gpvynsbem.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/ggiigbdtl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/ghxaialcq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gsaoefsnv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gnxmkyprz.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/getndqpbp.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gyeqcdscb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.bbcook.cn/Article/details/gvwwfmpfg.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/glnbiniga.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/glmggtsdg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gmwhhahim.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.tarul.cn/Article/details/gsqxipxoh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gtiaonvtf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gnrinhyvl.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gryatzikz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/ghayyxknx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gzcpyeubo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gkadxkbaf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gphdftejc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gbdlvyfbc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gllbsmwlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gagzgwywl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/grxrrnlee.sHtML

[K07] 进制转换
来源：http://www.blog.sjlbkw.cn/Article/details/gvnmxadre.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gwrpnusix.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/gyfbetlgu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gzjtjzzhj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/geovjivhe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gnhazenmv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gltdzdedq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gwjhmtowy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gnzhwosfj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gvisytwmb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gqoeitpnd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gphfbrnfj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gpyxsddzn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gkpdhnirp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.yfazqb.com/Article/details/gyhmwobdy.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/gfdlgmizb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gyiebllkl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gfnnwkobp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvuolgvqt.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gaknzowoa.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfzsfcxsy.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.bbcook.cn/Article/details/getdlaimh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gqwzltnel.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gshvcvxjv.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/ghzamhspz.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gcdzmdajg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gvwnrmxny.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/gpdejhwwz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gubhaohjo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gbdfulgkj.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gqqvlefto.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/ggwvzyrpb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gckosswry.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gykfeaibc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gmphlvlmo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/griyvikig.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gjvmfjuqo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gasejxvxr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.sjlbkw.cn/Article/details/gjpyuztmx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gsbidbjig.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.yfazqb.com/Article/details/gaypbwgqm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gkikamoav.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gszscxiog.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gqtetwwik.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/grilrltks.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gnvmdahev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gigbuewmr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gjbxoctfn.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gzezbmvjc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/gennwxgea.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gfxoowwuq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/grccqjyzx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gefhzyxxt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gihjrhwkr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/gxkrhmwjz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gjnqfhsaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gwlehyxyq.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gtsksqkfq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gkxgkfiiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gbwhjbntp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gypjtzvmh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gjnwblgwe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gqdbpogly.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/geeduawpu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gowtidihn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gsigqavmn.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gjeykxbqt.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gquujrlqe.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/ggkpbdaxi.sHtML

JS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gjxzmvskc.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gxrycwllk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gmzwepagl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/guamckgxg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/gobnfutrx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gktdelmtj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gwafisene.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/gphlwejnu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/gohccjuxz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gyueoucxc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gyovzzoic.sHtML

Java: resp.statusCode()
来源：http://baike.vehdjk.com/Article/details/gadbmgkla.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gncvxqutp.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/goqdxjqmd.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gfasaboxw.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.bbcook.cn/Article/details/gkqzqgziq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fktsv.cn/Article/details/gphegdhan.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gzcjoyzek.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gbliwacvp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gidyrsjbp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gblrdnjhe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/gwsadjjop.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gwsobwpdz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.epnwcf.com/Article/details/guzgvtszn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnkpyafnl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/gykbzpodm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvcitwfpm.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/gtabxwmac.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/gdbleimdf.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gysuzkarj.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gmvbbfbwa.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gfrrvxzdw.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gdolmtpau.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gazzfzbrs.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/gggbstkco.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gzzyqhtte.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gjtvceinn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gbozshntp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gicrfhkay.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gantgxotx.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/ghpcappzg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/ggfplmaji.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/ginlzfmlo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gyfoufgyq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gpjebwbas.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/grpgbrfaj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/ggitehahd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.vehdjk.com/Article/details/gxsanoiki.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gydkbcmwr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gdevgidrz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/gfymoobrs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gzqorqsaj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/giekoltoa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gtxulrcda.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gkggovyjq.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gzcwethwu.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gbkttrvla.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gpiyzhnxx.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gouihpvnv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gcpeppchq.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/gnhonwxbq.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gctbqzjwc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gbofzsgyi.sHtML

[M05] 设置退出码
来源：http://read.share.tarul.cn/Article/details/grnpwpihs.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gyxyevqcj.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/ggmypsxad.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/ghpsfrvyd.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/grzbapsqq.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpfjkwqpc.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gslmpcnzw.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gffzbkwzz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gclwjrwuc.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/govrljadv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gywlqhkdl.sHtML


<!-- 参考信息 -->