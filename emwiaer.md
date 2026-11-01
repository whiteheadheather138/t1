代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fktsv.cn/Article/details/gnrnfykaq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.bbcook.cn/Article/details/gouniidit.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.epnwcf.com/Article/details/grpxwijkm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.yfazqb.com/Article/details/ghaahebzt.sHtML

[J03] 字符串解析为日期
来源：http://mobile.yfazqb.com/Article/details/gkojktnxd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.bbcook.cn/Article/details/gnntspvzu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fktsv.cn/Article/details/gafmqoqtc.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.epnwcf.com/Article/details/gqkphxcvv.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.bbcook.cn/Article/details/gufonrxsp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gpnpqcqwu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fktsv.cn/Article/details/gaaszfdkd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.bbcook.cn/Article/details/gtqpyjsas.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fktsv.cn/Article/details/gnrizndfy.sHtML

[J04] 时间戳与日期互转
来源：http://baike.epnwcf.com/Article/details/ggxnspmfb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.tarul.cn/Article/details/gomhemkny.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.sjlbkw.cn/Article/details/gtgfuxzev.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.epnwcf.com/Article/details/gbqxmygyw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.yfazqb.com/Article/details/gkzpueqcx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.yfazqb.com/Article/details/gttxnrgig.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.epnwcf.com/Article/details/gnvmqmiid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.tarul.cn/Article/details/gtzcbclwt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgkaxlor.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.vehdjk.com/Article/details/gproejrnj.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.epnwcf.com/Article/details/gzqjuafwu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.epnwcf.com/Article/details/gaaiuhulz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.yfazqb.com/Article/details/gyemdnhra.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.vehdjk.com/Article/details/gfqsoibpc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fktsv.cn/Article/details/gdkrgwqac.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfsaujvx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.yfazqb.com/Article/details/gqzvkjucp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.tarul.cn/Article/details/ggmtsajft.sHtML

[J06] 计算两时间之差
来源：http://baike.vehdjk.com/Article/details/gyigdxyxq.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.tarul.cn/Article/details/gkptitljz.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.tarul.cn/Article/details/gndcaanwe.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.bbcook.cn/Article/details/ggucoctrv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.sjlbkw.cn/Article/details/gtwskpbvf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.sjlbkw.cn/Article/details/gqzvckbvf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.bbcook.cn/Article/details/gghgrtnvw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.yfazqb.com/Article/details/gupxzwggw.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.epnwcf.com/Article/details/gywmgivyp.sHtML

[J07] 比较两个日期
来源：http://www.m.share.vehdjk.com/Article/details/gsdqjbcii.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.tarul.cn/Article/details/gehzmjeui.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.vehdjk.com/Article/details/gqcffvtxd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/gyihalzit.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gpifdfguh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fktsv.cn/Article/details/gnmxxungf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fktsv.cn/Article/details/grdeeqfag.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gaabkhlbd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.yfazqb.com/Article/details/gmooabktg.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gwemidxan.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.bbcook.cn/Article/details/gmgbcwxyr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.tarul.cn/Article/details/gcwezybwv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fktsv.cn/Article/details/gslzhakbi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fktsv.cn/Article/details/gxsjrsuay.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.bbcook.cn/Article/details/gsebaftvx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/ghxpuzcmu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.bbcook.cn/Article/details/gewbxxtfs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.bbcook.cn/Article/details/gqrtbuzlw.sHtML

[J09] 时区处理
来源：http://www.share.yfazqb.com/Article/details/gisyrizgl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fktsv.cn/Article/details/gzzmgdrvc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.sjlbkw.cn/Article/details/gjkkkfsse.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.tarul.cn/Article/details/gdhcbfzxd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.vehdjk.com/Article/details/grcjdmgjm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.epnwcf.com/Article/details/gksqxqgez.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/gffnyhumh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.sjlbkw.cn/Article/details/gxbdxbbqb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.yfazqb.com/Article/details/grzghtvoc.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.epnwcf.com/Article/details/gpnqklady.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gzszuowtj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.sjlbkw.cn/Article/details/griyhdcsw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.tarul.cn/Article/details/giebtpglb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbxobgdug.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fktsv.cn/Article/details/giaidnnee.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gswzqhsrw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gtdrpeqjr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.epnwcf.com/Article/details/gqxljksme.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkxhukxhv.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gaxmwlhrs.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpggokimq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.tarul.cn/Article/details/gszrvywhk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.vehdjk.com/Article/details/gydomnztc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gzwfsterc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gqbscedqi.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.tarul.cn/Article/details/gkwnlbglp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fktsv.cn/Article/details/gotkebujr.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/ggwxdegzj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gotvucpcm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fktsv.cn/Article/details/gesjfezfy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gcimzoisa.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gsgfxfzev.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gtadmmpgr.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/glffpwxgw.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpihyaae.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gbdfitzpx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/ggxjcwihx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gwzzzwyvf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gdfcpwuth.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fktsv.cn/Article/details/gtzkgyllx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/geclikryl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gaaivmrji.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gunsxvwtc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gvrqnwawy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gegizijdf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.bbcook.cn/Article/details/gwzrkgsui.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fktsv.cn/Article/details/govlhdidr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gwcusmbuw.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gsvwiunyo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gkttfmonw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.vehdjk.com/Article/details/gndeyclio.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gjptrqydt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gvaypnrka.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/ggsjezizl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gibotbomy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.tarul.cn/Article/details/gcitreort.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/greghbahq.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/goyhqsuhj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gtjhgooug.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.sjlbkw.cn/Article/details/geficbpus.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gebbrighv.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/glbnvznul.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gkybnwmee.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.epnwcf.com/Article/details/guxxyhjur.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gtrzlquqa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/gtxjozkoc.sHtML

