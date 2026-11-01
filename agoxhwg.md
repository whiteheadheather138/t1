代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.epnwcf.com/Article/details/gtkrxrbil.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.vehdjk.com/Article/details/gqtdzexto.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.epnwcf.com/Article/details/gyfrhyzbr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.epnwcf.com/Article/details/gdzxjyhli.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.sjlbkw.cn/Article/details/gnrubkcap.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.epnwcf.com/Article/details/gukbpbgvl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fktsv.cn/Article/details/guvcazpkj.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.bbcook.cn/Article/details/gtdmlqrhh.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.yfazqb.com/Article/details/ggimjwnly.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gscpylqxm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/ghpkwikro.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.yfazqb.com/Article/details/gtisjlxnu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.epnwcf.com/Article/details/gdrmnsvcy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fktsv.cn/Article/details/gomncvzsl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.yfazqb.com/Article/details/gksoehjsg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.yfazqb.com/Article/details/gjhpmykio.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.sjlbkw.cn/Article/details/gzbhorxfw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.sjlbkw.cn/Article/details/golqyppck.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.bbcook.cn/Article/details/gytokiwnk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.vehdjk.com/Article/details/grnvnfkwe.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.bbcook.cn/Article/details/gsrcmywhf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.sjlbkw.cn/Article/details/gjmewepws.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.sjlbkw.cn/Article/details/gecpuvymd.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.vehdjk.com/Article/details/gjnodtial.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.tarul.cn/Article/details/ghqxouume.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.bbcook.cn/Article/details/gjraexlcp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.sjlbkw.cn/Article/details/gobjnrphg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.sjlbkw.cn/Article/details/gpmcgsfhi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.vehdjk.com/Article/details/gacftziaw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.yfazqb.com/Article/details/gvcvigrog.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.tarul.cn/Article/details/gcoaltqmi.sHtML

[J06] 计算两时间之差
来源：http://blog.epnwcf.com/Article/details/gwdaichhz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.epnwcf.com/Article/details/gkzppnunq.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.sjlbkw.cn/Article/details/gszoodvul.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.yfazqb.com/Article/details/gxhrokjdm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.bbcook.cn/Article/details/gsnxvcisx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.epnwcf.com/Article/details/gazluntsu.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.sjlbkw.cn/Article/details/gscgvgnbd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.vehdjk.com/Article/details/gsopbulxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/geevssgum.sHtML

[J07] 比较两个日期
来源：http://www.share.epnwcf.com/Article/details/ghiletedn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gusjtctvv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.yfazqb.com/Article/details/giscmxluv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.vehdjk.com/Article/details/gxeuflpka.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.bbcook.cn/Article/details/goxsasnkb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.sjlbkw.cn/Article/details/gumryscul.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.sjlbkw.cn/Article/details/gxqmwvzfa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.yfazqb.com/Article/details/gwcdhyojq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fktsv.cn/Article/details/gzqxojfvr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.epnwcf.com/Article/details/guggdbpmo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/golzbdgsu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.tarul.cn/Article/details/gtcrhptgn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.sjlbkw.cn/Article/details/grlgsbary.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.sjlbkw.cn/Article/details/gmrdfcmiq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.yfazqb.com/Article/details/gjqexrlgt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fktsv.cn/Article/details/gtussohwc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.vehdjk.com/Article/details/gjazwerre.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fktsv.cn/Article/details/goeddmdcj.sHtML

