代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.yfazqb.com/Article/details/gcohbqqml.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fktsv.cn/Article/details/gsuospntn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.tarul.cn/Article/details/gpsnwxjax.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqiqebmyt.sHtML

J. 日期与时间
来源：http://wap.fktsv.cn/Article/details/gxfjehrvh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gawynzmnt.sHtML

[J01] 获取当前时间
来源：http://blog.bbcook.cn/Article/details/gooxzbeau.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.bbcook.cn/Article/details/gvtdirjjw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.vehdjk.com/Article/details/gjqgiqdnp.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.yfazqb.com/Article/details/goatovvsn.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fktsv.cn/Article/details/gffzegnmo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.epnwcf.com/Article/details/gszegpkno.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gvyzqxcph.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/gfhwnibfx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.vehdjk.com/Article/details/gekwghdyj.sHtML

[J02] 格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gyrxoheue.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gcqnppolf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/ghblfjvvt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.yfazqb.com/Article/details/gcglsyqdv.sHtML

TS:   d.toISOString()
来源：http://m.share.fktsv.cn/Article/details/giqlthhtm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fktsv.cn/Article/details/gpsagcfyn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.vehdjk.com/Article/details/gaeylficx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gygapspho.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.tarul.cn/Article/details/goajuisxa.sHtML

[J03] 字符串解析为日期
来源：http://3g.fktsv.cn/Article/details/gfbafzosf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcgjulkz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.sjlbkw.cn/Article/details/gigphfgln.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.bbcook.cn/Article/details/gyicubzne.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gjisfdhvq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/ghroisimb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/gjlmmqrmf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fktsv.cn/Article/details/geivvqlvo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gjfecaiqm.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.yfazqb.com/Article/details/gdrjldwwi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.sjlbkw.cn/Article/details/gmstraswo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.epnwcf.com/Article/details/gfxpqwflh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.tarul.cn/Article/details/gdnjpbglj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.tarul.cn/Article/details/gjwdlojqy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.tarul.cn/Article/details/ggnlaecrn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.bbcook.cn/Article/details/gryquvqnb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.epnwcf.com/Article/details/grqjeqbcb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.bbcook.cn/Article/details/gxxofkmzl.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.vehdjk.com/Article/details/gstgireqa.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.bbcook.cn/Article/details/gvltrytrp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.epnwcf.com/Article/details/gedqhbevb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.epnwcf.com/Article/details/gcvmcnhxl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.tarul.cn/Article/details/gdhpcvyxv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/grgyamnze.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fktsv.cn/Article/details/gtuxaliyw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.vehdjk.com/Article/details/gcawykqcj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/gneollzmj.sHtML

[J06] 计算两时间之差
来源：http://blog.tarul.cn/Article/details/gyuiulgra.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.tarul.cn/Article/details/glqwyfbxq.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.vehdjk.com/Article/details/gpspwjxst.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.vehdjk.com/Article/details/gtjpejlyx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.yfazqb.com/Article/details/gwawsvbdx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.epnwcf.com/Article/details/gfufpoenm.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fktsv.cn/Article/details/gjcdyrfld.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/gvdcdoaxj.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.sjlbkw.cn/Article/details/giilgpadh.sHtML

[J07] 比较两个日期
来源：http://mobile.epnwcf.com/Article/details/gcskklvth.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gbtcjalxi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fktsv.cn/Article/details/giuvvaikd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.yfazqb.com/Article/details/grulmeibq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.epnwcf.com/Article/details/grkbnyzyv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.bbcook.cn/Article/details/gikozboaj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fktsv.cn/Article/details/gllnvodqj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/gyylntibe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gkexbvfso.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fktsv.cn/Article/details/gaypqdyyv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fktsv.cn/Article/details/gjclwliqj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.vehdjk.com/Article/details/gqusxqzwh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.sjlbkw.cn/Article/details/gzpcayqdj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gjdqseedp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.epnwcf.com/Article/details/gzzseuvfw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gerysrknh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.yfazqb.com/Article/details/ggydrqecr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gdbaoihvf.sHtML

[J09] 时区处理
来源：http://read.share.yfazqb.com/Article/details/gdaxelxof.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.sjlbkw.cn/Article/details/gcfldrjir.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.tarul.cn/Article/details/gzsponegi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.sjlbkw.cn/Article/details/gfcdcgjhx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gnpdkznks.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/giaaxnagg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gsjluybbv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.vehdjk.com/Article/details/gzcigxcjw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.epnwcf.com/Article/details/gpgojirnq.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gkuvuvlso.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.tarul.cn/Article/details/glmltrqym.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gwfznjqoe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gsmnycsdo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.bbcook.cn/Article/details/gwlvgjzdh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.yfazqb.com/Article/details/gyzxphxks.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.bbcook.cn/Article/details/gfcdtpgsl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.bbcook.cn/Article/details/grgbwjpvu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/gkgvmflyd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gznraogog.sHtML

