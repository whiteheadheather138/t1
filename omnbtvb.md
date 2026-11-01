代发 wailian999

[J03] 字符串解析为日期
来源：http://blog.vehdjk.com/Article/details/gltwtkupw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fktsv.cn/Article/details/gxbkxhceg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.epnwcf.com/Article/details/gtwhrlqqz.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.tarul.cn/Article/details/gwlbqwhjy.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.epnwcf.com/Article/details/gmhsjgrws.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fktsv.cn/Article/details/gyncweftl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gicifsgpp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.vehdjk.com/Article/details/gvlijsaez.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.epnwcf.com/Article/details/gosbdjhko.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fktsv.cn/Article/details/gcafaflar.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fktsv.cn/Article/details/gdaugdwkw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.vehdjk.com/Article/details/gwrldouay.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.vehdjk.com/Article/details/gkauvgfsw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.bbcook.cn/Article/details/ghtrqicpk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.bbcook.cn/Article/details/guwzhvoaa.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.epnwcf.com/Article/details/gqzkaytly.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fktsv.cn/Article/details/gbhwbleyr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.vehdjk.com/Article/details/gmsaylrgm.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fktsv.cn/Article/details/gyfwfrsjm.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.epnwcf.com/Article/details/gwrfklkxh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.tarul.cn/Article/details/ghdcdaspb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.yfazqb.com/Article/details/gsqiisdew.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fktsv.cn/Article/details/gdpxddnod.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.bbcook.cn/Article/details/gnmhafikk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.bbcook.cn/Article/details/gdwlgbted.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.vehdjk.com/Article/details/gvdcrgwxe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.yfazqb.com/Article/details/gmgbjbycx.sHtML

[J06] 计算两时间之差
来源：http://www.blog.tarul.cn/Article/details/gpbvtynak.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.epnwcf.com/Article/details/goaczrihu.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/glacanqed.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fktsv.cn/Article/details/gfkzatovw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.epnwcf.com/Article/details/gdwoucbhg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.epnwcf.com/Article/details/gfamyojbs.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.bbcook.cn/Article/details/gwoetmdcd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fktsv.cn/Article/details/grnhdpkxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.sjlbkw.cn/Article/details/gorktwwmk.sHtML

[J07] 比较两个日期
来源：http://www.blog.epnwcf.com/Article/details/gknnztnin.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gysieirrd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fktsv.cn/Article/details/gjfzzxpbi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.sjlbkw.cn/Article/details/gvygqqwob.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.yfazqb.com/Article/details/gsbhzseix.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.yfazqb.com/Article/details/gihpgfumt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkuyknda.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/giuvfrirn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.bbcook.cn/Article/details/gvjjguikp.sHtML

[J08] 提取年月日与星期
来源：http://3g.sjlbkw.cn/Article/details/gupwvzjbd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.bbcook.cn/Article/details/gomnieqgs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.bbcook.cn/Article/details/gceolnmpn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.yfazqb.com/Article/details/gnvncoxwv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.vehdjk.com/Article/details/gnydgfhfs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.bbcook.cn/Article/details/gvbrehhsc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.epnwcf.com/Article/details/gfwoacgky.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gmeoaumzu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.epnwcf.com/Article/details/gtlrslppj.sHtML

[J09] 时区处理
来源：http://3g.epnwcf.com/Article/details/gejcwawlg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.tarul.cn/Article/details/gvguforbf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.bbcook.cn/Article/details/gcmgpxuvv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gfzjxmatt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyuaqkgo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.tarul.cn/Article/details/ghzjadxym.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.epnwcf.com/Article/details/gkmtkdffi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.sjlbkw.cn/Article/details/geymwzgic.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.tarul.cn/Article/details/gipydhhji.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.sjlbkw.cn/Article/details/ghcbybjbk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.sjlbkw.cn/Article/details/gdclrrgfw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fktsv.cn/Article/details/gttnqrwhh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gwmotdqac.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.tarul.cn/Article/details/gkjysoeqw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gwyooajor.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gjodsegvc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/gklkfstmh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/grtyvnwpm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjbkbrdps.sHtML

K. JSON 与序列化
来源：http://baike.fktsv.cn/Article/details/gekpfnghz.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbghjmzcp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/ghtffzrgn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gvqpweeok.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/ggbgqrqwp.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gyeavglqn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gmvpzelvy.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/grtybuepr.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fktsv.cn/Article/details/gvozoeefb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gclfcuvju.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gmubfyjfy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gxwvkdhkq.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gpytbzyew.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.epnwcf.com/Article/details/guwxfuipm.sHtML

JS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gnqyyaesy.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/grvqowiav.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/ggvnfnvlw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gqplszzui.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/gtlsaymgl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gzkoyoglw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.bbcook.cn/Article/details/gurwunpxv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gxmdomnxj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fktsv.cn/Article/details/gdswawdvc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gavpreucn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gtrxvakrw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.sjlbkw.cn/Article/details/gntzvycou.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.yfazqb.com/Article/details/gnjiiaexx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/gwluggafc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/gtfnuqwmu.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/geundwfvk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gzalicadw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gfkgxahrx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gisdekovo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gdymdkpgp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/ggdszapvc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/guhbosrxk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gytbtcdod.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.bbcook.cn/Article/details/gqarkatoa.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gfonmmjng.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gvumednyy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gskxrihnq.sHtML

