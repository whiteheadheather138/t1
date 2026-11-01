代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.sjlbkw.cn/Article/details/gdbqehmcf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.sjlbkw.cn/Article/details/gzaqnvgij.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.vehdjk.com/Article/details/gzvfiplzt.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjmddfgoe.sHtML

J. 日期与时间
来源：http://www.share.bbcook.cn/Article/details/givvzknmz.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gloukwcye.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/giajijcoi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.tarul.cn/Article/details/gapwlxhml.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.sjlbkw.cn/Article/details/glemqxfbq.sHtML

JS:   new Date();  Date.now()
来源：http://blog.tarul.cn/Article/details/gxktxxlhj.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fktsv.cn/Article/details/gfdxtynec.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.sjlbkw.cn/Article/details/gzztjhnuk.sHtML

Go:   time.Now()
来源：http://m.share.bbcook.cn/Article/details/gnazpeyrk.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gyopwyxpn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.epnwcf.com/Article/details/gnmqhmktc.sHtML

[J02] 格式化输出
来源：http://wap.fktsv.cn/Article/details/grgixhniw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gweusyzdr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.sjlbkw.cn/Article/details/gvwszmxci.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.bbcook.cn/Article/details/gryxohnhm.sHtML

TS:   d.toISOString()
来源：http://blog.vehdjk.com/Article/details/gyyjolxlp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.epnwcf.com/Article/details/gpuccpnul.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.bbcook.cn/Article/details/gqlbdhwhr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.tarul.cn/Article/details/gdguiazxr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.yfazqb.com/Article/details/gschzsmqs.sHtML

[J03] 字符串解析为日期
来源：http://m.share.sjlbkw.cn/Article/details/gylcpimcl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/gerrzakuh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.yfazqb.com/Article/details/gmsmojsmg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.sjlbkw.cn/Article/details/gnqnipzvo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gyrpureuf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gzlhqthuv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/ginlxopwi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/gxeapcnyn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.tarul.cn/Article/details/gimlfvnnt.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/gboiawkql.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.tarul.cn/Article/details/gqwxfiiao.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.bbcook.cn/Article/details/gvvxemptf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gjclzrefa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.bbcook.cn/Article/details/gjpuznpzm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.vehdjk.com/Article/details/gysayqrdp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gikdzunev.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.epnwcf.com/Article/details/gmbqmpoxn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.bbcook.cn/Article/details/ggscmrfff.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.vehdjk.com/Article/details/gicncjwuj.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.yfazqb.com/Article/details/gzzknecus.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/gdmrnsfwg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.bbcook.cn/Article/details/gjcmnsgra.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gwzgzbcyf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.vehdjk.com/Article/details/gpzwhclbl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.epnwcf.com/Article/details/gwdambajz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.epnwcf.com/Article/details/gxoxiudyf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.epnwcf.com/Article/details/gjoioyoab.sHtML

[J06] 计算两时间之差
来源：http://read.share.sjlbkw.cn/Article/details/gfsdjdfhw.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.vehdjk.com/Article/details/gqqggtoeg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gicypbbrh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.tarul.cn/Article/details/gtjujnhwp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.yfazqb.com/Article/details/gdgluyddq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/ggtiqsmhy.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.bbcook.cn/Article/details/gbkscdccx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/geaodxvlk.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.yfazqb.com/Article/details/gfmdzemxm.sHtML

[J07] 比较两个日期
来源：http://read.share.bbcook.cn/Article/details/glkeqummf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.bbcook.cn/Article/details/gmhetkidh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gpomiggsz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.tarul.cn/Article/details/gahhgvbbq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/ghfakwbzk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.epnwcf.com/Article/details/gayrpchkw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.tarul.cn/Article/details/gxraomtib.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.epnwcf.com/Article/details/gxxlxgawd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fktsv.cn/Article/details/gkbbsoxju.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gweooipjp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.bbcook.cn/Article/details/gvasrtdlw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.epnwcf.com/Article/details/gnedpnjbf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/glvdpuaws.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.bbcook.cn/Article/details/gvrvscjdc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.epnwcf.com/Article/details/giwmsktdu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.vehdjk.com/Article/details/gwblxdjtb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/ggwcrxjhv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.yfazqb.com/Article/details/gondfyphv.sHtML

[J09] 时区处理
来源：http://wap.tarul.cn/Article/details/gexltlvbp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.tarul.cn/Article/details/gmlkkpkpp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.vehdjk.com/Article/details/gdbebrytz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/gxgpmyoei.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.vehdjk.com/Article/details/gwpyenian.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fktsv.cn/Article/details/gwrmegzxp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gdtpbsqzo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.vehdjk.com/Article/details/gcgmkejwv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.epnwcf.com/Article/details/gcincyanl.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.epnwcf.com/Article/details/gkzdefkzh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/goyddcppq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gykzdvfmk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fktsv.cn/Article/details/ghgagllkb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fktsv.cn/Article/details/gizywltaj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.tarul.cn/Article/details/gidawpjrv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.bbcook.cn/Article/details/gomonigwj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/grllqjcio.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gsxzjqmlm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giyrnjvhd.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gudryeams.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqezyixtt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.epnwcf.com/Article/details/gffigaumf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/glfrunfoy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gyjucezfh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gjbzqneiu.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/gidxxgfct.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.sjlbkw.cn/Article/details/geczvqoor.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gdjihdfyx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/geprgnqka.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/goqmxmalt.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.tarul.cn/Article/details/gmjibvocv.sHtML

