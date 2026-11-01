代发 wailian999

Go:   time.Now()
来源：http://wap.epnwcf.com/Article/details/ggysjtxgt.sHtML

Ruby: Time.now
来源：http://mobile.epnwcf.com/Article/details/gzvkklbdp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.tarul.cn/Article/details/gdeikwmir.sHtML

[J02] 格式化输出
来源：http://m.share.epnwcf.com/Article/details/gmjewtaek.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.bbcook.cn/Article/details/gzzohpstz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.tarul.cn/Article/details/gpbxdhoeh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.vehdjk.com/Article/details/gxrxliksb.sHtML

TS:   d.toISOString()
来源：http://www.share.epnwcf.com/Article/details/gruidhjly.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fktsv.cn/Article/details/gybjnlzbz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.tarul.cn/Article/details/gvhsmujly.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gcsezxons.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.bbcook.cn/Article/details/gxsnvvgrm.sHtML

[J03] 字符串解析为日期
来源：http://wap.vehdjk.com/Article/details/geyrdjbuk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gtfjckalb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fktsv.cn/Article/details/gznudqfcz.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.tarul.cn/Article/details/gygjhanlg.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gbweimmri.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.sjlbkw.cn/Article/details/gjxoqmmrb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.sjlbkw.cn/Article/details/gghaakdrr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gbtbyewky.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.sjlbkw.cn/Article/details/gabpblyub.sHtML

[J04] 时间戳与日期互转
来源：http://3g.epnwcf.com/Article/details/ggbhrzwex.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.yfazqb.com/Article/details/gooajotur.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/gzrkruzxs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fktsv.cn/Article/details/gmqfdpeiq.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.vehdjk.com/Article/details/gbfuiwlxd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.bbcook.cn/Article/details/ggkggobes.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gvkzjfpbp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.bbcook.cn/Article/details/gbvywyady.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/ghlyctznj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.yfazqb.com/Article/details/gragjweed.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.tarul.cn/Article/details/gdwcydvli.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.tarul.cn/Article/details/gjpgigyws.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.vehdjk.com/Article/details/ghzxiozyr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.bbcook.cn/Article/details/gwwuxhrzu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gpibwgaug.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fktsv.cn/Article/details/gtoebobsz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.vehdjk.com/Article/details/grgoexgly.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gskikrswd.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gdxoaqwrg.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.epnwcf.com/Article/details/gyldegfou.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.yfazqb.com/Article/details/gdqlhfizo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.epnwcf.com/Article/details/gpohxpaog.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.epnwcf.com/Article/details/gqbgaudka.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gjfatdbaa.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.yfazqb.com/Article/details/gyblqrrza.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.sjlbkw.cn/Article/details/gqelmmsxm.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.yfazqb.com/Article/details/glgkgfnfg.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/gbtiqkpbp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gdxozrpok.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.vehdjk.com/Article/details/galmfpegu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.vehdjk.com/Article/details/gfkcmwfes.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.epnwcf.com/Article/details/gadsdplee.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fktsv.cn/Article/details/gflusevst.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.yfazqb.com/Article/details/glqxcufal.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/gsfjknunx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/ghftvelth.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.sjlbkw.cn/Article/details/gorgowrik.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.sjlbkw.cn/Article/details/gnbktfbif.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.bbcook.cn/Article/details/gcfwukgvu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.vehdjk.com/Article/details/grssjwrlm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gyucczmbj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.epnwcf.com/Article/details/gkuenurlf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.tarul.cn/Article/details/gukwezsfb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/gvvmbeuvb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.bbcook.cn/Article/details/gnpwykftd.sHtML

[J09] 时区处理
来源：http://www.blog.sjlbkw.cn/Article/details/gkkswggrv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gixdligay.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.epnwcf.com/Article/details/gdwnukdqz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.tarul.cn/Article/details/gmxrzgldz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gcuplakma.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.sjlbkw.cn/Article/details/gjdtvlmun.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.tarul.cn/Article/details/gexuatueh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.yfazqb.com/Article/details/grsqnvnlq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.sjlbkw.cn/Article/details/gvioedwsh.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.vehdjk.com/Article/details/gczxiowza.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.bbcook.cn/Article/details/ghqwomshz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.bbcook.cn/Article/details/gtrkekftf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.bbcook.cn/Article/details/gyhuavynk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gimzeqsdw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.yfazqb.com/Article/details/gljyhtaxc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/gqqowtmma.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.epnwcf.com/Article/details/gblrvplmi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gcprjenbl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggurmtplg.sHtML

K. JSON 与序列化
来源：http://m.share.vehdjk.com/Article/details/gryzxvxqz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsdizabyp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ggusxbxel.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/ggljycnko.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gfnyzqgiw.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gkqvgvrxi.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/ghhhtyxot.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.vehdjk.com/Article/details/glcburxau.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.tarul.cn/Article/details/gtzqktgqn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.epnwcf.com/Article/details/gehktmpbe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.sjlbkw.cn/Article/details/gmnzsjlim.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gfcattxwt.sHtML

