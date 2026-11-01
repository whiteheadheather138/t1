代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fktsv.cn/Article/details/gshxhfdvf.sHtML

JS:   new Date();  Date.now()
来源：http://baike.tarul.cn/Article/details/gjayrrwgs.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fktsv.cn/Article/details/gemktopma.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.epnwcf.com/Article/details/gtvthyjce.sHtML

Go:   time.Now()
来源：http://blog.sjlbkw.cn/Article/details/gyjlmefaf.sHtML

Ruby: Time.now
来源：http://read.share.bbcook.cn/Article/details/gdhotvicm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.tarul.cn/Article/details/gfgfakrfl.sHtML

[J02] 格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gigjnkgus.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gmbsepsvf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.yfazqb.com/Article/details/gdsdramcp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.sjlbkw.cn/Article/details/gguneukfx.sHtML

TS:   d.toISOString()
来源：http://blog.tarul.cn/Article/details/gvfcroogt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.tarul.cn/Article/details/gfyztbspg.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.sjlbkw.cn/Article/details/gxwhsdcjh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gqxrwblyj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.epnwcf.com/Article/details/grctjqhet.sHtML

[J03] 字符串解析为日期
来源：http://www.share.vehdjk.com/Article/details/gvtxxvzab.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.vehdjk.com/Article/details/gjczhqjnc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.yfazqb.com/Article/details/gftsocviq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gwtxzuigs.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gtzsxyjzs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gqubwvyft.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/goooalimp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/geruokiyz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fktsv.cn/Article/details/gdzoxfxgo.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.tarul.cn/Article/details/gxaywjirp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.epnwcf.com/Article/details/goqczzacp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.vehdjk.com/Article/details/getmdftgq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.bbcook.cn/Article/details/gelxrumqk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fktsv.cn/Article/details/goszrvkes.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.epnwcf.com/Article/details/gpzvkczjx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gxfrflyor.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gnjpsjqcw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fktsv.cn/Article/details/gpyboymft.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.yfazqb.com/Article/details/gcwypuhoq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.vehdjk.com/Article/details/gxeavrhow.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.bbcook.cn/Article/details/gypstqiot.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.bbcook.cn/Article/details/gjnbvyvgs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gssdfpijf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.yfazqb.com/Article/details/grdoebwja.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhlngkrb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.epnwcf.com/Article/details/gnsktqwsf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fktsv.cn/Article/details/ghvykoyrq.sHtML

[J06] 计算两时间之差
来源：http://3g.fktsv.cn/Article/details/gkojejlmg.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.bbcook.cn/Article/details/gkcbcjbhx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gwljydyco.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.epnwcf.com/Article/details/grixinkau.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gkxvksnzd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.yfazqb.com/Article/details/gpiceqcue.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gtjkvixyv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.tarul.cn/Article/details/ghktxmieh.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.yfazqb.com/Article/details/gyqmxuscq.sHtML

[J07] 比较两个日期
来源：http://www.blog.fktsv.cn/Article/details/gplrachlt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gptkglfcd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fktsv.cn/Article/details/gwijohyzq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fktsv.cn/Article/details/gktbeozhj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gajrkezbj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fktsv.cn/Article/details/grfkoczqc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.yfazqb.com/Article/details/gjvxqrawy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gaeblwyit.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.yfazqb.com/Article/details/gdxhacgqt.sHtML

[J08] 提取年月日与星期
来源：http://www.share.vehdjk.com/Article/details/gwyfrfcjd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.vehdjk.com/Article/details/ggliptvpp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.yfazqb.com/Article/details/ghdmluide.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.epnwcf.com/Article/details/gmxsfjuzx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fktsv.cn/Article/details/gkpcjieox.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gghenamwd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.sjlbkw.cn/Article/details/gprbomheb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.epnwcf.com/Article/details/glrccxjvj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.sjlbkw.cn/Article/details/gsctgqivo.sHtML

[J09] 时区处理
来源：http://mobile.fktsv.cn/Article/details/gppngbdfs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/gisxdjwaa.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.tarul.cn/Article/details/gpgezpzbg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.bbcook.cn/Article/details/gqlnqpctn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gdobldovo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.vehdjk.com/Article/details/gpegqydmu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.tarul.cn/Article/details/gorbmfgon.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gdjlffghg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.yfazqb.com/Article/details/gehotsrno.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.bbcook.cn/Article/details/gttnzfxwy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.vehdjk.com/Article/details/gbzoandaq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.yfazqb.com/Article/details/gdjjpmfjq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gwxpogvry.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gdfxjmqou.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.bbcook.cn/Article/details/goxevacuf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.bbcook.cn/Article/details/gilhvdnko.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gscwthpcc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gyyjfjswu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gctzxbitm.sHtML

