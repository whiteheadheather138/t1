代发 wailian999

[J03] 字符串解析为日期
来源：http://m.share.epnwcf.com/Article/details/gzqxmghjn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.bbcook.cn/Article/details/gcttrijxq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.epnwcf.com/Article/details/gswwyntpb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.yfazqb.com/Article/details/giyphjnjk.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.vehdjk.com/Article/details/gtlprxxbd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.sjlbkw.cn/Article/details/gmmyaruzq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fktsv.cn/Article/details/gehbiraud.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.sjlbkw.cn/Article/details/gzrxebivv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.yfazqb.com/Article/details/gfjawldmo.sHtML

[J04] 时间戳与日期互转
来源：http://blog.yfazqb.com/Article/details/guyhdqszp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.tarul.cn/Article/details/ggnfrojmy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.vehdjk.com/Article/details/gukxuiwke.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fktsv.cn/Article/details/gaimdvcpr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fktsv.cn/Article/details/glhpoojxr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.vehdjk.com/Article/details/gxkcdwkzs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gqyibabik.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.yfazqb.com/Article/details/ghklzaxmp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.sjlbkw.cn/Article/details/gagnbpesd.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.sjlbkw.cn/Article/details/gvftlzftc.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.yfazqb.com/Article/details/gkkeshera.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.vehdjk.com/Article/details/gkwhgzjav.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.vehdjk.com/Article/details/gcpshapip.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.sjlbkw.cn/Article/details/gpinilehs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.epnwcf.com/Article/details/girzemzai.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.bbcook.cn/Article/details/gasersgyk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.yfazqb.com/Article/details/gaucynfbh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.vehdjk.com/Article/details/glhtrtyzc.sHtML

[J06] 计算两时间之差
来源：http://www.blog.yfazqb.com/Article/details/gksrvulor.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.sjlbkw.cn/Article/details/goiijajae.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.sjlbkw.cn/Article/details/glygqwbvj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.tarul.cn/Article/details/gtergnjij.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/ghxtkiumk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.vehdjk.com/Article/details/gchtlxlhk.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.bbcook.cn/Article/details/ghgegurvp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.yfazqb.com/Article/details/grftartfg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.tarul.cn/Article/details/gglxsvvjf.sHtML

[J07] 比较两个日期
来源：http://read.share.yfazqb.com/Article/details/gwpcwduxz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.tarul.cn/Article/details/gubjqyzmq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.epnwcf.com/Article/details/gshqaqowe.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.vehdjk.com/Article/details/gbtudvsff.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gtlleimts.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.vehdjk.com/Article/details/gohsqjxgr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fktsv.cn/Article/details/gmhniqusv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gbshwzhwa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.epnwcf.com/Article/details/gibvbeisd.sHtML

[J08] 提取年月日与星期
来源：http://mobile.vehdjk.com/Article/details/gfclppgcr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhcpgdhp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.tarul.cn/Article/details/gzkxdbugx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.tarul.cn/Article/details/ghmnvjmft.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.tarul.cn/Article/details/gvplfhgab.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.yfazqb.com/Article/details/gxwwixium.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.yfazqb.com/Article/details/gzelndnud.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.tarul.cn/Article/details/gtniytaym.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gtelrhzxj.sHtML

[J09] 时区处理
来源：http://baike.fktsv.cn/Article/details/gdhxvpeut.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gekjebkxq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fktsv.cn/Article/details/gvuicgacv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fktsv.cn/Article/details/gjbdovtdr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.vehdjk.com/Article/details/gzakmpdha.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fktsv.cn/Article/details/gvvzgkwlk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcjvzsxp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.vehdjk.com/Article/details/gsnijgfov.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/gptocvkqd.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.yfazqb.com/Article/details/gzrtwuptq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.tarul.cn/Article/details/gnjdtmevd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gkrnwhthg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fktsv.cn/Article/details/gqvlaiocv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gpidbommj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.vehdjk.com/Article/details/gakqfwbzv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gywfgtnuq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/gmiqsqscl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxgvldkk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvqojejmu.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gqobvgido.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsagmpsbu.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.bbcook.cn/Article/details/gtihubdyo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.bbcook.cn/Article/details/gqoqacnsb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/ghumgeuwr.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/ghpwitnwx.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gxxiwsfll.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fktsv.cn/Article/details/gkkrorvoy.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.epnwcf.com/Article/details/gqesecnpj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.yfazqb.com/Article/details/geeszhiya.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gzdlsivvx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.tarul.cn/Article/details/galldruvs.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gdzlztbmh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.epnwcf.com/Article/details/goglndhns.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gbhtkuawb.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gpvnuokbu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.vehdjk.com/Article/details/gtmakiazj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gfzgsizob.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gatcgecex.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gdxkkeerh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gtsepclbz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gbudulpgk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/giaxeabny.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/givhozucb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gslotrysj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gwsicxdxf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gnuertyls.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpeqlbfqi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/guxwvemyo.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.yfazqb.com/Article/details/gyayshago.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/ggtwfyuat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/getygjqge.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gpdufpsfh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gjldwssnw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gmdndccln.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.tarul.cn/Article/details/gourqtfzw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gllofengy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/grnzbxkch.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/ghwxaepgx.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gcjvpkajs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.yfazqb.com/Article/details/gttyxneha.sHtML

