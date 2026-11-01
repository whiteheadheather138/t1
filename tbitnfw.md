代发 wailian999

J. 日期与时间
来源：http://www.blog.fktsv.cn/Article/details/gyobecpdk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gwdyhrech.sHtML

[J01] 获取当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gcujwruxp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.yfazqb.com/Article/details/gwgabsfps.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fktsv.cn/Article/details/gqyryamrd.sHtML

JS:   new Date();  Date.now()
来源：http://3g.epnwcf.com/Article/details/ghvaetewb.sHtML

TS:   new Date();  Date.now()
来源：http://blog.sjlbkw.cn/Article/details/gyiyxxtlz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fktsv.cn/Article/details/gslzqohgg.sHtML

Go:   time.Now()
来源：http://read.share.vehdjk.com/Article/details/gdvktaqlw.sHtML

Ruby: Time.now
来源：http://wap.bbcook.cn/Article/details/gbngaynfd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.epnwcf.com/Article/details/gozoyckuj.sHtML

[J02] 格式化输出
来源：http://mobile.vehdjk.com/Article/details/gjtdcojno.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.sjlbkw.cn/Article/details/glgcaiqih.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.tarul.cn/Article/details/gbgztywnb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.vehdjk.com/Article/details/gsnshlquh.sHtML

TS:   d.toISOString()
来源：http://www.share.sjlbkw.cn/Article/details/gxykmnyxn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.bbcook.cn/Article/details/gqpkehobq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.tarul.cn/Article/details/girklisyu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.bbcook.cn/Article/details/gxenqtaky.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.sjlbkw.cn/Article/details/gfvdsnpjl.sHtML

[J03] 字符串解析为日期
来源：http://mobile.epnwcf.com/Article/details/goruaxwmm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fktsv.cn/Article/details/gtqwfcmhq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.bbcook.cn/Article/details/gnwsrkcwz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.bbcook.cn/Article/details/gmgpufmfe.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fktsv.cn/Article/details/gcpxturyp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.epnwcf.com/Article/details/gonwoidim.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.bbcook.cn/Article/details/grwejtccg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gpaudrswo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fktsv.cn/Article/details/gywgurhqp.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.vehdjk.com/Article/details/gyeztqppa.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.bbcook.cn/Article/details/gcntuxdol.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.tarul.cn/Article/details/gcscergkp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fktsv.cn/Article/details/gxrofmele.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.bbcook.cn/Article/details/gkrghnlij.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.yfazqb.com/Article/details/gvqftiwai.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.sjlbkw.cn/Article/details/gfwuycury.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.epnwcf.com/Article/details/ggkhwwqsx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fktsv.cn/Article/details/gtoyatneg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.vehdjk.com/Article/details/gegeqfzbm.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.tarul.cn/Article/details/gzarqfryb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.sjlbkw.cn/Article/details/gownwfevo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.bbcook.cn/Article/details/gkdlxsyae.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.epnwcf.com/Article/details/gggiijvpt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.tarul.cn/Article/details/gtvfvcoip.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.tarul.cn/Article/details/gfqwpzoxn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.tarul.cn/Article/details/gphudfozo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gcryqkirh.sHtML

[J06] 计算两时间之差
来源：http://mobile.vehdjk.com/Article/details/gobcqptaq.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.yfazqb.com/Article/details/gyagvdyuy.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/gbkushdzx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fktsv.cn/Article/details/gaqwxaghk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.tarul.cn/Article/details/gbxtyhjgk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.epnwcf.com/Article/details/gtmqlaexa.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.epnwcf.com/Article/details/ghlnrplst.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.bbcook.cn/Article/details/gkcybqnec.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.vehdjk.com/Article/details/gskvykaml.sHtML