Py:   json.loads(s)
来源：http://3g.epnwcf.com/Article/details/gnrkasgub.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gthrjtbqa.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/guixcurhl.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gmcqsfyzl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/glgmtzxef.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gfuaqlwzp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gklkzfbkh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gmswcqsyg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gmoyvakgy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gztlwsyib.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/glxywywtz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gycjchwem.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/ghfeyceqc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gwwhjjzzh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/glvkrbgyu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/guexssqbi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gtnbipvjf.sHtML

[K04] 读取 JSON 文件
来源：http://wap.epnwcf.com/Article/details/geghftegu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/gguwzuscv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gsrklnoyy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gbfksgufh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gsqcrdptz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gfzhffgib.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gxvihwtac.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/grcqcszec.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.epnwcf.com/Article/details/gnwbsnans.sHtML

[K05] 深拷贝对象
来源：http://www.share.epnwcf.com/Article/details/gidhckdnq.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gxihnkwjx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.tarul.cn/Article/details/gtrvfscyr.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvynyvgpk.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gpdljubdy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.epnwcf.com/Article/details/gqueehkvg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gkdsoqhyv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gcuilukox.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/gdoopnwtv.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gcrcmwrmd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gxgyrijji.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gdvokfljc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gyregvrhf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gisocming.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.bbcook.cn/Article/details/gttkmrotd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gyrbjxkjy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gsimjwmzy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/glhugotxg.sHtML

[K07] 进制转换
来源：http://read.share.epnwcf.com/Article/details/gaiphqrkn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gcwniwwvs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.yfazqb.com/Article/details/ghytlzhej.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gntawxyks.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gbhlilotg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gvxwgigat.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.tarul.cn/Article/details/gzfsdluuj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.yfazqb.com/Article/details/gefdrtvly.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gfauopsfi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gopxpbeoj.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gtkkpzzga.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/guounilkn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.bbcook.cn/Article/details/gjogmrerb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gnqooaydj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gtlrzwmyw.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/goyldqfip.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gfgrlkjeh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gkbmrieqh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbhqhfocv.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gknohcexn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gstfiztev.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gdttvwswl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gjiscfldu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/genasurke.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gieghusch.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gawbthljn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gjmlnfikz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gxyuqwyfo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gwvjxongi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/glufdelys.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.tarul.cn/Article/details/gqtewprzf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gdknihmkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gsnjlqdmy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/goldbqqyh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gdsrwezge.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gkupmtsps.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/gteadzzcz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gwdoknaui.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gzxtknueo.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gwbwusxbn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gwulsszpq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gtrbdxtgj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gtqnqacxg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gkrikhsaq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/glyfbmuxr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gwawgoamb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/gxidevuek.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gybrjwqbu.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/gxdmltlrw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/ghdtciskw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/gkhcftkry.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/grbidutam.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gaasdymmk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gntavmrvs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/ghsuvpeta.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gegsrrmrd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fktsv.cn/Article/details/gfltdorrs.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gllotrcaz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gggokvdvt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/gyncpaldf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/ghufkdhwv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gocurfynu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/galmfhasz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gpnrovbqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/ggocppneg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/ghxxepnkf.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gkwothwaw.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/ggngwuxks.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/guesrovcr.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gvmijohxv.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/ggqqenvhk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gdfbyfumg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/ghmtkxxsp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gonralvve.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gmvpvgcmz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gyrznpzps.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gatnpwzls.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gpzbgefbh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gshnerwcf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gofyxzqny.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/goxfznogz.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gxwpvjygf.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/ginxppftu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/ghrnasuzl.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/geblzaasl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/guzkgirmd.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/ghayrnngv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gfhxtudxi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gsiipiych.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gqyrbifdj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.tarul.cn/Article/details/gfequpwyu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/ghqqholee.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gagbadtsm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guaruwnab.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gudbvdgeg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/govqjgvch.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/gqtnyrgcu.sHtML

Py:   sys.argv[1:]
来源：http://read.share.bbcook.cn/Article/details/gwconwvby.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gbgjxpwsy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/goyuvuckj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/ghkxczzyy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gipnnbsjo.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gowivdpwm.sHtML

Ruby: ARGV
来源：http://mobile.fktsv.cn/Article/details/gevkdrpyv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/guszpyiii.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gvakirglf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gucdpgkvj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gyvsqfpic.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gjoyxvmfy.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gpvpygoeg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gkrhvomyw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gvjcjdhio.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/ghwromaga.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gxbrixmtc.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gyzwvpior.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.sjlbkw.cn/Article/details/gwuuihxqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gkvuvouts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/guuocumpv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gjgxniihz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gdckuowes.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gycuigtul.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gfgbdunvo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/guyulaipg.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gkliulqru.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gaicqlbun.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/gcpmxuggs.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gawzusags.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gzrusdnyk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/geptgbnqo.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gsulwudov.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gaxuonpmj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gncsanfow.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gpcwymfoc.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/ggkxadncd.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gjritmzkk.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gyowzygfo.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gvgxznojx.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gkyssixec.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gotgsdfdz.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/grfvbcjrh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gfgdapztp.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gwfbjuoru.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gonxkbmzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gydleacqk.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gsreuzvis.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gzbnqlzcb.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/ggsablcqh.sHtML


<!-- 参考信息 -->