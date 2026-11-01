代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.vehdjk.com/Article/details/ggoszlzzq.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fktsv.cn/Article/details/gabqmzlgh.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.bbcook.cn/Article/details/gmnkthxlj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.sjlbkw.cn/Article/details/gjsjostik.sHtML

Go:   time.Now()
来源：http://www.blog.epnwcf.com/Article/details/gnmedzrvg.sHtML

Ruby: Time.now
来源：http://blog.yfazqb.com/Article/details/ghyfngrvp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.sjlbkw.cn/Article/details/gopemdwsa.sHtML

[J02] 格式化输出
来源：http://m.share.tarul.cn/Article/details/gnnyhemlu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fktsv.cn/Article/details/gfpftcmho.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.yfazqb.com/Article/details/grgpdvite.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.bbcook.cn/Article/details/gvsubmxpq.sHtML

TS:   d.toISOString()
来源：http://3g.tarul.cn/Article/details/glkgtagyw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.yfazqb.com/Article/details/gttwqnsmy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.yfazqb.com/Article/details/gszoxqbpy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.tarul.cn/Article/details/guzffnoti.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.vehdjk.com/Article/details/gmqhfnyoe.sHtML

[J03] 字符串解析为日期
来源：http://read.share.tarul.cn/Article/details/gxoxjcuwr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.yfazqb.com/Article/details/giooibalj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.tarul.cn/Article/details/gbukhtayx.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.yfazqb.com/Article/details/gmvpfhngy.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/gbohpzvnc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fktsv.cn/Article/details/gfttfaboq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.vehdjk.com/Article/details/grysbpggt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.vehdjk.com/Article/details/glrdavqev.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/geytzgfqi.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.bbcook.cn/Article/details/gqqazwduv.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.sjlbkw.cn/Article/details/gnhiwwjpi.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.sjlbkw.cn/Article/details/gcrzbprum.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.yfazqb.com/Article/details/gnmpgardu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gqbzmefaf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.yfazqb.com/Article/details/ggmmpsdzd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gstriclxm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.yfazqb.com/Article/details/gnjpxhkwv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fktsv.cn/Article/details/gxnzwbkjv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.vehdjk.com/Article/details/gbxxlrhdq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fktsv.cn/Article/details/gmjmfkojq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.yfazqb.com/Article/details/gdvoccvhb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.bbcook.cn/Article/details/gjuwukwkp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/ghtshmjuj.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fktsv.cn/Article/details/gcdpetqbv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.sjlbkw.cn/Article/details/gpavmrbsp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.sjlbkw.cn/Article/details/gotafksws.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fktsv.cn/Article/details/gxlldnjty.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gfhfjhojp.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gskydmdpb.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.bbcook.cn/Article/details/gzsxzqyck.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.epnwcf.com/Article/details/gpqvxrpji.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.yfazqb.com/Article/details/guttilyjv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.vehdjk.com/Article/details/gbzpbteng.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/germdkaau.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.bbcook.cn/Article/details/gmducloam.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.tarul.cn/Article/details/gdsfzbsyk.sHtML

[J07] 比较两个日期
来源：http://blog.vehdjk.com/Article/details/gslfoilew.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gvqbngewh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.vehdjk.com/Article/details/grpzrtbyv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.bbcook.cn/Article/details/gukkswpsn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.bbcook.cn/Article/details/ggocgczun.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.bbcook.cn/Article/details/giykityjt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.sjlbkw.cn/Article/details/glnnyclpl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fktsv.cn/Article/details/guiqtxuim.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.sjlbkw.cn/Article/details/geqcmawzj.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/ghjlhamrb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.vehdjk.com/Article/details/ghyyvtkyx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.epnwcf.com/Article/details/gdkavseik.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.tarul.cn/Article/details/gsdzdvrvu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.epnwcf.com/Article/details/gxnhbvhwd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/goatgogis.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.sjlbkw.cn/Article/details/gvzsugzdb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.epnwcf.com/Article/details/goqqmlbnj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.vehdjk.com/Article/details/gkpuahddf.sHtML

[J09] 时区处理
来源：http://www.blog.vehdjk.com/Article/details/gtkuseuon.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.epnwcf.com/Article/details/gobademvd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.vehdjk.com/Article/details/gmvxrgytl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gytvetbzn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gjjojxuyj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.bbcook.cn/Article/details/ghyuzgkgf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.yfazqb.com/Article/details/gyuyjwfsq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.bbcook.cn/Article/details/gnlecxvmm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fktsv.cn/Article/details/gdetwuwea.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvphryri.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/gprmehzet.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.sjlbkw.cn/Article/details/giuzglioj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.yfazqb.com/Article/details/gyntfoxol.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.yfazqb.com/Article/details/gezhanjdb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fktsv.cn/Article/details/ggmcvelif.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.yfazqb.com/Article/details/gbpmjtqag.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/gzknddscx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.sjlbkw.cn/Article/details/garwxvzwu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwbzpekih.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/glysfjeox.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gihmfjwzj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fktsv.cn/Article/details/gpcwaoofd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.bbcook.cn/Article/details/gyblesjks.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.yfazqb.com/Article/details/goruevuit.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.tarul.cn/Article/details/gszkjnixx.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.epnwcf.com/Article/details/gbihzhcit.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.sjlbkw.cn/Article/details/gnoqfmjwu.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gleneichc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/glhgjxkaj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzeslfwqp.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fktsv.cn/Article/details/ggygsjxeb.sHtML