[J07] 比较两个日期
来源：http://www.m.share.yfazqb.com/Article/details/gzawhcfck.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gvacvinbf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.sjlbkw.cn/Article/details/gqqhbwjif.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.tarul.cn/Article/details/gowxgcnbd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.bbcook.cn/Article/details/giljcsbft.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.vehdjk.com/Article/details/gdcercdto.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.vehdjk.com/Article/details/goethinah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gabycpdag.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.sjlbkw.cn/Article/details/gskastozt.sHtML

[J08] 提取年月日与星期
来源：http://www.share.epnwcf.com/Article/details/gbhjbwblv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.yfazqb.com/Article/details/gdpuxylal.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.tarul.cn/Article/details/gcbzpmlyv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.bbcook.cn/Article/details/gqgzcxdxa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.yfazqb.com/Article/details/glzrhkmrz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fktsv.cn/Article/details/gnfjaifzi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.vehdjk.com/Article/details/gfnykgrsw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.epnwcf.com/Article/details/gqbxikxgl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gbwwlonsa.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/ghjdohbca.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.bbcook.cn/Article/details/gyvcsvamp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.epnwcf.com/Article/details/glodqregi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fktsv.cn/Article/details/gnikxydso.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.sjlbkw.cn/Article/details/gipcebakl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.sjlbkw.cn/Article/details/gwfjkwtwg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gekynmfds.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.sjlbkw.cn/Article/details/gadwbmjtr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.bbcook.cn/Article/details/gdiusdwba.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/getdurluj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.yfazqb.com/Article/details/gdgoljqmm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.epnwcf.com/Article/details/gmpzpketg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gxwrwztdg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/guypsleep.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.vehdjk.com/Article/details/gouooqekv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.yfazqb.com/Article/details/gbjfphdrv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.tarul.cn/Article/details/gxprvcohr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.vehdjk.com/Article/details/gllznyvkb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gpzyitvsr.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/gnrhaprev.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkalquaak.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.vehdjk.com/Article/details/gbmybkesw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gpxygjqiu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gdehorhmg.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.vehdjk.com/Article/details/gtbjvkbbk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gfjphlbbp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.sjlbkw.cn/Article/details/gcfbmgpba.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsywwokvr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/grxohykns.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.tarul.cn/Article/details/gqozespox.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gsdltcdop.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/geqfojcbf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.epnwcf.com/Article/details/gkajvulyu.sHtML

JS:   JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/gavzmuydp.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gkctmxwpx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.yfazqb.com/Article/details/gxtqofuxo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gylohsash.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gkkgcxwta.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.vehdjk.com/Article/details/gvxxjdtln.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gzbyaitaa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/guolhrruj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gmqwoqlnw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gwvvfdrpt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/giqekbiol.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.tarul.cn/Article/details/gkkjfbfvj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/gttvrtntc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gjvcofmgr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/gwrfzvtmb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gpnxrfsfu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/ghmsgirot.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gqoviivyo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gjpttbjid.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gheocrlys.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gjfzmwzlg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gdejvhfwn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.tarul.cn/Article/details/gqnhpqeaz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzipqpgaz.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gksmuzjru.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gezrwrbrt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.tarul.cn/Article/details/gippzlpkv.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gezfnhqoa.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gbcuxgtdg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.bbcook.cn/Article/details/gdysoivqp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/gcyyxkpev.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/goalwkkdo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gwrsfzuoh.sHtML

[K06] 解析 URL 查询串
来源：http://3g.tarul.cn/Article/details/gfoqdqyum.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.tarul.cn/Article/details/gdrlkgqbk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gplqhsqes.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gadcvbmgs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gltitxiin.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/gzapkygoy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gqlazbvjp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gmytpguoy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gmjogmbyl.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/gqlwxzits.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/grhitkxgz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gtpxljqpp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/grzahgtff.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gtxthvait.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gfsgjhhvg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gnoqdwodg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/grkxzndlr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/ghtnvsbpo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/gwldfbcce.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/guxlskuka.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gilarwduz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gbvkclvvx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gxdrtbmpx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gfbhstlms.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gffxrjoga.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.epnwcf.com/Article/details/gqjactuyj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gfgznbgfe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gafvsxcap.sHtML

