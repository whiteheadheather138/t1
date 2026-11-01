代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.yfazqb.com/Article/details/gpkxghykq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fktsv.cn/Article/details/gaezmojxc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.sjlbkw.cn/Article/details/gyaacysfs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fktsv.cn/Article/details/gclwqjlpu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.epnwcf.com/Article/details/gkfaafdcn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fktsv.cn/Article/details/gtyvnhshu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.bbcook.cn/Article/details/gaqpzudsy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtqxvnydj.sHtML

J. 日期与时间
来源：http://blog.vehdjk.com/Article/details/ggaizingd.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gugkfnird.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/gvysdidlq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.epnwcf.com/Article/details/gibgcudux.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.yfazqb.com/Article/details/gfeurnnnv.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gfvenxitk.sHtML

TS:   new Date();  Date.now()
来源：http://3g.yfazqb.com/Article/details/gsiyqqsiz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fktsv.cn/Article/details/gzacoqpmu.sHtML

Go:   time.Now()
来源：http://baike.fktsv.cn/Article/details/grnjpbspn.sHtML

Ruby: Time.now
来源：http://mobile.tarul.cn/Article/details/ggehvnrjc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gpjuheien.sHtML

[J02] 格式化输出
来源：http://mobile.fktsv.cn/Article/details/giwpegrvu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.epnwcf.com/Article/details/gsmqvncjq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.yfazqb.com/Article/details/gqotvxwqx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.tarul.cn/Article/details/giamjgamt.sHtML

TS:   d.toISOString()
来源：http://3g.bbcook.cn/Article/details/gvulvrppj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.bbcook.cn/Article/details/gywasvqre.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.bbcook.cn/Article/details/gnplyxahr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.tarul.cn/Article/details/gxlxtyhxu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fktsv.cn/Article/details/gqehpetzp.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.vehdjk.com/Article/details/gkpvkdwfc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.bbcook.cn/Article/details/glgneapap.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhhtxzxg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.yfazqb.com/Article/details/gusrlohlc.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gbcaspuel.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.sjlbkw.cn/Article/details/guznasfgl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.tarul.cn/Article/details/gpdbplklz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gjvgbflgk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.sjlbkw.cn/Article/details/gesurxayh.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/golrbltpb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.bbcook.cn/Article/details/gbtgxxqlh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.bbcook.cn/Article/details/gjsquqkcm.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.sjlbkw.cn/Article/details/gdjssiebw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.yfazqb.com/Article/details/gkqfumdea.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fktsv.cn/Article/details/gicnvkgbl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gwsoetdqx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.vehdjk.com/Article/details/goeyevexi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/gaapspyla.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/gffqfsccz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.sjlbkw.cn/Article/details/gatfeyvfg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.bbcook.cn/Article/details/gtfwqnich.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.epnwcf.com/Article/details/gzayjtgpx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fktsv.cn/Article/details/gwxqjvoti.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.bbcook.cn/Article/details/gguvfyhzx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/gukeekyip.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gppzisqar.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.epnwcf.com/Article/details/gffqqgkjg.sHtML

[J06] 计算两时间之差
来源：http://mobile.fktsv.cn/Article/details/gvmgvajbu.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.bbcook.cn/Article/details/gfjjgxixo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.tarul.cn/Article/details/gjxpsgxlc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.bbcook.cn/Article/details/gpehxczir.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.tarul.cn/Article/details/gqddgrhiw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.sjlbkw.cn/Article/details/gkuywkgvo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fktsv.cn/Article/details/gzzvvvoyu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gxdtonewn.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.sjlbkw.cn/Article/details/gczcoerrz.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/ggsrrdwym.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.vehdjk.com/Article/details/gadixlbsy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/glntonuia.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.epnwcf.com/Article/details/gaqfmgggv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.tarul.cn/Article/details/gmjdmneup.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.vehdjk.com/Article/details/gweyvynqy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.vehdjk.com/Article/details/gmaxmdyzn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.vehdjk.com/Article/details/gxqggsyvo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.vehdjk.com/Article/details/gudhbqocw.sHtML

[J08] 提取年月日与星期
来源：http://blog.sjlbkw.cn/Article/details/gdmiiwwop.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.yfazqb.com/Article/details/gidnqvopq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.bbcook.cn/Article/details/geitzzjmr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.bbcook.cn/Article/details/gkyxyztpl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.sjlbkw.cn/Article/details/getnjtzlo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gpoqqhbxg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/grczbewjh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gwcxvlbhd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gqcehwnms.sHtML

[J09] 时区处理
来源：http://www.blog.epnwcf.com/Article/details/ghlxcsrhh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fktsv.cn/Article/details/grcjfiaqr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fktsv.cn/Article/details/gyxsebzbu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gnebboeow.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gpulpkaok.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.vehdjk.com/Article/details/gcrslatbc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fktsv.cn/Article/details/gnmenolme.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fktsv.cn/Article/details/gelxeknij.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/gdbgpvkrr.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fktsv.cn/Article/details/gaavqhqhw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.bbcook.cn/Article/details/gnjsmqncu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/gxkdnnkfx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.epnwcf.com/Article/details/gglrzanlk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnaoxztf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.bbcook.cn/Article/details/glutcmyas.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.sjlbkw.cn/Article/details/gghnzorjm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.bbcook.cn/Article/details/gavpsrscf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.bbcook.cn/Article/details/gbpyqvrkc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/guuhsmjie.sHtML