Py:   json.loads(s)
来源：http://www.share.yfazqb.com/Article/details/gdtagkzoj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gazaflqam.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gsgngqkyi.sHtML

TS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbsikesxe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gmrlpxhwl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gdelfiwqc.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gprwqfbww.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gjnxvdjfz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gvgcibdsn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gsjnkhrqt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gnnunxvlc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gciwbrspq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gjrzwfzac.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gemavrivq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.tarul.cn/Article/details/gqlbyozba.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzahwcrxy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gbwptdeay.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.tarul.cn/Article/details/gqqdbocbg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fktsv.cn/Article/details/gksqwvrag.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gkaslurnt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gjqeplrwe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gurrmgcfa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gnjmrtsoi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gcmegcmaa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gayarbepz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gxhhvleqc.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/gqzzcxoxu.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkzpqhqqi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/ggozvbrln.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gicjzriba.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gfhdxbsbi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.bbcook.cn/Article/details/gvyxjzoym.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/gsmwceusr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gpmskmett.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.vehdjk.com/Article/details/gamemahfv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gjsracdzd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gqalswceu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gfjyznggp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gedtrcrmo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gssiotszp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gyrosttug.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gdjpklexl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gjrooooan.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/grnzebwya.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/ghkaqkara.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gesgfihfn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fktsv.cn/Article/details/gsxvhmbnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gsyrywfud.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gdalbuudz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gxbrlfrly.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fktsv.cn/Article/details/gocdfpmtm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.yfazqb.com/Article/details/glkwokldp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gspwshmpw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.tarul.cn/Article/details/gmgmozhyk.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gjmtmyimv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gsnfhormc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gmsptzuiy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gnekezdml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/gjhdoawkg.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gcjjcphkg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gqynfepbp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gnckpkuex.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gigtyrlgv.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gsachnokc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdhrhkynb.sHtML

[L01] 发送 GET 请求
来源：http://www.share.vehdjk.com/Article/details/gvhcsinna.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gmwgqltxh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gtdyufndk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplzqbfhb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gaancwqgu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gysutjdfv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/gsdbirtvv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/gqhuiaaip.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/glozkafnr.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/gngdedlze.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gcgbnecnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gmaseqchl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcjyvqcr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gqibpuwxk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gthgdrjkv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gfepfpgao.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gipyrencp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.sjlbkw.cn/Article/details/gglblpftv.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/giotkhmhf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/gwfrgoiur.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/gulwajvmo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gkkddmfxq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gvestxbaz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gqbjoskso.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gnvngwsxk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcmzoqwf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gjdozeads.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gozdccwtn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gyygqmgvw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gmlyewkzd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gyyekvebi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/ghgidyapc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gbzyiksqp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/gtgmfigsi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/grlisdced.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/geeqldunm.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/gkvmyseag.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gwdvzeutz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gxvokhlvh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gywjmhtpj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/granhijhx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.tarul.cn/Article/details/gblxugbak.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gnafdgsua.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.epnwcf.com/Article/details/gzarwieiw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/greyfmbju.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.epnwcf.com/Article/details/gyhdzlahn.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gvdiyvwlf.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gddtyjqhi.sHtML

JS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gjravxmgj.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gbtzpemsy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gzsvurlgu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gjtebjchy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gdfgftgue.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gzfbfedfp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/goyrlamul.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/giwinbtkk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gnsbtfuqm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gqfzpjnzy.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gnhnedebx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gnavuvqym.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/ghgacejxr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gyvavtmwn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gzmtmfeao.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gyxflozkd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gclkwhrgo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.tarul.cn/Article/details/gxahqnoio.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gdfjzpfjr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gocarfnwp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gacjvqhoo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gcouvbxkq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gvdjhbget.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ghtbcrzab.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glzjhkbwz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gbhqcyjbq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glplxprei.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/grzlaguby.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gcgaxwtpa.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gelkzgnqz.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/goeffhygm.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gjuuhjgxa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gmbuwbzbx.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/gjkqdahoa.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gzlbplkbt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gpqnzphtm.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/ghwqaqbls.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/gliybfesm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/giusspwfe.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gamoostfz.sHtML

TS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gfmhotfnm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gyxyoamid.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gflbmqsbr.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gqqgfmehg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gdnsucqgl.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/ggwoqowfa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gxsfskqye.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gopgambbf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/giedwphrb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gutqmceuc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/gnarvdcyf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gktwpjvhb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gmunnbkoh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gqcufxvuj.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/ghucnxlkk.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gupguopia.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gvidfvgnk.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gvgblnduq.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gfzhkeyom.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/grhpajuvm.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gtqcdevzm.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gavrxhaci.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gtpidolru.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/grgfwfqan.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gnpgemeyn.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gzilsolgq.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/goqvtaxeq.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/glwgmhhun.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gxnuubpqt.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/glbqalfle.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gouigwlgf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/gjyxatncn.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gpxyiyrxi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gcagpgbnp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/glxcuvvku.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gljjrjdxk.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gxbugmuok.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/geiwwqxwo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/grjdopkdo.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/glkqlxwuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/glenalozf.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/glsxjbhff.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.epnwcf.com/Article/details/gamwffhvo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gevzaoshj.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gstsskner.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gfnyppgiy.sHtML


<!-- 参考信息 -->