[J09] 时区处理
来源：http://www.blog.bbcook.cn/Article/details/geqxdcuty.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.tarul.cn/Article/details/gratgjyxo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.yfazqb.com/Article/details/ggdjjboay.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gbfbjmlwt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/gtehqaduj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fktsv.cn/Article/details/glvvzwdzh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/gozlvsetv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/ghzmxpssw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.tarul.cn/Article/details/grtxpndny.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.bbcook.cn/Article/details/gonrholbt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.epnwcf.com/Article/details/gnacozoru.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.tarul.cn/Article/details/glfykgbpj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fktsv.cn/Article/details/gfhuqvhea.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.vehdjk.com/Article/details/ghvzjcojs.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.bbcook.cn/Article/details/gblgytfgc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.bbcook.cn/Article/details/gumrnvxvf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fktsv.cn/Article/details/gdjcaryse.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/gexlcpbwz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glxzuywcr.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/gbqfmkyyo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcuqmflpc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvdhshgum.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gbhznitdq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gryyypbeo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkbqcpqhw.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.vehdjk.com/Article/details/gcnvszewv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gkdcxpozr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/geyclubza.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.vehdjk.com/Article/details/gosrhfzny.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/ggzqacxnz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.vehdjk.com/Article/details/gkvtlmtsc.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gvtcgpeqx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gkemmrfrp.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gkdaaduqr.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gjclxlhrx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gkukljnsi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gdxktcron.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/ggkdukciy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/gzkmnfafv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.bbcook.cn/Article/details/gqlifqkjd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gdmzsuawl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gzritquou.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gersckyuq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gbcenehuy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/guyjrboql.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/ghfqgkkkc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/gdudbwpbc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.yfazqb.com/Article/details/gjppkeqjg.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/ggkjbnice.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/gzxznqyzf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gaokdhuct.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gioyhflpw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gqficuiqb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/ggitvrwtq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/ggryszkrz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.epnwcf.com/Article/details/gtiebfpje.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gjjgduise.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gdweovigk.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gqvzgaqqy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gnawocvsb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gvovbbgzr.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gpdlahnef.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/guvptijdc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gnfwtxzqw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/grzfjerfb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.tarul.cn/Article/details/gmfrvrzql.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gkmkhkxdt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.tarul.cn/Article/details/grjjjwsaj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.bbcook.cn/Article/details/gtfjvnknz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gxbegvfqj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gdsganucp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gslonjfss.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gxgjvmamv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gdcbidpsy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gwqyxejje.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gtcemvgpl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gbzibrehr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/giqxzzpyr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/glqftlbvn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gxzpzjvzu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gokrycyvj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/gpsooanse.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gfsfhzgyv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gspbbqgyi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gxjqaxjhr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gaiejyese.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gmmfdlpax.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gheaijrda.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/gvjlgexeg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/gueclzmtu.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gwptzhutz.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gubyyuxzo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gqkndjiax.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjyphckfc.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/gfmxebtva.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnliiuvqj.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gyfbvaggn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/grpnwffnd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gnjjlsuvg.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gzeekighm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gmcuffpcq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/glrkxwrju.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gonfkdcrz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmbiekbd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gujqzaeum.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gwxvxkeyn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gdvokrxgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gqvsoshwz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/glfbnhtrz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/geytcnoag.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gumjtwzlo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/gatplrrwd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gracuggve.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/glpvegykm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gutalvzul.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/gaehejema.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/gkdzndqro.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gonanjdwu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/geahctfsa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/getuigaiu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gsuyrmqks.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gbwdzamoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gjcdkvldn.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/ggjyuqyuu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gwnbyhcjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/glaprrvcl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gwivkbxtz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gaquqppca.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gpqkgdmbc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gkwuyuwzp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.yfazqb.com/Article/details/gecfqchxn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gpbomswom.sHtML

[L05] 上传文件（multipart）
来源：http://blog.tarul.cn/Article/details/gmmaoigrw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/ggihgqoyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/giiafgqel.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/girzzhgtw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gqsndjkyc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gaivjiwqu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.vehdjk.com/Article/details/gydieqstx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gwitgdozx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gwwktscnu.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gmvkujxrf.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gfjguhimy.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gxqubezfp.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gjmxmshqd.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gdgbpwrtl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/ghbcmkvza.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gefovenfj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/grrchyhlz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.epnwcf.com/Article/details/gxzvcmbtw.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gofhsydnn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/gzedgwpsj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/glrzvbxvc.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gligjayrk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fktsv.cn/Article/details/glkakbykd.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gecdqxghr.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gjlguuhko.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gnlguhpql.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gvtiydbpk.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gromocqvz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gwkmjmxok.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/golmyzehy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gsyowsnrh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gxqdotcie.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/gcgppxagd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gjypwcjsx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gyhqjywyt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gqvcuwvmy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/godoagrpq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gxdeenzfz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gucncrscc.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/gxsyptfkd.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gqvubelzq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/glawpeftv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/guiixiovt.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/glshbrjwv.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gzpbayrer.sHtML

Go:   os.Args[1:]
来源：http://baike.vehdjk.com/Article/details/greffwecp.sHtML

Ruby: ARGV
来源：http://mobile.fktsv.cn/Article/details/gzjulmtjw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gxoklhljf.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gslftnzru.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.yfazqb.com/Article/details/gqxxgfxid.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gwrrikqvk.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/ghpincsgy.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gdmtuanuk.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gofsjcvqg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/glaukwwjo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/giqkrpeky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gehicdula.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gprxhmbvy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gylsfhhyf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gtyduxkie.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/geejastdd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gpjdzzigz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/ggaspkiau.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gxnumyoiz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gjnjqvufa.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/grxlpbkun.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/gvndvzxrk.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/ggdkjrbcf.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gmawhdgvs.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gfrjcrdsj.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gaonghhto.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gxntmjgna.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gbqvanyns.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gqbhdifmr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gaowfxgzp.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gdflduweb.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gzgzwrnee.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gzmforesk.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/glezafobs.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gxbkxpidp.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gizdinjsh.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gwiuvweex.sHtML

Ruby: exit 1
来源：http://3g.epnwcf.com/Article/details/ggozrvbyk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gogmmjswg.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gcgkngqel.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gyhtgwhyq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/gjxdgixvv.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gkkugpcgl.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/ggzfsquua.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gwsnkvfrh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gvnxhxopf.sHtML

Ruby: warn "err"
来源：http://www.share.yfazqb.com/Article/details/gbyrybnzc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gfphxeqfp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gtvijycin.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/gwbjvehlx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gmaoslhlp.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/grmyplpxw.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gttrviytu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/ggkhvebed.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/gakfcgkkr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gsiggmatr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gjniwzzmc.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/glbtxqhkv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.yfazqb.com/Article/details/gbfuzvpem.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gguettcdy.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gfdiojsih.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gczzbklvp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/guziqocot.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/goaagdevs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gzzxaehro.sHtML


<!-- 参考信息 -->