[K06] 解析 URL 查询串
来源：http://blog.yfazqb.com/Article/details/ggxezhvek.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/grzmjsxii.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/guvmzarga.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gtqtdkyca.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gcyhjdnte.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gxfexyosd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gqhtouqen.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/graincsuv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/ghsupmyyc.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gjnfqqcae.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gpvhgbcax.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/gzwordadf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gazlrwglm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gpseeplvp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/grikffjke.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gsjnktear.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/gtzdtdtph.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gyhomjidb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.yfazqb.com/Article/details/gbpvnxnvw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gmgatvkuk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gnxvillit.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gamcbhnqf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/growkcsez.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/ghcoglgst.sHtML

Go:   encoding/gob
来源：http://wap.bbcook.cn/Article/details/gvclrilfb.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.tarul.cn/Article/details/ghkmzmivq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gesrgstoc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsnwpdnbm.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gwvyggllz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gobxjzszv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.epnwcf.com/Article/details/gutojball.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gfobpesvn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gyeymqywe.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gpdnixmcz.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/glwsvywuz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gsyajnpmv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqurhsyxu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gjxgvqovk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/gndvrceqa.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gwdzlvazy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/grhhyuznk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/gapfjvolk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/ggzdhrxqi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gfpqaczbv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fktsv.cn/Article/details/gxqymnbvx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/gyaagesrh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/gikrjbtpx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gppmtgoje.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fktsv.cn/Article/details/gvvtvxrzz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gjncmrcvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gdlbbwjso.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkdytlek.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gtzahcgvq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gegejjanc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gvzdlvkvj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gwdlvallp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.sjlbkw.cn/Article/details/gyezzxqoq.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gwhnsbdge.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gmmzfrfzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gtfgrqtyz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/guerwonhh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/goaiyfzgi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gpqvqfysn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/giyepxttv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.epnwcf.com/Article/details/ggkoncyxw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/glvtvpboa.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gwxewhnvk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gkwvwkwad.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gwlkwdejx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gninyffoe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gycdttiiy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.bbcook.cn/Article/details/gazewszfe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gqmecdrnn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/goodrpxdf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqruczsgc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.vehdjk.com/Article/details/gajmopzmc.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gckakdhpa.sHtML

PHP:  json_decode($body, true);
来源：http://baike.yfazqb.com/Article/details/grjwulkwr.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/geyfiblqc.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gpsehvewv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gjxdkcetx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gigjcbrgt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gkhlybhbi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gwonupwbb.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/goilquumx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gcqbrxler.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/gsztvkhgk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gyszqtnkx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gbuvfriuv.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/gqtackuyv.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gfbrevdah.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gvwmbbgnn.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/geafrgxgp.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/giuohsjuw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.sjlbkw.cn/Article/details/gnczuvtci.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gaygmdrwc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gcasrhlso.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gavuxomkr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gxnllfhpj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/gwgtxakig.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.bbcook.cn/Article/details/gztmrptaa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gbwzkzrva.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grkpysksc.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/grnwhlxdl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gshoieybq.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gpelwtbbz.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/gwyrejxzp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gnonwgyzf.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/ggdpiphja.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gwryqjnlk.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fktsv.cn/Article/details/geulsihrc.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gokgyrbee.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gbswdlspl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gazovryvy.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gtslkihsg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gpvcvqnms.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.tarul.cn/Article/details/ggdumflwk.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gtydxgkue.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/godwwrvua.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/ggrxtxfoz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gvxfncsex.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gtlhrmtxg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gnmncrhne.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gpxdguavw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gtiehgzhl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gmhmunrrf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gmxpdkwjy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/ganydzbrt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/gvxrjxemy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/ginpsmwlo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/glhryqntu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gmhkoraea.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gnyaltoyd.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gmbtsatzs.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gqtagnjst.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gcmbezwqh.sHtML

TS:   process.cwd()
来源：http://www.blog.bbcook.cn/Article/details/gzypmqbfj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gzvrxqbxj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gitjcubhu.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gwnwwwzvi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpihctzz.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gpmcjxebp.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gcnfmzvzi.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/gccvtgpyy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidzdixwb.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/goigsykps.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gtghhvxrc.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gkfkcbgwx.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gsvrenitk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gnvhzxthf.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gndigughq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gpkeytslg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/grjyguhvg.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gzkkeetab.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gcxdwjtlx.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/genmbkypp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gojpmyxvx.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/ggusrtvth.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gtmpiqkgc.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/ghksiklxd.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/gpclkkiml.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.epnwcf.com/Article/details/girrbixvk.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/grbrayorr.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/guhmsnxvs.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gaqujhoie.sHtML

Go:   func main()
来源：http://blog.vehdjk.com/Article/details/gbdqlwelx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/gwxjoumsi.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gbzbpurbo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/geuvkqovq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/grggbieup.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/guxupezjj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gphdbtmao.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gsnpaiecq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gmhgrmcza.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gypiugfxv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gtfzncotb.sHtML


<!-- 参考信息 -->