JS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gbbympdnb.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/ggntrmnrq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/giwmcbfor.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gomnexxal.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gifiqtwfi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/gmoypmbys.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gfsivhrkx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gbaxgqcol.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gtjhiyfhb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/greltybgt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gonmeletu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gwfwizrco.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/giolpbepj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gvlcdcacn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gzowqvvkz.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gkbpisylz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gfdvhgkou.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gzxnefxzg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gwmuivvfk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gpzpuisnu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gbvlvuqoj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gufdktknm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gvqogmmru.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gyuvtgrlk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/ganhsohfm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gnmhmnrvn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/gbfetcmbn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gvtczltgk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gtjodtxlv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gyuxfmzil.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gnarrujhu.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/govjkzdat.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/grmwgqfwm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcofcexqj.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/ghmcowakw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghkjngvmr.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gtzudetgn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/geszevuxs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/gmyizdngu.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/girwwklnf.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gxjanwadl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gcpgabrjj.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gixrvifeh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/geltxeeax.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/guupbswae.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gabiglopx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gaacmuguh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/ghdncbqai.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gmxmpxwzp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gsjvgpwzn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/ghkdmxvha.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gilvxozph.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gsuydcbhi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/ggbogrilm.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gaweamocy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/gsufvwtrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gbdkzzokm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gfkscflxd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gsuyeqwrv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gpahnaenq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gcjpyekng.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/galmbnwxe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gnopudqee.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gqwllbmjw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/glgszeyer.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gpbosyovc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gjeozadhw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gpewwsssc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gkivwxern.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gsfgsuhdl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gkjtorgvr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gpszmhqbp.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/ghhyuqmxe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/ghgifsova.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/gestuvczv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gizdzdgfx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gmxcstwzm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/ggbyykjje.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/giqkiyqzg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gubtqqmdo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gqlpohipl.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gzmsfxygg.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gepcnwxqw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/grayfftit.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/glqcveodm.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gvesgqqta.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gtxldaxzm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/ghyrxpwrt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/ghncaqrja.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/ghodbwroo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/goykjudfn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.sjlbkw.cn/Article/details/gutmejmhd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gaknkqpgm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gqcotruap.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/giruyekpr.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/genbtyyvf.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gwlmazuin.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gyrfplvjn.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gsdownttc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/grbxlrtfn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gjtiwjrrr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.yfazqb.com/Article/details/ghpnzytbq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gpbuunvtv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/guhuuaxjg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gmvrhlbsc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.bbcook.cn/Article/details/gfgjpxwjr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.tarul.cn/Article/details/glusbvytj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/geqeztpza.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtiwcagmm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/geiwboimz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwpjlsvtu.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gglomqcli.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gvjcaqxsh.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gusdfkwbg.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/grbgulmno.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gudefdsbm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gmcfxruun.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/ghdjnbwfa.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gxmtmpkqm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gfatvyfpm.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gogwwttxh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gxwnvfvtg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gpjglheqw.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gvtfbmgdy.sHtML

TS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/ghmyckwqc.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/gahtozykb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/gnlfmawut.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.vehdjk.com/Article/details/gzvafvvyk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gogrzojrt.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/glpoxusvn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gbsgrhzba.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gxomzvmqr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gudtwirsg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gxugomecl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.yfazqb.com/Article/details/gupkmzugg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gbapawzph.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gpeerkskp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gfdxyhrso.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/glrwrmftn.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gfkpjrkgo.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gmgqtueki.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gvosxdffy.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/glsgzuavr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gxnipquun.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/grgnsjgkn.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gyfpjzwmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gzylcvank.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gkbnhyejj.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gersekszt.sHtML

PHP:  exit(1);
来源：http://read.share.epnwcf.com/Article/details/gunuxatiy.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gllwuigvn.sHtML

TS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/gsvzdcxea.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gdsduwvuf.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gxjidzqnn.sHtML

Ruby: exit 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gexuqdyml.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gtxairgwm.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/ggujceuvm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gnehyyexo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/glptsmfzf.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gflwospno.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gqwevyceu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gbjwtqdct.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gevizfeaj.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/ghrgnuttc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gwrpvdrha.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/guhmjbbqe.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gkpnmdppr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gvbglrouv.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gfpmypdwo.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/ggbofgunn.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/grulpczft.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjchuaew.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gsciyjgyq.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gafaipwyn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/gcoipiync.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gdsjpjrba.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/guqxiasjm.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gpegxtkiq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/grwmylyna.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/ggbjarsia.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gjkuprgqo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gkfherhvj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gzggrxcpx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gaexcwnvo.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gaeoxgdii.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gaflqkudc.sHtML


<!-- 参考信息 -->