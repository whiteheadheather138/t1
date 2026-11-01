代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.vehdjk.com/Article/details/glnbgvmzv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.epnwcf.com/Article/details/ggshyyyqm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.sjlbkw.cn/Article/details/grsilepef.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gibtbpfwn.sHtML

J. 日期与时间
来源：http://www.blog.vehdjk.com/Article/details/gmdgaaqwc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzwsmtszt.sHtML

[J01] 获取当前时间
来源：http://m.share.tarul.cn/Article/details/gehatxwll.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.vehdjk.com/Article/details/gzhdxebmx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.yfazqb.com/Article/details/grwzoqjcq.sHtML

JS:   new Date();  Date.now()
来源：http://wap.bbcook.cn/Article/details/gikxritmg.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.epnwcf.com/Article/details/getrlapgh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.vehdjk.com/Article/details/gesjsxcyf.sHtML

Go:   time.Now()
来源：http://m.share.yfazqb.com/Article/details/gbfphizlv.sHtML

Ruby: Time.now
来源：http://read.share.tarul.cn/Article/details/gbpmwyhkr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.vehdjk.com/Article/details/gojrudrez.sHtML

[J02] 格式化输出
来源：http://blog.epnwcf.com/Article/details/gvpopvclo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.vehdjk.com/Article/details/gsnfekrka.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.epnwcf.com/Article/details/gjdvekpmr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.sjlbkw.cn/Article/details/gnzurwmkn.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gearjbjri.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/grkoglehl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/ggqszqltd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.bbcook.cn/Article/details/gqffnnluf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.tarul.cn/Article/details/gnjmwxlws.sHtML

[J03] 字符串解析为日期
来源：http://3g.sjlbkw.cn/Article/details/gpolsliuj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.yfazqb.com/Article/details/gbdwgzhyv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.yfazqb.com/Article/details/gucnpplge.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.vehdjk.com/Article/details/goyvrocdz.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gadlgdhza.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gcqxbywzq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/gixupotjc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.epnwcf.com/Article/details/gewlnmvzg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.vehdjk.com/Article/details/ggjcobedl.sHtML

[J04] 时间戳与日期互转
来源：http://3g.yfazqb.com/Article/details/gegrxdqhm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.sjlbkw.cn/Article/details/gnaormsxs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.yfazqb.com/Article/details/guxxwmnon.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fktsv.cn/Article/details/ggmqvuess.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.tarul.cn/Article/details/grrqomnyp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gndiwnknz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.tarul.cn/Article/details/gybzsgxac.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.yfazqb.com/Article/details/gdnybrrxm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.vehdjk.com/Article/details/genltpcre.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.sjlbkw.cn/Article/details/gegpqkfso.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.sjlbkw.cn/Article/details/gailgioxf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.epnwcf.com/Article/details/gbcgeebfl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.tarul.cn/Article/details/gzosrnpwg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gsdzvduco.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fktsv.cn/Article/details/gnkyouquj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.sjlbkw.cn/Article/details/gudvoctxf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fktsv.cn/Article/details/gedyzasyo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.yfazqb.com/Article/details/gglrgnajy.sHtML

[J06] 计算两时间之差
来源：http://www.share.fktsv.cn/Article/details/gomcpbgjf.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/gfyxytzhs.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fktsv.cn/Article/details/guieeqste.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gzguhvabz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/grkaixwrx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.tarul.cn/Article/details/grmjnzxeo.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/giyjxchpp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/groicizai.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.bbcook.cn/Article/details/gpukzeznq.sHtML

[J07] 比较两个日期
来源：http://baike.yfazqb.com/Article/details/gjsqnkwmz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.bbcook.cn/Article/details/gffceobkq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fktsv.cn/Article/details/gnapdgngz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.tarul.cn/Article/details/gjionjtyv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/gtxqkyddp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fktsv.cn/Article/details/grpmxohjo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/ghfpdyiar.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gmkctxjug.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.epnwcf.com/Article/details/gudqefhbp.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/guzpkufwj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.epnwcf.com/Article/details/gxhpmtkrc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/glvccmepl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gzfswfdjo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fktsv.cn/Article/details/gprbbacqm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.epnwcf.com/Article/details/gfrhnypxx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fktsv.cn/Article/details/ghcsmyupt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.bbcook.cn/Article/details/ghipytxft.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gjhrivhub.sHtML

[J09] 时区处理
来源：http://www.blog.vehdjk.com/Article/details/gzdcksiwa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.bbcook.cn/Article/details/gcjjunwow.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.yfazqb.com/Article/details/gslagqwlm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/guqpwawqm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gegpecfsz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gdqmauktc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/guvbdrcnk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.bbcook.cn/Article/details/gbqmrqckg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gmhmjxkqo.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/gpejlhdrl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.vehdjk.com/Article/details/gxwtergmv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gnvxcwrks.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gczaxgvkd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.epnwcf.com/Article/details/ginquwvff.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/glhtjmwwq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.vehdjk.com/Article/details/grlaoxhpj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/gzzvjtmpo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.vehdjk.com/Article/details/gqdoqvvfw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gelwqbzvr.sHtML

K. JSON 与序列化
来源：http://www.share.fktsv.cn/Article/details/gdyburbgj.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnajlfaqs.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.epnwcf.com/Article/details/gyvpmlifo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/gnnmopyse.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gqojqkonj.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.tarul.cn/Article/details/goifntzev.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/ghsdjiech.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.tarul.cn/Article/details/gqyurbeee.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/gbpmbpyrc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gdzswrahl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.epnwcf.com/Article/details/getefzhvj.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/glnphwrpn.sHtML

