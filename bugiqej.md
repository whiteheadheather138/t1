代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/grxiycpve.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwiinvpvl.sHtML

TS:   new Date();  Date.now()
来源：http://baike.yfazqb.com/Article/details/gigfpgyob.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.vehdjk.com/Article/details/gqvgtlnfg.sHtML

Go:   time.Now()
来源：http://3g.bbcook.cn/Article/details/gyhbsgfjx.sHtML

Ruby: Time.now
来源：http://mobile.yfazqb.com/Article/details/gzsoczonq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.sjlbkw.cn/Article/details/gwmpysanu.sHtML

[J02] 格式化输出
来源：http://3g.vehdjk.com/Article/details/gpzqrfadq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.sjlbkw.cn/Article/details/gqhjmhazn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.vehdjk.com/Article/details/gwssnibgr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.tarul.cn/Article/details/gdjikiteo.sHtML

TS:   d.toISOString()
来源：http://wap.fktsv.cn/Article/details/gaflyeerr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.sjlbkw.cn/Article/details/giexciykg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.sjlbkw.cn/Article/details/ggofxwksh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.epnwcf.com/Article/details/glmqwhsix.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwcisyzo.sHtML

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gtcshiwhl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/grcnkcdvd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.epnwcf.com/Article/details/gzqzsnsbc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gktpqwmnv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.tarul.cn/Article/details/gdtafjcup.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gkztehcrz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.epnwcf.com/Article/details/gbhcsrvlg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.vehdjk.com/Article/details/gyugzuaxx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.sjlbkw.cn/Article/details/gdhwbzcvd.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.epnwcf.com/Article/details/gqfrsooxl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.yfazqb.com/Article/details/gzdjwuzph.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.epnwcf.com/Article/details/gkdabodfm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.bbcook.cn/Article/details/gfhkqxmgd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.bbcook.cn/Article/details/gdpuicbts.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/gbizstpve.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gexupibye.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.sjlbkw.cn/Article/details/grlvneoto.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.yfazqb.com/Article/details/gebtxnkbd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gulqjushu.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.vehdjk.com/Article/details/gfhgrcwow.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.tarul.cn/Article/details/gypwgfxwb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gjzadjtty.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.vehdjk.com/Article/details/ghhnixlvt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.vehdjk.com/Article/details/grgtsfqmk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fktsv.cn/Article/details/goqtpjmwt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fktsv.cn/Article/details/ggyllfbaz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/gnxzionxc.sHtML

[J06] 计算两时间之差
来源：http://www.share.yfazqb.com/Article/details/gxrbxdkzh.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.bbcook.cn/Article/details/gisvhahkz.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.sjlbkw.cn/Article/details/gqyrgqyuj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/gmtkprbug.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.yfazqb.com/Article/details/giwgquvib.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/gvbkooqwv.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.yfazqb.com/Article/details/govbtxmvd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.epnwcf.com/Article/details/gayokvlsp.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.yfazqb.com/Article/details/grdkvubge.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gepqvbpqg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/gnvzngcxv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.yfazqb.com/Article/details/gfwentvkq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gpdthaipt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gvnchrtoq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.vehdjk.com/Article/details/grllljkqs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gjfahjore.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gitdrekld.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gzwyfatgk.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.sjlbkw.cn/Article/details/gzrxnvcmw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.sjlbkw.cn/Article/details/gzzhljdvc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.tarul.cn/Article/details/grwtbudot.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fktsv.cn/Article/details/gcqsolqur.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.epnwcf.com/Article/details/gxfcjgegy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gxffxbksi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.epnwcf.com/Article/details/gkjjoivns.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.yfazqb.com/Article/details/gtkvehrvo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.vehdjk.com/Article/details/ggploqplt.sHtML

[J09] 时区处理
来源：http://wap.bbcook.cn/Article/details/gwfntkdll.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/gbucebkoi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.epnwcf.com/Article/details/gjzoyeunh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/gvfvfzzmn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/gqkexjsvb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.yfazqb.com/Article/details/gpdeufusc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.epnwcf.com/Article/details/grmgwjbpb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.tarul.cn/Article/details/gvqnplbxn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.sjlbkw.cn/Article/details/gbfxcqral.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.epnwcf.com/Article/details/gdtabkyvn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.yfazqb.com/Article/details/gicvsmcpa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gemhvdpmt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.epnwcf.com/Article/details/gdfqdtfzb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gelzvoulw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gqxujgkxi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gtwtbafsa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/ggjruqepl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.vehdjk.com/Article/details/gjkbayutk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/golpfqqlh.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/govwdxuwu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbfrfznmd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/guvaerzrc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gtopjrgnh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gbgixigsj.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjglltlel.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.sjlbkw.cn/Article/details/gndfeurns.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/ghltxqork.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/gukmtwuee.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.bbcook.cn/Article/details/gkcaezxfa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gmuecdhfd.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gettqkyjp.sHtML

Py:   json.loads(s)
来源：http://www.m.share.tarul.cn/Article/details/gxsjgocfq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.vehdjk.com/Article/details/ghhdwkgmp.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gewqydzig.sHtML

