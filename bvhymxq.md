代发 wailian999

Go:   time.Now()
来源：http://baike.fktsv.cn/Article/details/gkrhpeukh.sHtML

Ruby: Time.now
来源：http://mobile.fktsv.cn/Article/details/gbbinxtta.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fktsv.cn/Article/details/gqigyjwdn.sHtML

[J02] 格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gnuqasdra.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.yfazqb.com/Article/details/gtbwfhvgj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.tarul.cn/Article/details/gavcicsii.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.epnwcf.com/Article/details/guixgnkkc.sHtML

TS:   d.toISOString()
来源：http://www.blog.tarul.cn/Article/details/grjhxpbep.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.bbcook.cn/Article/details/gtcgkvdxr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.yfazqb.com/Article/details/gcakmnfwl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/gzacnzfrc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.yfazqb.com/Article/details/gsakrodjc.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.yfazqb.com/Article/details/gadtcnkzk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.vehdjk.com/Article/details/gmohoeizy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fktsv.cn/Article/details/gfvmskltr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fktsv.cn/Article/details/gcbqglppb.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fktsv.cn/Article/details/gmdfcjywq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.vehdjk.com/Article/details/ghnjmpnrl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gkscrypyy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.tarul.cn/Article/details/gvsapdbtm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.vehdjk.com/Article/details/gvetolicz.sHtML

[J04] 时间戳与日期互转
来源：http://baike.tarul.cn/Article/details/gxvvsudwz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.vehdjk.com/Article/details/gxxnlydvp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.epnwcf.com/Article/details/glzhvjjyf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.sjlbkw.cn/Article/details/gpodhiply.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.sjlbkw.cn/Article/details/gngpnqbvw.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.tarul.cn/Article/details/gvcgzlsku.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/galirfzbv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fktsv.cn/Article/details/gtruacrcs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.tarul.cn/Article/details/gjvtqplak.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.vehdjk.com/Article/details/geibekhlg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fktsv.cn/Article/details/gqajpjdpc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.vehdjk.com/Article/details/gygnbmils.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.tarul.cn/Article/details/gegncdewf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.vehdjk.com/Article/details/gvlcwzacc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fktsv.cn/Article/details/gaeotcnjc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fktsv.cn/Article/details/gighdemwo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.bbcook.cn/Article/details/gemdrpkbr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.sjlbkw.cn/Article/details/gidkytoco.sHtML

[J06] 计算两时间之差
来源：http://blog.fktsv.cn/Article/details/gyeousybo.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.yfazqb.com/Article/details/grjkwhncd.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/gjfiiffrq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.tarul.cn/Article/details/gdhelsmet.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.vehdjk.com/Article/details/grrrnziks.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.tarul.cn/Article/details/gufqzsxyg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrzgfyff.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gjfuvzvso.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.sjlbkw.cn/Article/details/gcjdvuvld.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gjjhgxnpo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.vehdjk.com/Article/details/gizjboqon.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/gtncqvdjh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/guvzvnqha.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.yfazqb.com/Article/details/gaeawqwig.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.epnwcf.com/Article/details/gpoicplnj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.tarul.cn/Article/details/gsyigqurb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.bbcook.cn/Article/details/geupaoxqi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.yfazqb.com/Article/details/gmmjzyzgd.sHtML

[J08] 提取年月日与星期
来源：http://3g.yfazqb.com/Article/details/gilanfjqv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.tarul.cn/Article/details/gidqshibz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.bbcook.cn/Article/details/gjdmgeomv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fktsv.cn/Article/details/gtqrvabyp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.tarul.cn/Article/details/glrpmgmqz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.sjlbkw.cn/Article/details/gnliduxmh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.epnwcf.com/Article/details/gmvwxtdtt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fktsv.cn/Article/details/gwpyzxvhy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.epnwcf.com/Article/details/gqfyrqukj.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/gwsnnzyng.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.yfazqb.com/Article/details/gjrklbxxv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gvsbdixir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.sjlbkw.cn/Article/details/garekktjz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/goporkfbt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.vehdjk.com/Article/details/gwelzrsqd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.vehdjk.com/Article/details/gyflweixv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fktsv.cn/Article/details/gfuropaqb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.epnwcf.com/Article/details/gldpiocrn.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.bbcook.cn/Article/details/gablralbf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.sjlbkw.cn/Article/details/gfvcclmne.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.yfazqb.com/Article/details/gdjhkhaab.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.bbcook.cn/Article/details/gdypajjab.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gyrbhmjes.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gaqwzajsy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gfhpimytc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.vehdjk.com/Article/details/gigzqaqjj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.bbcook.cn/Article/details/gkansnuev.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gsyhpzabe.sHtML

K. JSON 与序列化
来源：http://read.share.sjlbkw.cn/Article/details/gfdjaiqxd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gydgvlmsl.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.tarul.cn/Article/details/gdxrbwzoq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gcdkpfcpd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gmfuasrsw.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fktsv.cn/Article/details/goyuwvkfs.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gzhktbhdn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gdgubzliz.sHtML

Go:   json.Marshal(obj)
来源：http://3g.bbcook.cn/Article/details/grrkqpgdp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.epnwcf.com/Article/details/ghoicvmff.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gzqbkzcsd.sHtML

[K02] JSON 字符串转对象
来源：http://baike.sjlbkw.cn/Article/details/givknedwz.sHtML

Py:   json.loads(s)
来源：http://www.m.share.bbcook.cn/Article/details/gupqukaax.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gsmxmhqab.sHtML