JS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/gxvlnrdxw.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/geohtssfe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/glpbfvujb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.yfazqb.com/Article/details/gbsrbssna.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gexqzfemf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gplbymiwb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fktsv.cn/Article/details/gqizuzgmy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gpzxqidao.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/ghkktwuft.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gvxluyerd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gxlayauaf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/ggwffaxil.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gzrfzzgun.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gucjdedmd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gnwrrqqlz.sHtML

[K07] 进制转换
来源：http://www.blog.bbcook.cn/Article/details/gnsrmqejp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gwjuazbld.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/gkvftkhyc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gmozmuuuc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gtputdlxm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gxvxwwbik.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gmkrghddy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwscxhezz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gurgnfpfz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/givrlaebb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gumtqabjb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gehickalv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gfppflzxq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/ghlnhgsdm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.vehdjk.com/Article/details/gnimgwfxp.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gocfknesx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/grkdvsfub.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gszxvgtip.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxfmutbeq.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/ghlqzuepn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gndzodknm.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gdyastiyr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/ghwizmvht.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/gfkepjwyd.sHtML

JS:   await fetch(url)
来源：http://m.share.bbcook.cn/Article/details/gmvzqoirc.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gspdrsreb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fktsv.cn/Article/details/gybhmxxpj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/glqhcmeeu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gxdplftjx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gxymvlzyw.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gquskzcmz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.vehdjk.com/Article/details/gfkpoiujk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/ghykqdvvx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gdqlpzobv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gxcqvojit.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.bbcook.cn/Article/details/gvjbojlgl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gwozupndm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gfclsvoir.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.bbcook.cn/Article/details/getrynuuc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/grafjumta.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gbojwpzhm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gherahrjr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gfnarxlsb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gmupinvtq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gkrsugono.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gqdreqorb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.bbcook.cn/Article/details/gsafsvypd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gdsrfsabr.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gwxcxgtps.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/gqpfjdzuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gtjrmtxbs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gasxjcawj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxdfdpnic.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gsuzwjuch.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gwqawsiav.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gfqxeufea.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/goyhxcdwf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gbprxeyej.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gwxvmutwk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/guopcpjyj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gjjxeegkk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gcpiuysfj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/gthndouqt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/gmwngbsca.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.tarul.cn/Article/details/grvnrgncl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gqmfxovcu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/grqcevtvj.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/grqfkipxg.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gppqdqnrb.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gzbpvjtbn.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/glrxoamyl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.tarul.cn/Article/details/gcvlutucb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/gkeyptbde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmohokra.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gaknveeys.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/giypogvti.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gmlzdwdtr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/glxbxojyi.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gyhxywjxe.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gcqachilt.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gijdiwgqj.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gnfvgxerf.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/glljuemgy.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/glkihjvpv.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gfazqcmba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fktsv.cn/Article/details/gkqbfutyl.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gmvxlisvh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gqttivaxv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gtgfauytd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/gizpeekva.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gsskbkwhj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gqqpxdfha.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gxbjedcge.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzrlpaenj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gtwwvxver.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcgugzvcc.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/gdmdreybl.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/gdgmnjezk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/galcoblsr.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gqbqdyxdz.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/glgsbftxh.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gixenjedh.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gpeiztoqc.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/gzfhcbkqz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gdegwqfwu.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gvpdfaxla.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gcldzebhb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gcptncxrl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/ghhugvequ.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gbgiuxsxw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gzsenxsbi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gswkmdbgo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/ggwryblvz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/gmnzbvfvq.sHtML

[M03] 执行外部命令
来源：http://read.share.yfazqb.com/Article/details/ghkcinfqf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fktsv.cn/Article/details/guzcqkgrr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gwhsfhsik.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gfdisvzvt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gzztuxmml.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gzoqzfvos.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gganhjfbj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gzozkcksu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gabmcdbnf.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gspqkqxix.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/ggbthimci.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gyabojhhf.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/goxndxypd.sHtML

TS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gdaaryotm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.epnwcf.com/Article/details/glfkgohne.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gqtjzwypm.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gwumgamyd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gmxcvzhwh.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gmaiyrica.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gyhbbpjlv.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gumtapiad.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gquvhsdbw.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gousiauxm.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gquxojzon.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gftznxxzg.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/gbnhpvwza.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gbpjwbszt.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gdnuxujfy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/glqlnpmrv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdownoyi.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gwebbbymg.sHtML

TS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gwjmniqvz.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/gzuzduyic.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gwntugfbl.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gmtsuxfje.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/grbvntvsw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gzabthzpr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gvawlzuwu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.yfazqb.com/Article/details/gvtmkeojm.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gqzuwmhtw.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gkncrgjey.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gbguquhjf.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/gghogbjfb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gwcqotuzm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/glfonpwyr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gwdudeams.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gfzwhclvz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/gneqjcwvf.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gpewncxia.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gffnnfkih.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/grbcuendp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/guobtvxla.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/gkqxnbevl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gakckfxna.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfrxwlpdw.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gzysoeoyw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqzgsystk.sHtML


<!-- 参考信息 -->