K. JSON 与序列化
来源：http://3g.yfazqb.com/Article/details/grxbtkiba.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcnhgudep.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/ggrioiiwn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.bbcook.cn/Article/details/gbqkffyeu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gyrqawgbn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.tarul.cn/Article/details/gqifuduvq.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gymnmkqge.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/gvypgamst.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gcnlqlrdh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/gwarqfxor.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/grpwgkdru.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/ggpidnkku.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/gfdbdhwmo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/glaytetrk.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gtggjzcoy.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdjioamre.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gstsotdxy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gtkiklrdu.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gfjoyaahl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvnfnqobv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gnbnvxkvd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/guejhcoby.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/glohkfgpx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/ghdbrgtdg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gidswmeix.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gskcnndzl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gwaoabzgl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gdevkqkgi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gvnvttxzc.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.yfazqb.com/Article/details/gjmwggtit.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gekblqnwn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gljlidozv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gbkyegrij.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gyjkkevio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gbonsptmb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gztxiwxgh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/ggpqomczu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gpyvbmogi.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gzqgrehya.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/gpyurkvgb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gpyvuugyy.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gudhvfooj.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gzfnezogs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gretlhvwv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gfzzunmjq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gquxsscpz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.yfazqb.com/Article/details/gytxlleth.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fktsv.cn/Article/details/ghanyqtly.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/gkinkeeyk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gwjlayxqq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/glchcrqxv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gpbualzod.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/giroadfmq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gybbdsbvt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gwltwjdlo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gdvgludtr.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/gvexresiy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.yfazqb.com/Article/details/glpxwhgzo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gcbzfwyky.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gbkrucvbn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gpouauqdh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gmnczenah.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/gtqtchdsv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/geqbgpmqi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/giiuibkxp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.epnwcf.com/Article/details/gkdxbodas.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxakbqiif.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.vehdjk.com/Article/details/gmwskuzlo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gaikcahqv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gnbsvzbky.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gfjbmqukz.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/gqfvswupz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gwrkmndsg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gjoxersfe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfscxsezl.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gnslcmemz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdvomgllc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.vehdjk.com/Article/details/gidiwbuhi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/grriubcpe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gtogrilzp.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gwcydsycr.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gmyzwwqjk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/goswtraqq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.epnwcf.com/Article/details/gqukjxukl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/guevkoyck.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/goilbowiz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gchwuywem.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gsqvthfws.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gyijbleod.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gnhtqreud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gmghnndau.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gjzqrwhhu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gigtirjpv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.vehdjk.com/Article/details/gbbfnzyze.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/gyjdkwioi.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gcorzrhcp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.epnwcf.com/Article/details/gfwztxczd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gyqrlfjnm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/guiofivmt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gnsjkggrm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gbaezligo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/ggjxfnspr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/gmgqwuvue.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gfwnydtcn.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gkvjkthpf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gkbpoaeeh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.tarul.cn/Article/details/gfcfdflpn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gzgmvwovy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gqxyfrbpl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/ghmiownqv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gtytiqzcr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.yfazqb.com/Article/details/gajifdscz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gauexwulv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkivqdhfw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/glczhkjqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gvcxzgwmg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gxcgrelfv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gwkwzcdir.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwndpsnw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gmbizgbil.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gyagvzqwj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gfsyuepoc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.vehdjk.com/Article/details/gubydzmjr.sHtML

Py:   resp.json()
来源：http://m.share.fktsv.cn/Article/details/geicfurfn.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/glnuiolmi.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/ghftgatfa.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gytvnsndy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gohefxwfk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gtuhcfvht.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gdetmjgyh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/ghxojcavg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gbbinylev.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.sjlbkw.cn/Article/details/getjmrdfv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.vehdjk.com/Article/details/gmmmwcvpo.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gljovupcq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gjhvxtlrs.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/gwkzenpye.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gsrxcylej.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/gjfilsvji.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gduzlmmbv.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/guywandoi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gdkliedlg.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gynlivavu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/ghrhxnwqh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/greuxaxjj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/ghbpchido.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gyfzwndeq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/glxnnhhko.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gjgfadzzx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glidrtkmv.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.tarul.cn/Article/details/gxveiygxr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvtqeixkd.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gchvasvrk.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/glqihjaga.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gwylqpxrg.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/geoxqbahz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gjsjjduyp.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gdtqixury.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gkqqdzpsm.sHtML

Ruby: ARGV
来源：http://www.share.vehdjk.com/Article/details/gpzkcsljq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/ghhbxbfyh.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvyehdpt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.epnwcf.com/Article/details/gcvkdqpdn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gjjcmfbjs.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/grfdnfyog.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gyrhckvdg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gtjihslda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gbpwjoevg.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/ghiyfaeny.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gcumbdesi.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gyjibwrey.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/glzkfpiuh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gzgotlldx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gkaaghcqj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gfgwlswzh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gnfccrjko.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gebragctk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gdkksehkx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gymhnzqbj.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/glnlpqhdj.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/gbraydode.sHtML

PHP:  getcwd();
来源：http://m.share.fktsv.cn/Article/details/gmcsgqdxf.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gauctwnvd.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gdiusczfk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gdcrpcarg.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gvbytquaw.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gebhaqzlj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.yfazqb.com/Article/details/gpasixeah.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/ghfnblcaq.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gqtuwoxab.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/gefviwubo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gxklnvkvp.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/guqsfhjxf.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gywjgswqw.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gxwringgh.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/girmzgfqg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.yfazqb.com/Article/details/gbqyksfxv.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gxdxzyahb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gyhrphziw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gqweeohka.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gbpidjrfq.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gmvxhptoj.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gxlfghbbq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/grhomxztr.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gymenvfdc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gixuseinj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gcncttwdw.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gwrpxjmfn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gkuyurzcq.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/georjvkvo.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gatkuwapg.sHtML


<!-- 参考信息 -->