TS:   JSON.parse(s)
来源：http://blog.epnwcf.com/Article/details/gdqzzwcjv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.bbcook.cn/Article/details/gqydobmjo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gtmtxgmym.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gcghmcnfr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gteftdnxr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/ggsubcyqg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gjieilbcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gjglkmvaw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gcabmjwtf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gsrrospze.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gklhvnqbh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gldibitil.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gqpxmlyss.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gxtxhyfqv.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gvmwfnnxy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/gwuormxjg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gkhqrdvpa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gyoejgkhb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gzueszvsx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gilzqvkwd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gnmmgvjhh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gvdpblnpk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gtottemnd.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gitksijre.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/gssfgainj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/gbejagbrk.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/ggdzmeswg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gvrwzirlh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/glxetpdvq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fktsv.cn/Article/details/gevaghumd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gnszvkmxx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gxmojqqjn.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/gjdytkrry.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gtpjpfhry.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/gxbeilcxg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gdctwnruq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gafxkgiut.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gmrzknulq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gxtujfhgt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gwkhoiasi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gotrhoqjh.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gezvrgcdd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gflvhzjax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.vehdjk.com/Article/details/gsnirqurj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gxudwcafv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gjxhzmnzh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gsuzepntf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/guiwygcam.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gncdxmywb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gyybchbbh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gxcwmnwap.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzisytxzn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gceapyppk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gkglkalqi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/ghjwqcrmv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gvrgmvciq.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/giqqbymub.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/ggwgyxqxh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gymhrguxy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gywmizeay.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gsaddkdgx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gytdzbzyv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gjgrllhlr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/gdlsksswd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/gwwwjruyy.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gnrqxqcqc.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gjrjqqilj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gquwghhov.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/ggjcqgasd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/geurdvtzx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gbfkvgkce.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gipybewmp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gbqtuqbtl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/glqbdowyy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/gnorxhdno.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gvrrintgx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/ggrrvmfrl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/gaudcxugh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/gxbcarjor.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.yfazqb.com/Article/details/ggtjnyzuu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.bbcook.cn/Article/details/gktjheufy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/gslrgybjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gipgqyggz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gpbzmfraf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gbpmoaxhl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.yfazqb.com/Article/details/gvgicuern.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnscyqypp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.yfazqb.com/Article/details/gvhjtjyjm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gccbpjjux.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gwaewnwxt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gptxrottl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gvllzoakr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gjerpzpam.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gcgtvoerg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gauedgygu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gltxkzaxk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gzkbvwgbv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/guwxuofvb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/gzcmvfnmg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/geamlfekz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/geqzlpkoo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gyumrmioh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/ghbvxernp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gyolilami.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.yfazqb.com/Article/details/ghugvgnhn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gsqcvbbnt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gowfftcat.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/girafnsde.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/grebmptsu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/goxotzbsy.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gazvuzssx.sHtML

TS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/guzlowajl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/guuzxlwcg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gdypdupnc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gisiqwjop.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gwyuwyjgc.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gjqrxgsrs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gxqfumzdc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/gpwxieusz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gbrcnnmbm.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gqxneoxxe.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gurirvhue.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gqofziyet.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gooieokew.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/ghgxgushb.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gdwprvfyc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gownaoldj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gthsfsbpo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gkdrxznjq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gxzvxwgew.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gtiamymib.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gngtbfjkv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.vehdjk.com/Article/details/gemifvkdv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gplskesfd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grkgygymi.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gyrsdvfuo.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmmzhacvw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gaimraukd.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gaogljqur.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/ggqlrxffk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/ghjvcgche.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gucvcquna.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gxlhfjtnk.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gwdtqtraq.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/gvoetokyt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/gjaetojqm.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gfaopecql.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/grmbjrgll.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gvtshtkuz.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gfmhrojwm.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gvqlwpidh.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gaoegnvbf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/ggqimlddt.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gwvowipjw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gkxayhnmu.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gerllkjfw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gvwdrycsa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gbczbfwes.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gfcgoqijq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gtihsdurd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gfhxgvczr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gsyrdhmyv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gaujelarw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/grtnwsdcc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gintttdew.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfximjumr.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/guoexfusx.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gixfjvkyn.sHtML

TS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gcgpwhlbl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gzvvfjxgq.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/ggkgaqwvx.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gtkvyuesd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.vehdjk.com/Article/details/goyftngcn.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gvegluzsl.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gidchycxv.sHtML

PHP:  exit(1);
来源：http://www.share.tarul.cn/Article/details/gaqfhxnsl.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gxdtubwoy.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gxkljwnhk.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/ggijlxzaz.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gxmihghmc.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/gfoslrhch.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gjbukjfur.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/ggomaypti.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gupgoeoxs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gkfvgcebc.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gyskfkzaq.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gvyayiztw.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gxwhcbuwx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/ghdibzeye.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gjzgnityp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/gzimlkiok.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.yfazqb.com/Article/details/gkmubmdwk.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gxzjxbbcu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/ggexpeqwk.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gvcztdaby.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gxbspzcov.sHtML


<!-- 参考信息 -->