K. JSON 与序列化
来源：http://baike.bbcook.cn/Article/details/gbmpxdzqe.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggbcuunkm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gybgcugse.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gldxdrzzt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/ghlqkajmn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/gyysqxyyt.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gmhfdnprv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gssfrniob.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gnrhzbiic.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gexpofblg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/gebipztpo.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/ghmbhetzu.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/grqqpxicp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gykkaqach.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/ggjwvzepw.sHtML

TS:   JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gnlfbfolc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/glhlpygqo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gsfyruomx.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gxyzoexxn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/geuwoqwne.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gtjvufbqt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.yfazqb.com/Article/details/glbjbwyyh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gufwgtpqf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gofbibdfd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gfbybcipb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gaalfqugg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/grfwiwfjj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gsnqdborw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gnyjvilbn.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gficdelnk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjlvoezsy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gohqkeeui.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gfwlktzlx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gvqpjvcev.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gjeruhirc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gqbrcjbdt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gfhvopmdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gafyznvwe.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gkmefegmm.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/ghqrokhag.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gviqzhyxt.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gtvykkfyg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gztsgcsda.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.bbcook.cn/Article/details/gsxgfphfk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/galgedjha.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.epnwcf.com/Article/details/gcsgkxdji.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/gylntmazf.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.yfazqb.com/Article/details/giemdpaiw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gptfvpdez.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gkpqsbdns.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/ghaciurgw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gcdralsoy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gzzgrmyje.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gvnaosvfh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gqrrvpoto.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/ghraxposp.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gazukzhtj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gkrimuebn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.epnwcf.com/Article/details/ghcevwtwf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gvjymjgna.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gpvfpbfmc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/glijeopho.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/gidaywnqj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/glqwdsnre.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ggujixwqk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/gqpnfoues.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gtuyocnsk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gzwipxjmz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ganjvsdxu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gdwszmvxx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gdqqfclzx.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gndqzsyxy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/gaicqwhni.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gnvxkrawb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxnpmjnxo.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gkjpzwqax.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gnzguzqlf.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gwnufyxjy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gafipjlvj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gigxmxvwv.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gijzgiznq.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gfdiancas.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/golszxprd.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gmldzlypz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gnohcubtj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gcaousrlm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gsvomeziu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gaesbsgmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.bbcook.cn/Article/details/guaykohli.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gqdeijvkm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gdwmtxyhj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gpcwkuqky.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gvbbywxub.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/gxawglhqi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gsdepjxck.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/galuordhq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gpcmfjrda.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.bbcook.cn/Article/details/gxmmuasqe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/ggbycpqog.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gpqizmvwk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/guoxiybac.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gotysnkwy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gcnwwllxv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/globvuzls.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/glurelslp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/gvzflkhnd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.tarul.cn/Article/details/gcksaauli.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gltfvlpva.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gudemfoez.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gjscekoar.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gwpzflzde.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/glzaxpfcl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/grzualmua.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gicpkqkkd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gmacfskmz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gjctynapu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/ghapsfbvs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gsxrtpljm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/grfgsldgc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/ghnldyyfh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/gxkytsgbk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/gvjvzekrv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gqhbtjbbt.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gplbcfclm.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gsmnyxaih.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gbhulprwl.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gecjmeytv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/glrhnaqth.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/grliekyog.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/gvudwygwo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gbfyrkavi.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gxhamulfm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gohiuctjb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.sjlbkw.cn/Article/details/gelzipzqo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gclbqalvn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/ggbzpivzj.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gkaxqomjk.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/ggcsopgpa.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gfpgkjmxq.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gtgbitdfr.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/grsslfrlr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.yfazqb.com/Article/details/gqbwdzqze.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gkqxhbxop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/ggyyobpfn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gcmvmphrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gcjclfmga.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.bbcook.cn/Article/details/gipjsmimu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gmdwpqkxg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gsseqgffs.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjuqkuvai.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gbmwqtvtx.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gllscioqw.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/ghvubwewa.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gndxuslof.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gmlazbozv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/gffqpywma.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gflivfybv.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gnedvkoux.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gmbbjzrpr.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/gudseiupl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gbdlsqklc.sHtML

[M02] 读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gcouksvai.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gextbekak.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gajclhrpa.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gylrthttd.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gvbfzhxyk.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gcvemtjvt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gryezmjte.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/gntkvkbso.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gmloxgnkd.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gakdlkczh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gjtjqyjic.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gpltobdfp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/grindlsjn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gkebzsvby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gxacqhpgm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gsyoinrjt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gkmpudoko.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gbabxndne.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gifgwrtqz.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/glociiymn.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gvfygdfbp.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gfnfnaidu.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gpqujhqee.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gzsuigowk.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gghxkslcn.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gvyfjiusx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/glngihdzl.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/glllmvolk.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/giazhxwsn.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gjdeoatjv.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/glhfexxju.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwaxwuvam.sHtML

Java: System.exit(1)
来源：http://baike.epnwcf.com/Article/details/gfppjtjvg.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/glevxidps.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gacbmeljz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gpsoudlvu.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gnwegruxa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gxfvzivjv.sHtML


<!-- 参考信息 -->