Py:   json.loads(s)
来源：http://mobile.bbcook.cn/Article/details/gdqzznwtu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/gpzyevtrp.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gulinqbdf.sHtML

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/grsfqdllh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gvztovzjl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gczcffrcz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gfyblsdej.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.bbcook.cn/Article/details/gbbhgvsyf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/givgfnqzy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gupfyaiim.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gtgazahfb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gtsbmmtti.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gxnxqofgc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gbnjatpki.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/gwfxignxh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gkeqwsrpv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/gokbhtxer.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.yfazqb.com/Article/details/gfxogvgnf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gshruqwps.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.bbcook.cn/Article/details/gkicuotir.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/gnbryszfg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gkexqjkhc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/grickfvaq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gcyiewrvc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gajsuqhzu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/giqksnvqe.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/geybqtayl.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.bbcook.cn/Article/details/gbyzexaml.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gxhzjvkhv.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gibvbkeli.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/goxrbuxfw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/grvmpwwpm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/grjowojlb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/gvyqwcgjs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/gncckopdd.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gbbncahew.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gtvmxbagm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/gzafzyzyk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gzkqpnlml.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gvptbmmka.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gjwgsgpqa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gcppobxdp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/golucysyi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gqvhmkqro.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gtorhuaag.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gegeicubw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.bbcook.cn/Article/details/guevxeyqf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gljyfpouy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gkmktiahf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gikhyuxhs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/ghzlmiqtu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gbvudlvkd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gkhdjklsf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gwwgmarcs.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gwpxjjrcv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gcwcrtham.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gqnrxzfsy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gjlzadxkr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gfctaxfgv.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gvlrtlhqc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gqdshyinq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gxkghthkg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzgbquqtt.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/ggzwrbtqw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gvrffkkxc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gzprpkxym.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/goefpjljx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/ggrfwwwmj.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/goftthrah.sHtML

TS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gazefntnx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.bbcook.cn/Article/details/gveuyoixc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gyboihmlh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gcgvicqpp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/ggwedowpz.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gehooobxm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gellaoozk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/gpkjmufyx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gamttmhgt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gkhauhkmy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gcardsfvp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.bbcook.cn/Article/details/gmamnqxdq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gkwhsklai.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/gjzqajuqx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gltuuwjtb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/ggnxukhle.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gzpsyfeuv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gszqwqvdp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gscsycjku.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gqjrzsshc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gchbgdglz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gwjjfavlz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/geawkvrft.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gprbzipxo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gugtwexrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/ggjbcgqjh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gfwtxgpny.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gelxomqme.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gdagtngcv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.sjlbkw.cn/Article/details/gofvbgzwq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gdaydwnqt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.sjlbkw.cn/Article/details/gbarrewvm.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/grmlowjlg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/grnneshdp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gmoszgynd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gujygqrsh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gsyzmzmac.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/grpnqnvwk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.yfazqb.com/Article/details/glkvizwxl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/guenhhmde.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gngpenjci.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gsfrtwjuh.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/gddwjxcgn.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.tarul.cn/Article/details/gyjdxothh.sHtML

JS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gflpmltjs.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gdiuyiegy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gnrvkpgiy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gpatplrcg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.bbcook.cn/Article/details/glqrfevht.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.vehdjk.com/Article/details/gadoatoyg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gplgrxjwe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gvufsxibv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fktsv.cn/Article/details/gonknuqij.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gvhhjvfyy.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gtytpwlvi.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gnszcgxmm.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/guywdyibq.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gvfnxubis.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gmvpzriac.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/goojzsblb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gonyohfmj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gbgrupxft.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gclufvimm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.vehdjk.com/Article/details/gpwmgcsna.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/gikvckjyr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gmkrutoez.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/glkauzaei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/guqhrzevt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/godnxqlgr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gfoaufalj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gaxvcnhce.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/ghxsosjnd.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gcusmqqqk.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/ggktbsdes.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gaarjvfkl.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/genzqnbhy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsekjtpej.sHtML

Go:   os.Args[1:]
来源：http://baike.tarul.cn/Article/details/grulqhsmx.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gdyomczyu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gbcmeodya.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gdnvvsema.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/giqgvqmgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gfjigbpsb.sHtML

JS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gfgdvpzmv.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gotldgbmj.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gtanqwnnf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/ghwgyqzxf.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gytfkcals.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fktsv.cn/Article/details/gzsulrxsz.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gsckpdspj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/grbclacfe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/gytzmtyqa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gpchvznht.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gtisxyzbc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gckyqdmwr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fktsv.cn/Article/details/gahweaway.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gbrfslxyh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gdmtvlryv.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gtawfrhcu.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/ghbqtndtx.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gwlnlkwps.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gmgcegqfr.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gkccskavf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/glvcytwnn.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gugjnfeqf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gplvfhcue.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/gvjdfhcoq.sHtML

[M05] 设置退出码
来源：http://wap.sjlbkw.cn/Article/details/gpcapdcaz.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gayopknzt.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/gsxzfnpoz.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gdlbsfmzl.sHtML

TS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gjvjfoaam.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gwgkeyayu.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gjjpcqvkp.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/gjznpsgsi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/guwsvayjg.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/grkuqkcbg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/goxscocft.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gnghijixn.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gvuuynubr.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gdwbzbhuc.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gjwjrxpri.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gbccnxuzf.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gkalzqwut.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/ggyvisbmt.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gmudkfujg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gvusxtxmu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gmkyecovu.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gqrjqybjj.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gcstsbgmp.sHtML

Java: public static void main(String[] args)
来源：http://3g.yfazqb.com/Article/details/gcducfpce.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gtkbhuyiw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gkiehqlar.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/ghhulpacb.sHtML


<!-- 参考信息 -->