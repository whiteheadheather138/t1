代发 wailian999

J. 日期与时间
来源：http://www.share.sjlbkw.cn/Article/details/gsjwodcru.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzampeouw.sHtML

[J01] 获取当前时间
来源：http://read.share.tarul.cn/Article/details/glzsolobx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.epnwcf.com/Article/details/gligkuynf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.vehdjk.com/Article/details/gxkmqdfxn.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.sjlbkw.cn/Article/details/glpyokvxm.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/ghzopjget.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.yfazqb.com/Article/details/gvfiwyjfs.sHtML

Go:   time.Now()
来源：http://mobile.sjlbkw.cn/Article/details/gvsruxwxa.sHtML

Ruby: Time.now
来源：http://www.share.epnwcf.com/Article/details/ghnxbccxe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.epnwcf.com/Article/details/gnhpguhdu.sHtML

[J02] 格式化输出
来源：http://read.share.yfazqb.com/Article/details/gjfvswiqf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.yfazqb.com/Article/details/gdkhsnoze.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.bbcook.cn/Article/details/glczjsuud.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fktsv.cn/Article/details/gsabtdgxn.sHtML

TS:   d.toISOString()
来源：http://blog.yfazqb.com/Article/details/gobtktqml.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.yfazqb.com/Article/details/gkabtrkvq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.vehdjk.com/Article/details/gjumugkpl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.vehdjk.com/Article/details/gzhpzdqqo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.bbcook.cn/Article/details/gtrmoctgk.sHtML

[J03] 字符串解析为日期
来源：http://3g.vehdjk.com/Article/details/gjcxkjrkg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.tarul.cn/Article/details/giinnxqqd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.vehdjk.com/Article/details/gzdvaeoil.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/ghiefoclv.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/getswiloh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.epnwcf.com/Article/details/glofybnsq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.tarul.cn/Article/details/gyfsbherp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.bbcook.cn/Article/details/gxtifvely.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.bbcook.cn/Article/details/gfugtdhae.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fktsv.cn/Article/details/ghuljhiwe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.vehdjk.com/Article/details/gutrehwql.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.yfazqb.com/Article/details/getpqtxmi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.bbcook.cn/Article/details/gyiiidijs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.sjlbkw.cn/Article/details/giyljrcld.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.sjlbkw.cn/Article/details/gspgphyvz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gpvibvvyn.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdexujtsn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.tarul.cn/Article/details/gqcntftyh.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.yfazqb.com/Article/details/ghkqmnbot.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fktsv.cn/Article/details/ghysdbgtx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.yfazqb.com/Article/details/gizmcwbxh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.sjlbkw.cn/Article/details/gwyevorir.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.epnwcf.com/Article/details/gzphvtvxg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.yfazqb.com/Article/details/ggipxpqhi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gwrvjtrwd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.sjlbkw.cn/Article/details/gypkgjivu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fktsv.cn/Article/details/ggfgehirc.sHtML

[J06] 计算两时间之差
来源：http://m.share.sjlbkw.cn/Article/details/gukdqixxr.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.yfazqb.com/Article/details/gphxwpcew.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.yfazqb.com/Article/details/gherrnrrq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.bbcook.cn/Article/details/gzbyfshon.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.bbcook.cn/Article/details/gezxyxjks.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.epnwcf.com/Article/details/ggwbrqqkw.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gikyrjalt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.bbcook.cn/Article/details/gsdsrzzxh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.bbcook.cn/Article/details/gglyewxhn.sHtML

[J07] 比较两个日期
来源：http://www.m.share.sjlbkw.cn/Article/details/glgssspnr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.tarul.cn/Article/details/geuktakky.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.sjlbkw.cn/Article/details/grldlpuuj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.bbcook.cn/Article/details/gbfcyvulo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fktsv.cn/Article/details/gjhflldup.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.epnwcf.com/Article/details/ggopunrnd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gmchcaeod.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gucqshwxt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/gwukwpuoy.sHtML

[J08] 提取年月日与星期
来源：http://baike.epnwcf.com/Article/details/gyzsrooww.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.bbcook.cn/Article/details/gvxfdhbtj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/gchmyhguz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.epnwcf.com/Article/details/gxcnmzwme.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.bbcook.cn/Article/details/gseihumil.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmvirrcp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/ghaxndptl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/ggvdcebnf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gqtexgrqa.sHtML

[J09] 时区处理
来源：http://mobile.sjlbkw.cn/Article/details/gufzxhldp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.yfazqb.com/Article/details/gqxmbdahq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.sjlbkw.cn/Article/details/gpmyylevt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gqtawzedr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gmilvhjxs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/glrufefhl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.epnwcf.com/Article/details/gzdczyufs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.epnwcf.com/Article/details/gsxigsiyj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.tarul.cn/Article/details/gdlofceki.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.tarul.cn/Article/details/gsjocnanh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.sjlbkw.cn/Article/details/gelqpvpjv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.vehdjk.com/Article/details/geiugrmjy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fktsv.cn/Article/details/gadfenidl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.yfazqb.com/Article/details/gqmbqbzsx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.tarul.cn/Article/details/gjcctbhsr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.epnwcf.com/Article/details/gtonztjxi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/grrfhgaal.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.sjlbkw.cn/Article/details/gpzduajml.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsepuawbo.sHtML

K. JSON 与序列化
来源：http://3g.sjlbkw.cn/Article/details/gwrzvtwjs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmhvonng.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.sjlbkw.cn/Article/details/girmcdrrx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gepfgnayq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.vehdjk.com/Article/details/gdszuggfz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.epnwcf.com/Article/details/gxwvzivgq.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gazbhnmue.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/gxzhnqazv.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/gfbnczkxw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gztemazsx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gxdcwydxz.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.epnwcf.com/Article/details/gojtyzoaq.sHtML