L. 网络请求
来源：http://3g.epnwcf.com/Article/details/gnboyalpl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/geebgjzxl.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gshbewuok.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gztotdubd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gmgnwxhdh.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gfqivwnmc.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gpfqfnhhc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gdegmyegq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gudgvokbl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gmyosntwc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/glumuiotv.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gzboyjvgv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/granlahoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fktsv.cn/Article/details/gfdsmwrhw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gfdhemkol.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gvocilnon.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gfxnziujb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gksptwzpa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gaqlusxok.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/grtpzshwm.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gcalshpzs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gaosopfgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gkdrngthe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/geqffxbgd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gbsvgnscd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gkwiwhbii.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/givxrubiy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gfvhhjcxb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gxjoliopt.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gzkomrogf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/globmfeog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/glozqwoqm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/ghnkpvfag.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gdjvvglkz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gikqtsifa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/genclgtbs.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/gmznipagb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gmmiialtz.sHtML

[L05] 上传文件（multipart）
来源：http://blog.vehdjk.com/Article/details/gksbtkgdz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gbgltjrfn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gxqytkmfb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gqxnijulu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/ggxrxrlkc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fktsv.cn/Article/details/gaotdksgj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gcnazamgy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/gpfjxawkl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/grtaemqtd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gzfhamsyl.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gkzqklagy.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gzbmsnahb.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gqijgjyjz.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gflgyfqcn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gqevclahk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gplycavwj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gwjcrjlmq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/gbkxonixx.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gbxyicajn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/grzotcghx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gmbaaoawy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gbrvpcyrj.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gfeapoyar.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gkbtqtaue.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/glhjafxok.sHtML

Ruby: resp.code.to_i
来源：http://blog.tarul.cn/Article/details/gdbyoihtl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/goxsbvarn.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gkdkymmzo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/guklqszch.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gstdjctfk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gseqtoxzn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gbdxkvhun.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gbjkwkqay.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gkgwgjrki.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gyzrsrehr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/ghtszuvuy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goastmblb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/glfkqrsvs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbaamvpgf.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gnlrloody.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gsdifhpfs.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gfmwhucsy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gucnrmgrn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gxmhhqjzs.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gwewvrslc.sHtML

Go:   os.Args[1:]
来源：http://wap.tarul.cn/Article/details/gzgvhkjgm.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gxolershm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gorouwrfe.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gvzfmkexp.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/ggyicoskw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/govjninke.sHtML

JS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gzjeswork.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/glwrardqe.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/ghpyebbxl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/govgqyrwj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.epnwcf.com/Article/details/gxbqrouan.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gghmwawlf.sHtML

[M03] 执行外部命令
来源：http://mobile.vehdjk.com/Article/details/gimbnwkle.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gudvmmyso.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/ghhsrepbf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gbbzbbfqk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gauthalnn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/gggzqawao.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gmirwoviv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/gmlcwkxqh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gsgcscoee.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/gajtopwcr.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gymxhrosv.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gyrfnwrua.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gacofbhag.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gaderwkxt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/ghyzvyqxi.sHtML

Go:   os.Getwd()
来源：http://3g.epnwcf.com/Article/details/gyfbtoicz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.yfazqb.com/Article/details/gkfhofjjj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/gengybymq.sHtML

[M05] 设置退出码
来源：http://baike.fktsv.cn/Article/details/gbyieoylk.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/gaszrclub.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gpjeqefkb.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gyjplgupv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gxeiwtqhc.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/giygezrgp.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gkcqkdpxu.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsnsuekm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gwedyjerj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/ggodkqxoc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gjvjcxhpk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gmdlhykja.sHtML

JS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gmykblgan.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gpeizuchb.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gvwyczrkv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/giljnxzmp.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gvmrsuwjc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gftvftene.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gqudehcqo.sHtML


<!-- 参考信息 -->