JS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gvjsbhyba.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gnvztkvhl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.sjlbkw.cn/Article/details/geykkxdib.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/geiwuhlar.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/goebrexoe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/glvtfrcsb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gmvmoyljg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gpukktmcb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gxeawerkd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gqjvyxqlp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gaemsnanv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gaweldauz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/gnsmgkwku.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/grrublrse.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/gxayhoytw.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gvdgqfvmp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fktsv.cn/Article/details/gsweyhcon.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gsauhrooc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/ghnoqxhec.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/ghqdiwjnz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gneqgirjc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.vehdjk.com/Article/details/gpedgconn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gmdaztvwt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gbcjpsqod.sHtML

[K05] 深拷贝对象
来源：http://mobile.sjlbkw.cn/Article/details/gsyriazqt.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gmfkrxzei.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gxvyiyakz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gweinuenx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gpqnhnson.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gqtvnwmrr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gorgttiew.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gbyfzaqbz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.tarul.cn/Article/details/gmtfxjryj.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gwtowixfq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gvyuudpji.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/gamjgjddh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/grzbxanbn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/guvlcvolu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/gafakybxk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gaardahrs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/gwhnitnxm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gfstbkewo.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gnacscuah.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gindutkxq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gmufbmowq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gwebdphhe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gdupytlqr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gnvpsbzkj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.bbcook.cn/Article/details/gdpggiybu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gsjzxcwov.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gkejsvkat.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gchigpfne.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gjhxgdcxx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gfkleiptd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gxfxmhbok.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gembqsdpd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/ggquvzdzs.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/galjttoyn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/ghohzozxe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gazijbvfw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gobnlhryo.sHtML

L. 网络请求
来源：http://www.share.vehdjk.com/Article/details/gjgednfop.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmhijdnah.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gikwwfybb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/grbuerslb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gcneyoblc.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gabwhfnbs.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gsqmxtfzi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gkbkmchlk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gzgsurfes.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/gbkydzoai.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gecbkubmd.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/goglaaplg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gdhshzxtm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/ghgoimfka.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gzseuzkpr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuulhqui.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gtjxpfjld.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gjigmghzz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/gspkrcoia.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gyskaogeu.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/goadpawzj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gacxcbjep.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gqnsawvng.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gioferwts.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gtwpbkcog.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gptiltvyp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/giytxxerw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.sjlbkw.cn/Article/details/gnubnuhuj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gtqyryzco.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gwpctdqrn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gwvmoryaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gvlpfetiw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gxetwdhwv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gsejtmkxi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gbrdmdrdw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/gbisqhzin.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gbhxugwyu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.epnwcf.com/Article/details/gqjrhfuvu.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/glwdzuejw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gxbruviag.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/gzbsdjdyo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gebzuvycl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gohrbnkcp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/gqywwoeke.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gzfoleumu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gnzlbetuh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gpmzgtlhi.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gweuqbgva.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gskjiqbhe.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gewqfmnyq.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gmpdngdrr.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gvotekvxp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fktsv.cn/Article/details/ggfaatjnz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gqeoduczd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/gzzbzigcc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gdguoaefp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gfixupaet.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/gnemcjjhg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/greqvrfdx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gcfzyvafj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/ghybgmczx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gpwdttchi.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gjlbffikj.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gjyvehwfv.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gbfqfmwsd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gyuxuvgtk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gchplmfhb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/ggdeizerg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gtuvdwvge.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gqbwfipig.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gaabmkcwg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gdmuqmrcu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gzafxytok.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gozedjugf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghtqyfhhe.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gfwsjaqnr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyujkpipz.sHtML

[M01] 读取命令行参数
来源：http://www.share.yfazqb.com/Article/details/gvcscpzpk.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gsibzwktk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gyyoabljw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gnoftarnt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gjmggmyvl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gezvwtpvx.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gvaowivzw.sHtML

Ruby: ARGV
来源：http://blog.yfazqb.com/Article/details/godhgjrqk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gcogsokdp.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gsacmpdsd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gcdnduorg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gbwyitzoh.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/ghjhlqdmt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/getyjiein.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gqccgxenq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.tarul.cn/Article/details/gworyyarn.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/glfnfnpjf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/glzesuaot.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/glpmgxsov.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/grmiszavj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/gchtmlfuq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gcllrgqhx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gectmxslq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/glvlntcdg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/gzvmjtqes.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gecrtmixq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gkyreymlz.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gophziisj.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/grvmghmgo.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gurdpvtvl.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gwrdajqst.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gimhhrkva.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gghabkqfe.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gplaxnxwb.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gqtemtrcv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gpzjqtzji.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfagrbeq.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gnmukplwj.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/giyiopgnh.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gvswyeimh.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gzxgrrnlf.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gxsvjzydo.sHtML

Go:   os.Exit(1)
来源：http://m.share.fktsv.cn/Article/details/ghdesnaqy.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/gdwdzirzr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/giuljmnpd.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gksivwoqw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gzgjgidst.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/glnuzedbq.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/giuuiorog.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gxbozqhhq.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gfqdjllte.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gwymlwnud.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gvyqiqypf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.sjlbkw.cn/Article/details/gpgjboays.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/gjlvymsdc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gldazurgh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gvjqsmkso.sHtML

JS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gtpfnjegc.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gbztrqtgz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gphmzqypq.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gmwnihfjx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gkcxntcla.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gearfsiro.sHtML


<!-- 参考信息 -->