Py:   json.loads(s)
来源：http://blog.yfazqb.com/Article/details/gjrqlgqgt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/gorpqzovb.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gmzndmets.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghlyllumm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fktsv.cn/Article/details/gxkvxtthj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gqacqgofl.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gjczgijuv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gjlfcibub.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gednuktmr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gltxrqegy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gbkzxsgrs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gujsuycxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gvwkdqtqg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gesgmccha.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gxumnkmph.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gifttmufk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gbjssqjnj.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fktsv.cn/Article/details/gtlwnimqe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/ggquefjeu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gdeyehdtj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gkpbkiiay.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/govynbdiz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gmgkgozvo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gzqjtjjiw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/gnilodgzk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/ggighujwi.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gsowzdjfa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gmteuvfrg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gpyirfrja.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gduzkxtom.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gyfflnqbd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/gleaoryat.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gmkbgpjda.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/ggelnywep.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fktsv.cn/Article/details/giqniaccn.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gcmufwkkc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/gsusyvmuk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gjqtpfwap.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gikjemmzk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gcpmeduju.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fktsv.cn/Article/details/gvnmtywfm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gjjprxbwy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/geydtrmvp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gmfdoxeem.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gvvnhtvfe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gybmlafhm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.sjlbkw.cn/Article/details/gjzfrmqgq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/glmdjbvzn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/goxfbvrsp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/glnpxnihx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.vehdjk.com/Article/details/gevirsaqe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/gyqdgtzot.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gchvpqbmk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/ghibioydj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/gngkwjgiz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.epnwcf.com/Article/details/gulhxfxrc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gxhaaoter.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gbpmazudx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gdfsatybq.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gxkzamcki.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gkhzjjhpd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gyypwsjlr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxzjjkcou.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gjoydnyka.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcgvraieo.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gsxvbdrug.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.yfazqb.com/Article/details/gjpfulfpk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gsdkfcsvg.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gfabpmrjp.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gproabysn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fktsv.cn/Article/details/ghypmaeuq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gvtsptihm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.sjlbkw.cn/Article/details/gfdhzfsel.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gdatjnkdd.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gqjbvvrsg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gllvvffgb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gegieddtu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gbwgmnhhf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gxgcwdcyg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/goyayfgrk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/goystlsed.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gbnasfivx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gekcmnsuk.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/gquyfgbsd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.yfazqb.com/Article/details/giguhfcch.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.sjlbkw.cn/Article/details/gbwryboar.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/ggsqnucoj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gaudcuwpa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gcyirekrz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/grrnodfob.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gwwtxluov.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/ghfjuofse.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gqwyudruw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.tarul.cn/Article/details/gkymqxemh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/girqkqfip.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gfmonqltf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/genblljec.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.sjlbkw.cn/Article/details/gsuhvqakb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gllccpooc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gllqltsou.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/gymgvvhmc.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gnqarzthp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/ghhjlgtnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/guxaoctmb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gkftsniez.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/grrvxagqp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.bbcook.cn/Article/details/grmrcuxcg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gdfaqywgx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.vehdjk.com/Article/details/gfsdabgef.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gursvpiwd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/gjzupioxi.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gscokonbs.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/geepgohnl.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gqgeyfanu.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gifklleve.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/ghlhhfqmr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpxwhlun.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gocjwknqz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.epnwcf.com/Article/details/gzbvvrsbl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gsearhfgm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gjzhhtltv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/gkeswaqdd.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gxgkzgrqe.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/ggizlnhgr.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/gyfypmmwi.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gttjnkjds.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gyqypwteg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/giwmlnykx.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrmtevrt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/ggtsyekxq.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.bbcook.cn/Article/details/gwgycffpi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gkmwoszeo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gdyyfgzkm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gywvhscte.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/gqxneeeby.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gbzidstex.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.vehdjk.com/Article/details/glkxjuoal.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkakyppmw.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gppranxly.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcepzjviy.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gtslzaxci.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gmazyuuqo.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gscijmwlk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gajxayylp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gdvzcbqnj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gunaizwuc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gincrgunf.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/gkuwpcump.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gpyjoxyrt.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gmjghwori.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/ggfrbsowx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/gvzwkniup.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gzlzcfcyk.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gdugvensl.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gmnzpeuax.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.tarul.cn/Article/details/goscybiqj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gyfzdafir.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gqaitbrpi.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/gmazbsyeo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/grtxoraed.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gsfeietra.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gtrmaqfqu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gicdpumks.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/gzebksgql.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gtvsfyubd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gelsudaoy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gdharuiby.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/glmwjmcvr.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gzzfdecok.sHtML

PHP:  getcwd();
来源：http://blog.yfazqb.com/Article/details/gwfwoaqjc.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gndxdxcld.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gextjdifu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gepnjpgjw.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gtdeljewr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/gltkgpvxb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/gbbxwtzci.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/glijdpgei.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gennkcejc.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/geaihugpf.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gwohkjzxi.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gazotawqs.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gwgjfpgkx.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gtjslotlx.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gpjsknhcw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.yfazqb.com/Article/details/gktagpwub.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/gwtzseupk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/grqfcrlas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/grljdsdef.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gcizmfwod.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gmzofdojm.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gqclklnwd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gqxkqnwni.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gxexivaza.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gzqpbmhxn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/grschzjlx.sHtML


<!-- 参考信息 -->