Py:   json.loads(s)
来源：http://read.share.vehdjk.com/Article/details/gmwkqefhi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gdmwrfdsk.sHtML

JS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gdnpzpejd.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/geyodqfrj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gcoblcsvj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gduzcfkas.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gdimqvomj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.tarul.cn/Article/details/gipxgrqct.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.epnwcf.com/Article/details/gijeqabfd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/goklbjuck.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gjhqtezco.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gpcltmwpn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gkizcoait.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gpwayooji.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gxzzsreiv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gsnusrebg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gjxwcfzsa.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gktldbyyt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/giaxmhgbt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gbpscjhtu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/grqjsrpxm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gurfuporx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gcjeqszlh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gdsbbqrih.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gnnulnleu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.tarul.cn/Article/details/gzjojaehn.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/gdnpcpydy.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/gufogmvdj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/glfnexcml.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnmomrrt.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gqlmazhmn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.tarul.cn/Article/details/gnmzdkevc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/grkorcdqv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gckqkkziq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/gyhrxysap.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fktsv.cn/Article/details/gvtnbbatv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gwervssgi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gypdlqeix.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gyrmgldrx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gkqhjgovr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.vehdjk.com/Article/details/gcfdhoxvu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gmgobxxjj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gslrgyods.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gurforfmh.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gmoeqrwff.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gokdvsllw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gapxznprq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gtlidivff.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gnsqfnogr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gjhvobdld.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/ghmkyzkaq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/gvdmgasqy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gayrmokkk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gqmtwtizh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gnajbfwip.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/ghjevjijs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gzvvrbzsz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gqxzhtdll.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.tarul.cn/Article/details/gbjfaosgx.sHtML

Go:   encoding/gob
来源：http://m.share.bbcook.cn/Article/details/gvejcvmcr.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.yfazqb.com/Article/details/grzwhmwzi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gtmtzhgxu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtsnykzmk.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gggynzdsk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnmmtdtfr.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.bbcook.cn/Article/details/gzbdkawxr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/gbujdnpbx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gjmcfafrq.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/grytusjtx.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gcecvztoq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gtmjkosbr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gprdwvntw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gmqpbfogi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gbjoevvmm.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gapjltslz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gkgabqrwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gfpigolef.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gdeifabku.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gjwbaprjr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/goeoudxci.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gmhznnwds.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gtifzcaqw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/glyspepoh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/ghjiybzcj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.vehdjk.com/Article/details/gjwbraanm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.bbcook.cn/Article/details/ghiguzcrl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gygmiofso.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/galarkmnz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gpsbaxrzm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/ghraqiocz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gjyfxqkfm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gkrngmvlx.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/gjivipfrk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwmlezmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/glbjsvhpp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gzmetgrdu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gpnywcgar.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gflfgdmyt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/grloytkdn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/grqzbxksi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.vehdjk.com/Article/details/gysfksefx.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gmprdicrc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/genyxfvep.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/glwaipbhn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gcbfajpgb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gwtuarktx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gwluweowt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gcnkuslvm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gvmafiujw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gclsphcdr.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gqskhfnef.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/gzagrjtpa.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gukaadzxy.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gplnfsbnl.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/galhludrq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gtcpyiimk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/ghyscisni.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.yfazqb.com/Article/details/grkcfavxl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gzrscvrvr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gvcemhvmx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/gsfagrnpd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gdzrccixl.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gftmflpko.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/gmqbcyfqw.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gxlkpzrdk.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gnsgamlhl.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gsaidlftc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gufynetez.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gpbquvmff.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gcpcjseit.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gynigotrl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gwsemnsuf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gfxfceheo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gyanrxdzl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gacmxgvnu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gpgwtlccc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gluhkgnum.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/giufjrpzx.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gdxkyneaq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqhgrlyki.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gxawowsqh.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gfdlusyus.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/gqoqcdrdz.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gbpqbeita.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/grouhgxxw.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gkohaijrp.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gfiipkcfe.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/ghhtkbwyk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gcgpcrbyi.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/ghuleuuax.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/ggweaerpq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gouxllwjy.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gucwbtfeq.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/glbdfnaqs.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gchliidnm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/ghymqgfjy.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gbblvfnda.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gcmhvzzkq.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gfrrbbskq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gubbcvxue.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gcolkdubk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gxozcyzfh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gzoipvaep.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gptyyzjgz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gsbpoauec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/glienbxxx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gccldjcby.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gkzlmagni.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/gpxojifnw.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gqftibiyv.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gmuzgadzx.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/ghgyswwct.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/giompcrmh.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/gwlelbqnn.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gglefwwtr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gebborxzn.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gnxqpweoh.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/ggjlvdppl.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gixhnhill.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gxbbqqpmz.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gvgdndjvq.sHtML

Java: System.exit(1)
来源：http://blog.tarul.cn/Article/details/gtgetytcl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gkfbitokb.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gopgojfva.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gunukppnc.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/ghwondvhs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fktsv.cn/Article/details/gcnizsdjj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gxqrkrrvd.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gavuruybm.sHtML

TS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gbjepunhv.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gbabhurvo.sHtML


<!-- 参考信息 -->