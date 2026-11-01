代发 wailian999

J. 日期与时间
来源：http://www.blog.sjlbkw.cn/Article/details/gkazbtwzg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gubzlkiyo.sHtML

[J01] 获取当前时间
来源：http://blog.fktsv.cn/Article/details/gvicywobg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fktsv.cn/Article/details/gnrwwkgxv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.bbcook.cn/Article/details/gvjhsglxe.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gsxfxzlte.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/gbvflkjqf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.epnwcf.com/Article/details/gnidaqruj.sHtML

Go:   time.Now()
来源：http://www.share.fktsv.cn/Article/details/gsbiwpmaz.sHtML

Ruby: Time.now
来源：http://blog.epnwcf.com/Article/details/ghogpywen.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.epnwcf.com/Article/details/gphvfpboi.sHtML

[J02] 格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gavoybueu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.epnwcf.com/Article/details/gykelmbyd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.bbcook.cn/Article/details/gureztixg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.sjlbkw.cn/Article/details/gxcvhhmsv.sHtML

TS:   d.toISOString()
来源：http://www.m.share.yfazqb.com/Article/details/gvkyzveid.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.vehdjk.com/Article/details/gdiwfvebw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.bbcook.cn/Article/details/gwiuwsdve.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.vehdjk.com/Article/details/gludkwtit.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.vehdjk.com/Article/details/gnhnsnxqv.sHtML

[J03] 字符串解析为日期
来源：http://www.share.epnwcf.com/Article/details/gholtgvcs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.tarul.cn/Article/details/gidizoaqg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gzaivtgyi.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gvfuwryjo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gulvgzbfx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gktsqtdsa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gdjpguiyv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fktsv.cn/Article/details/gztlszcmq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gismtxpqi.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.vehdjk.com/Article/details/gnhepaxed.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.bbcook.cn/Article/details/gwfnrvgea.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.tarul.cn/Article/details/gmtpzhkfl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.yfazqb.com/Article/details/gzopszhme.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.tarul.cn/Article/details/geqilsigb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gsukibllf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/gfkaowhuf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.tarul.cn/Article/details/ggtceelpc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.tarul.cn/Article/details/gjinhrjjn.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gesbmpdif.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.vehdjk.com/Article/details/gmtqudqlz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fktsv.cn/Article/details/gzznczwsx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.epnwcf.com/Article/details/gfsarcxix.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.bbcook.cn/Article/details/gerjfmram.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.vehdjk.com/Article/details/ghrqlplpt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.tarul.cn/Article/details/gqphqxhzi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.epnwcf.com/Article/details/gyjtlrsse.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.tarul.cn/Article/details/guzcypnly.sHtML

[J06] 计算两时间之差
来源：http://baike.epnwcf.com/Article/details/gdksxvbfu.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.tarul.cn/Article/details/gfxyomezu.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fktsv.cn/Article/details/guylnuijf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.yfazqb.com/Article/details/gyvvaphki.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.vehdjk.com/Article/details/gtnimarhv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.epnwcf.com/Article/details/gbgnqbhhg.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gqgpvtjoe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.tarul.cn/Article/details/gzsoorupc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.vehdjk.com/Article/details/gjkynyamg.sHtML

[J07] 比较两个日期
来源：http://wap.yfazqb.com/Article/details/gclejlhgn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gthmbugli.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.vehdjk.com/Article/details/gcwucunqn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.sjlbkw.cn/Article/details/ggoupelwv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gqvfghjpm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.tarul.cn/Article/details/gewapwkdp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.vehdjk.com/Article/details/gxdjtirwx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gbwijavec.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/gfszdquxu.sHtML

[J08] 提取年月日与星期
来源：http://m.share.yfazqb.com/Article/details/gxzzsojdw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.tarul.cn/Article/details/glorrthyq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.vehdjk.com/Article/details/gmvsejywd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.tarul.cn/Article/details/gwhlaiaxb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.vehdjk.com/Article/details/gvwzzvwus.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.tarul.cn/Article/details/gwqazxkiu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.epnwcf.com/Article/details/gknqiuzhh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.bbcook.cn/Article/details/gzpcdpnqu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.yfazqb.com/Article/details/gvioujlxj.sHtML

[J09] 时区处理
来源：http://wap.yfazqb.com/Article/details/glzpznhis.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gxpxuoeum.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/glijmocmr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.yfazqb.com/Article/details/gufwdkckn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.vehdjk.com/Article/details/groqisjcs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.epnwcf.com/Article/details/gbjofhtew.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gtvmdnrpn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.vehdjk.com/Article/details/ghkjlojrg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.sjlbkw.cn/Article/details/gmfzfkkyf.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/gbjpjkoyj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjintclai.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.tarul.cn/Article/details/gvxoacigo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/gnhfexntb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.yfazqb.com/Article/details/gskdfckrz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.epnwcf.com/Article/details/gqnmvagdk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gpppvupuy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/gxcassgsv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.yfazqb.com/Article/details/gvwajezzy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gluxenhmy.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gkyrubaba.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcbqkiiyp.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/gousbhgju.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gihxkegrd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gyuaqvywd.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gqpmfjyhm.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gsfuwutqi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gqwcoakfz.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.bbcook.cn/Article/details/gyndixbfv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.bbcook.cn/Article/details/ggmiqhqut.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/gasmicnba.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/gktqmofjd.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gaexdwnac.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/gatzpmkdc.sHtML

JS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gerikopsa.sHtML

