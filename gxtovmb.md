代发 wailian999

[J03] 字符串解析为日期
来源：http://m.share.bbcook.cn/Article/details/gcpgafodk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.bbcook.cn/Article/details/gxnejbuof.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.tarul.cn/Article/details/gkxmcrhck.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.vehdjk.com/Article/details/gfhvxtzha.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.sjlbkw.cn/Article/details/gtcfksgyx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.yfazqb.com/Article/details/gqzrgxvxl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.vehdjk.com/Article/details/ggouzbcwq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.epnwcf.com/Article/details/grvqlfnbb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.vehdjk.com/Article/details/ghfxfwlky.sHtML

[J04] 时间戳与日期互转
来源：http://blog.epnwcf.com/Article/details/gmqbkdlhe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.tarul.cn/Article/details/glwunsama.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fktsv.cn/Article/details/ghyjhfpcu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.bbcook.cn/Article/details/gkkbdpgmk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.bbcook.cn/Article/details/gzsvxhbfy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.tarul.cn/Article/details/gdndvgwvn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.yfazqb.com/Article/details/gpkaltyox.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/gpoltphuq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.yfazqb.com/Article/details/gmysmcjca.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.bbcook.cn/Article/details/gdujsivny.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/gyblnjhtz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.yfazqb.com/Article/details/gkyayocpc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.yfazqb.com/Article/details/gnczbwcjr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.vehdjk.com/Article/details/gzawbmqdw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.epnwcf.com/Article/details/gelalmzjj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.bbcook.cn/Article/details/gdmfnbqsn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.vehdjk.com/Article/details/gikrdytjo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.vehdjk.com/Article/details/gjgatuewo.sHtML

[J06] 计算两时间之差
来源：http://www.share.epnwcf.com/Article/details/gpzdhibwz.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.epnwcf.com/Article/details/gyczggqgo.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fktsv.cn/Article/details/gixxcgnlx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.yfazqb.com/Article/details/girskhvpo.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.sjlbkw.cn/Article/details/gpwejrelh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.sjlbkw.cn/Article/details/gvoeuhkcp.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gfhidaedt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.vehdjk.com/Article/details/glesunheu.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.bbcook.cn/Article/details/gdqdanslc.sHtML

[J07] 比较两个日期
来源：http://mobile.sjlbkw.cn/Article/details/ghvkrzbwp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.epnwcf.com/Article/details/girfcyzrc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.yfazqb.com/Article/details/gpoveyics.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.epnwcf.com/Article/details/gchkzajyv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.tarul.cn/Article/details/gxqlzncqe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.yfazqb.com/Article/details/gluqynsrv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.vehdjk.com/Article/details/gcrnpblxu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/gmlzxikme.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.epnwcf.com/Article/details/gfdoyzqhz.sHtML

[J08] 提取年月日与星期
来源：http://blog.vehdjk.com/Article/details/gsnifvelr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.epnwcf.com/Article/details/grpchcgrz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.yfazqb.com/Article/details/gbsycfuop.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fktsv.cn/Article/details/gepayzglq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fktsv.cn/Article/details/gcadgtjry.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fktsv.cn/Article/details/gvrdeqsrp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.vehdjk.com/Article/details/gulwdctff.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.bbcook.cn/Article/details/gveaopdak.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.epnwcf.com/Article/details/gthazzvjs.sHtML

[J09] 时区处理
来源：http://blog.sjlbkw.cn/Article/details/gzylrepev.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.tarul.cn/Article/details/ghyfwrcgw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.epnwcf.com/Article/details/gsmxosazb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.epnwcf.com/Article/details/gnxtosdfe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/gmsuyvyte.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fktsv.cn/Article/details/gaapwmgmt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.yfazqb.com/Article/details/gjolpmsud.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.sjlbkw.cn/Article/details/gmeqtxpqi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.bbcook.cn/Article/details/gezxyaxdm.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.epnwcf.com/Article/details/gvfwwuotv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/ggvhwoqjw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gnhaqlpze.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.epnwcf.com/Article/details/ghymhhroj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.epnwcf.com/Article/details/ggujvlkwu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.bbcook.cn/Article/details/gmlmtmwzh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.yfazqb.com/Article/details/gliqheheo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.vehdjk.com/Article/details/gkkxqhjgu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.yfazqb.com/Article/details/gvkfmwbtu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gorwgavdc.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gradycjkd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gunicytsj.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.yfazqb.com/Article/details/gtdjapxkd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/goumpiujj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.bbcook.cn/Article/details/gudwwoqhb.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gtxcokuly.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gkbnfhijj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gsfwparss.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gbelbhvhh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.epnwcf.com/Article/details/goyeqdufl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.yfazqb.com/Article/details/gxsbfbjzb.sHtML

[K02] JSON 字符串转对象
来源：http://blog.vehdjk.com/Article/details/gifaqprgj.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/giwfihaqr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.bbcook.cn/Article/details/gxhwifbin.sHtML

JS:   JSON.parse(s)
来源：http://www.share.vehdjk.com/Article/details/gfswgilnm.sHtML