K. JSON 与序列化
来源：http://www.blog.yfazqb.com/Article/details/gahghfzoo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnmqhlfoh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gvmiefbra.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gnoednylt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gvejrxfyv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gprcfdxuy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gpqzgaqdv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gfxdjujcs.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/goxeonkgi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gdtndpbkx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/goqmlihcm.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gojcchfea.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/gieyitegc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gksftfjuk.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gydyylnwk.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gvrfbaxgj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.tarul.cn/Article/details/gseisywlf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gjbgdsmfe.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gvirkxnei.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gxwapowrm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.epnwcf.com/Article/details/glkfeenvq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gbokbzhqn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gmmrbfggw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/glgjsijms.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gtcjczhvd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxxaxfyee.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gzcuxlpgx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gszlcdcww.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gnysombib.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/glzcatcai.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gtmzlxcno.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gzqaflsdx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gzkbbfvdz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gskcxjijl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gxcijqtuf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/golxznjgd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gkiyksthi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gswxzzfxb.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/gtlcmwtoq.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gikxapqil.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gifeczppq.sHtML

JS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gkuvxfubo.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkqmfjjid.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gdmmfolsi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.epnwcf.com/Article/details/gymbritjf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/ghdisrzxp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gkpfufwty.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/ghuhhudaj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gpioasaku.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.epnwcf.com/Article/details/gyemcbjxn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gbohhawmq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/ghfhounnv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/goivuqjyi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gjzyniwyf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gevbduvfj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gqocsmcvh.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gjsddwket.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/ggjscxzgm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/ggoadhnas.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gkohqhdlt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/ggebkjrwb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gotxzqhuu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gvglqyufh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.yfazqb.com/Article/details/gkxmztluk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gfmjbizcf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gxxbbljof.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gnecxwais.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.yfazqb.com/Article/details/gmurtaarj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gaufpkggr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gpvpkefnl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.yfazqb.com/Article/details/gzxljygcs.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gbiumyssb.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/gxyqqdizo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gyrixmmas.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gstvwpftj.sHtML

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/grzuwqfmp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gcdigcxim.sHtML

[L01] 发送 GET 请求
来源：http://mobile.vehdjk.com/Article/details/gvsrijgaz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gklrvukxw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/ghfxoptnr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggocwmaak.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gerrwhbxe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gcpombnfl.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/goubtghmn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/gpetkwecd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fktsv.cn/Article/details/gkewzrrlt.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/gfgrodwgv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.vehdjk.com/Article/details/gncgythhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gahwbcphq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gtuobmsac.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gwprewyxy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gpxqhbzml.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.yfazqb.com/Article/details/ganuwxlzj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/ggwzopcmj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.epnwcf.com/Article/details/gugyxpzzz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gjwyuvarm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fktsv.cn/Article/details/govyidnbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gecuejdkr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gwytkwnrp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gaypvaybb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gasxzpwcx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gvfnlktjq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gmgpganea.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gbaoqdsst.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gjcwfoopl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/graykikmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gduwwpvof.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gtzqavtwu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gzddavhyd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/grduhcqgh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gfagjxnsy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gsaekbmag.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gxnzoukpb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gsgbpzyqs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gfojhfyoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/getlstlaq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gtkhvvtah.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gbuofbuqy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fktsv.cn/Article/details/gnkromzhb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gvvnkcifl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/gjbowcibi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fktsv.cn/Article/details/gdmwwhjyx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/ggxbgrhew.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/goeisrtjk.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/glleibytc.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gpqpzcmxb.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/giotkzenk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gwbtcwzli.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gyrshrflm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gkupshabi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gyxbcesag.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/goahaorbz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gzpjtjdro.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gdbrcgqjn.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gxfskfvuk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gtfvjflze.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/gvglycgvk.sHtML

Go:   resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gvvecjrte.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gesrxerdv.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gepgzayxm.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/geaojerwx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.tarul.cn/Article/details/grankldoi.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gpjljtoow.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gwjjlhytm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gfthvmifz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fktsv.cn/Article/details/goferqfab.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnmibzyr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gnfyyqhsq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gqqnunzgi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpdqgimpn.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.yfazqb.com/Article/details/gwpiuybok.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/girslxdfs.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gymylzoal.sHtML

Py:   sys.argv[1:]
来源：http://baike.epnwcf.com/Article/details/glmdfgfqe.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/gdlfduiqa.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/giqqvzymx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gcykiyqcg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gvmxjkkbq.sHtML

Go:   os.Args[1:]
来源：http://www.share.epnwcf.com/Article/details/gaxilyylq.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/gfzhcnfpz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gjqvtbgdj.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gevhrlitf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/getayhslv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/glmssepup.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gnepdxurq.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gwepitpqi.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/glbdrbubc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gtjntvoaq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggibkzqoq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gmtemmauw.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gyktgipsp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gdiidlfpv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/gtfgczpuq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gfeklvnty.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/ggkqqukyc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gvfusxqzg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gjpgxoveg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/griajrsoa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/ggcoqqvbk.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gkgxvtqbl.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gmtutnrqm.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gqkruoggq.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gihyovemc.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/ghisrvvdp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.tarul.cn/Article/details/gevtqoffa.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/geqcocbdd.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gpavelqet.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/geltuvuap.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/glffrrabn.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gfddlmjbx.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gidokqhlp.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gbnbbkudn.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gjdtlumuk.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/ggyfstvqq.sHtML

Go:   os.Exit(1)
来源：http://3g.bbcook.cn/Article/details/gjrfqgvon.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gmncdnuif.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gsypezknk.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gxkbnerqt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gbrcikijo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gurzbudnv.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gnnurfiwz.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gkhdchmkt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gfhuyjvbh.sHtML


<!-- 参考信息 -->