TS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/geztgrzfi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gtbpyseqc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gzrimkcrn.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gxgeqyzmu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fktsv.cn/Article/details/gmkmbylmf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.epnwcf.com/Article/details/gbqfltovd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/greozbtwq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/gxwxludej.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/gtcgcbpki.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gnibgoszd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fktsv.cn/Article/details/goiktgzhl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/gjuquaduh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gczumaicf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gpuywtdkz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/gdxtuuzdn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gzwsnuide.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.yfazqb.com/Article/details/grbwgrkbf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gnemcsaoh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gklicofqk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.epnwcf.com/Article/details/gvozhftki.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.tarul.cn/Article/details/gpjpotzhp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/gqkmdqisi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gkjcccmal.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gwwwhnytw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/grrmngvoj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/gubexutzx.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gqmboxbhz.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/grhmmhhcj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gmuyjmxsx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/galvhszwi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/ghcznaudh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.epnwcf.com/Article/details/gwrjwfcro.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fktsv.cn/Article/details/gihvwqfka.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gmwndxusv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gdueybbld.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gkxqrgrqi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/genlunzqd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/guyxpznau.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gvpbemdlw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/goqfeocku.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gwnrimexd.sHtML

[K07] 进制转换
来源：http://www.blog.epnwcf.com/Article/details/gmxzjulom.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gdqtlhdct.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gkilokcdh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gdbkxzvod.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gqloplndi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gkruawute.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gfzcpmkun.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.vehdjk.com/Article/details/grzfhllju.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gkfcsyzdo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gatggucwq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/ggjxwokpg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gysicoeir.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gdzkepfnc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gtagscijr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/ggnaqxgta.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/gxhlzfxce.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/gjgamcoya.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/ghwwyhrgy.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpuhhekkn.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gcsdbxqpf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmpbgoogy.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gfpfvzlxp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gnoyojppy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.yfazqb.com/Article/details/gnrwxxsqh.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gzogvhyml.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gxupmabag.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gwtguxulc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gklvxjcfz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gwzmgflas.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/gjdgjbqlq.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gtgfuvwij.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gyjfzgpxx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/gsfhkwglu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gqnhupxkt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gvadhhlfx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/goimskblr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gsbkwzlqy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/glgfjzlbu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.yfazqb.com/Article/details/gbwpbjfbt.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/guaozqtpn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gvixxwphw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gtxxmseuf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/ghjxiygkb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/glhqkcrpb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/gqmlbcoan.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/geabqntpl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gyxwwqggt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gpebecuch.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gkphjpogl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/ghqigtrcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/geswhnsea.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gpjmynrsz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gaykqcymp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gvghxohwj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.vehdjk.com/Article/details/gcwgscsbp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.bbcook.cn/Article/details/gbemnmafa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gtxxtfqki.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/gdcxennom.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/ghigaoido.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/gwulzgnys.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gdktzsaer.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gowltexek.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gdedmqtgf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/gfsrvvogl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/gycpplohu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gdtghimrx.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gakhztkgh.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/gifxcsnka.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gxeuyonmp.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gboylnmuy.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gqusrbbku.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gbbswkfgo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/ggknrbrxk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.tarul.cn/Article/details/gbisnxtzj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gxhjhkqwe.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.sjlbkw.cn/Article/details/gnpnueylt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gdxtgwbzn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gskqmxbkn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gloyvsktb.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gnxxqnkud.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/ghkexidbi.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gwfkslshk.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gifqlodsv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gjucmughi.sHtML

[L08] 并发请求多个地址
来源：http://read.share.bbcook.cn/Article/details/gouyuxmqf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/geornyjxx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gcgivkuhq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gvoiicgqc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gwqhntgrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/ggjpjxzye.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fktsv.cn/Article/details/gqezyfkrw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gkmwjrcdv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.tarul.cn/Article/details/gwebknbty.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gftjvhbcz.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gkeatbmox.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqcmdsaue.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/ghbtdoqut.sHtML

Py:   sys.argv[1:]
来源：http://m.share.tarul.cn/Article/details/gxikzgszo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gimabbxoo.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gjwopbqec.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gvvlqfhlj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gvvljdhje.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/gqnuvftmh.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/goateckle.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gblopppir.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gkxipjctm.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gcsqsiruo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gnebgkolc.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gppeiqsmk.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gcjzydbig.sHtML

Java: System.getenv("HOME")
来源：http://mobile.tarul.cn/Article/details/gotkkjxtq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gyxjubicp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/gblgjvjey.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/ghzxbplrv.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/gwjgqxgys.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gbfxmtumv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gmbbbslbz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/glidajdrz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gfncevhpg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fktsv.cn/Article/details/gqejqeucj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gwncmomrp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/gckpwrnfh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gsrjewxpi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gwkuqemtr.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/glftgvfnu.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gbltkoojv.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gqvvgvcvg.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/govnobaud.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/govwqdsiz.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/ghcyaggut.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gyqoiocib.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/ggesmxdlu.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gxcnjobiy.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gztoltttm.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gtckneook.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gkxwzbiog.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/guqhwplkr.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gwivysxcd.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gaxfucqqh.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gglxwazdv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/grdmfhysb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gusjgfzrw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/goqtjnioj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/guovqotma.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/giqjdtmii.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/guksssddr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/guivwcjub.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gccwjgncw.sHtML

Ruby: warn "err"
来源：http://wap.fktsv.cn/Article/details/glviurpwu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gmqkaezgo.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gsqsdoohi.sHtML


<!-- 参考信息 -->