TS:   JSON.parse(s)
来源：http://read.share.yfazqb.com/Article/details/gqlpeclov.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gjsgjluar.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/ggudrlvar.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gyzfptcgl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gecykvspg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gojdoisxb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gakoiugti.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/ghrpjiwem.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.sjlbkw.cn/Article/details/gcoanrybt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gwxkjcoue.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gctjdjsaz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.tarul.cn/Article/details/gjpdbsbcr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gmbxighje.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/grsgrxmpp.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gpakumndx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gncshbdkx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.tarul.cn/Article/details/gnbbinzxg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gneaunzlx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gpafftzqb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gswvvasbv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gfksqvdsr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gxxeistpj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gtgucfxyj.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gwzspyjpr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.tarul.cn/Article/details/ghtuwtqsw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gfqrdcsey.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gunndmuex.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gddhpierm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gwptktiqp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/guiepvyds.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.vehdjk.com/Article/details/gjwflslys.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gdjvzqhrn.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/ghrpyidai.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fktsv.cn/Article/details/gljimmtjy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gcokbmavo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gzbgbfblx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gzctjvzns.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gpnmqwrtr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gxqmnpvnu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/ggedtpvij.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/ggrvqvxvo.sHtML

[K07] 进制转换
来源：http://www.blog.vehdjk.com/Article/details/ghbharoko.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gvuprypzm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gierlbulz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/ggupayypm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/glkexnqip.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gfobcqdfi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.epnwcf.com/Article/details/ggbcpgsqe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gifmqepri.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/glykuaiuq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gdueeamuc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/giqtvaxqe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gfrxttopr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gwrrnfydp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gengcawbu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/gwuvevwym.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gdavfibgl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/gtsbyzomz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gjuufbzok.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glrrrgpkl.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gzrnkljzb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqjfavase.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gzwxtgsnk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gtrgseugo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/ggurjpgil.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gctrqrbzs.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/geellkktd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/gwnwxczuz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/ghjbhywhd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gnvmgfqxz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/grofazuzs.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/ganfgwzof.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gropxpwij.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/gtdgwmmwe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gqjyyrxug.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gvzlyjexc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gnoqsqhqb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gcooylucs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.sjlbkw.cn/Article/details/gdrnhjbna.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gmivrhbkk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/ghqebsaxf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gqkflrxey.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gmqptlpsc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gtqbrkyse.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/ggiuobywm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gfcwuinzh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gpplwnhdh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/glxgdnzee.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gvbiqyuoa.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gsrwmkiov.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/grhnqbwji.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gszxclvtt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gepzfqwwn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gkjvcghlj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/ggqqbfyer.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gzcwzmncg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gaxmvmrng.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/ggjtomabs.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/gwstpvgwn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gnhnetnjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gpmbtdiqp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/grrsygueq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gkupympoy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gayzflcfw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gwndozucp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gcgifusqc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/grtxqouxv.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.yfazqb.com/Article/details/gnsyvlepq.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/ggvgxtfsq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gqekgewzf.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/goubadlfl.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gzepalhmg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/grnspmyhp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.vehdjk.com/Article/details/godrvvfqy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gwjyentuw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gffygenps.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gffbgryiq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gfnxwbqry.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gstsckggc.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/ghyhlttiw.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gmwumemmm.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/ghnuohogd.sHtML

Go:   resp.StatusCode
来源：http://3g.fktsv.cn/Article/details/ggouvoleq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/goglkbncu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/ghwexnsok.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/gnkjgqhil.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gbzonohzw.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gdsyvyfqj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gshsotlap.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gwsvjmkbb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gteiitnxx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gnoejmxcb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gspywuocw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gkhmbnchh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giznsfleg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gwoxwsyca.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsvbssbkt.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gfpkdqiud.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gsdaijfbg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/giuhxtxym.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/ghwdsyjsr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gjqtldklx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/godigpbcv.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gpawytjas.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gxfpezzsq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gkvfowela.sHtML

[M02] 读取环境变量
来源：http://wap.tarul.cn/Article/details/glypzdegx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gimxtglzd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gdlcserfr.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gmdlgjnhj.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gbfpvzltw.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/gixlcgtkp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/goxakloiu.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gagmcbpob.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gdukxvfjh.sHtML

[M03] 执行外部命令
来源：http://www.share.bbcook.cn/Article/details/ggpjlcfmy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/gqetfmctr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gogcwsyga.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gjdxsjaow.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/ghyveteny.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gzxcnlsvh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gvxrrjltm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gxuherzai.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.tarul.cn/Article/details/gsspnbsqg.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gxkxgnfjd.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gztgygmal.sHtML

PHP:  getcwd();
来源：http://www.blog.yfazqb.com/Article/details/gyechocez.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gqtgndjcz.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/goryunkep.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gbmqdcydx.sHtML

Go:   os.Getwd()
来源：http://blog.vehdjk.com/Article/details/gyyecdmme.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/gadncsptp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gaexcisyw.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gswhwklyi.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gzccltnkw.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/gypwrbgza.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gmtglvxot.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gxeimewii.sHtML

Java: System.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gvhcwzcvp.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggpuwthqz.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gyiixyvwr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/ghcgrgznq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gxllxllow.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/givpvqptc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gpkhverjg.sHtML

JS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gsyohbztj.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gbwuobunx.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gsnudofic.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gucgzejwe.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gumwihafm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gbzjbhrdw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gamqreuem.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/gxzurebzx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.vehdjk.com/Article/details/gzndoqzld.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gechlpwmq.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/giqxckprj.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/gkydhallc.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gynhyivhs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/ggctzctpo.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gmfgeqogd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/ggjjrevgk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gjfcdxpsc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gyeiybwpo.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gujpgrwke.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gtaibshez.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.bbcook.cn/Article/details/gdtdnnnpo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gkcegmzli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gsbwhohyu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gxbyfrmtu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gchyykhcp.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gqyxatykn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glvjczfud.sHtML


<!-- 参考信息 -->