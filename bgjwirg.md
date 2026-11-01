代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.yfazqb.com/Article/details/gzwihczzj.sHtML

[J04] 时间戳与日期互转
来源：http://blog.fktsv.cn/Article/details/geypnoqbm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.bbcook.cn/Article/details/gowukrzxm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.yfazqb.com/Article/details/gqbndgobd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fktsv.cn/Article/details/gxxygnrpe.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.sjlbkw.cn/Article/details/gmqiqtfct.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.epnwcf.com/Article/details/gvgrabfrw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.sjlbkw.cn/Article/details/gqxgnekfj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.bbcook.cn/Article/details/geusifsgp.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.bbcook.cn/Article/details/gkgnxddkl.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.tarul.cn/Article/details/gkwtyrysr.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.vehdjk.com/Article/details/ghpgouaxt.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.tarul.cn/Article/details/gweqnyalq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.epnwcf.com/Article/details/gaykludxq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.vehdjk.com/Article/details/giuurejbb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.tarul.cn/Article/details/gpyfrtseg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.yfazqb.com/Article/details/gfqeihlsg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.vehdjk.com/Article/details/givteauwv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.vehdjk.com/Article/details/gsunnjpmk.sHtML

[J06] 计算两时间之差
来源：http://mobile.yfazqb.com/Article/details/gmnbieyfc.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.epnwcf.com/Article/details/gilmaeqqa.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.yfazqb.com/Article/details/gkofhkhxi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.bbcook.cn/Article/details/gsxrwasbq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.tarul.cn/Article/details/gttzljpjb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fktsv.cn/Article/details/gfoaekiho.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.vehdjk.com/Article/details/gehymozri.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fktsv.cn/Article/details/gpgngiqeu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.bbcook.cn/Article/details/gukvvdevr.sHtML

[J07] 比较两个日期
来源：http://mobile.bbcook.cn/Article/details/gjckbfuei.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.epnwcf.com/Article/details/grfvbglvs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.bbcook.cn/Article/details/gncgtqaor.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fktsv.cn/Article/details/gkxkpdycy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.yfazqb.com/Article/details/glvklomqi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.sjlbkw.cn/Article/details/gxgjppzlv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.sjlbkw.cn/Article/details/gajujkkjb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/gfafzimec.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.yfazqb.com/Article/details/gzhaakuov.sHtML

[J08] 提取年月日与星期
来源：http://3g.tarul.cn/Article/details/gbzxznzim.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrebnhcb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.bbcook.cn/Article/details/gmzkufwaa.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gsfmrrnpw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.yfazqb.com/Article/details/gwfmdnplc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.yfazqb.com/Article/details/gmfdxnodx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fktsv.cn/Article/details/gkvtnbyqp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.vehdjk.com/Article/details/ghmeoerzx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.vehdjk.com/Article/details/gsjpnfhoz.sHtML

[J09] 时区处理
来源：http://3g.vehdjk.com/Article/details/ggkqeafsr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.yfazqb.com/Article/details/gveptqwps.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fktsv.cn/Article/details/gxopqsvpi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.yfazqb.com/Article/details/ggfizwlof.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/giddxybsj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.vehdjk.com/Article/details/gtnfytkak.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.vehdjk.com/Article/details/gsomupxkf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.bbcook.cn/Article/details/gmmypsvdj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.yfazqb.com/Article/details/gidnydpme.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.sjlbkw.cn/Article/details/gorhpmosp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/gjgzaojid.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.bbcook.cn/Article/details/gqtkrcjip.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.bbcook.cn/Article/details/gestriazr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gejgnvwta.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.tarul.cn/Article/details/gymnzpfnb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.yfazqb.com/Article/details/glbjedqsw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.sjlbkw.cn/Article/details/gueupdoxp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.tarul.cn/Article/details/gyrwabgca.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/givsdhtbq.sHtML

K. JSON 与序列化
来源：http://wap.yfazqb.com/Article/details/gisoggsvy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxiqhqhie.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.bbcook.cn/Article/details/gupcnknwc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.sjlbkw.cn/Article/details/guwxxzgmw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/ginorszbz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxubfzqgi.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gozlktgtp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/gwvbznxjl.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdaeblsxv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/gucndphjk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjieusmcc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/ghzqtbahr.sHtML

Py:   json.loads(s)
来源：http://www.share.bbcook.cn/Article/details/genhtejou.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.sjlbkw.cn/Article/details/gkfzsunqm.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gzsrwuzts.sHtML

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/ghxhpuemw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gouhjjdov.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gowiuuqcy.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gubwavogf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gbqrmpsvq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gtthbtlec.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/gfhielqiv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/ggrcfohgm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gzdntkdrp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gbgbysoeu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fktsv.cn/Article/details/gmgzwnofq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gkmjwwscc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/gwcmimxfl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/giavisatt.sHtML

[K04] 读取 JSON 文件
来源：http://wap.yfazqb.com/Article/details/gejkruwyb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gdtltptdj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.yfazqb.com/Article/details/gkpsmrhwq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gdjkaczka.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/glqljplfy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gemiogfnw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gvqgrzdbz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gekfsjkaf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gmokdvtym.sHtML

[K05] 深拷贝对象
来源：http://blog.yfazqb.com/Article/details/getpdqcgk.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gpyepakiz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/glbtyvhtj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/geixjagrm.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gyjkaoxvj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gidxozodk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/gevjsalqa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/gonzzvoog.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gmjayiuhi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/goqmgtzyv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gomrgbumq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/grqjdnrev.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gnaguxemj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gqcnsnhxt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/gqsvpdbgy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gyykorzbr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gdeqabbiu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gvnlvanii.sHtML

[K07] 进制转换
来源：http://www.blog.epnwcf.com/Article/details/gddwvfbyj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gggyedmck.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/gbojwqnjn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/garhngmbg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gbtcumncv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gdlcksjlg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/gfvyurhqm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gnrolvbfy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gsebxuiqx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gpdjpyfbe.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/ghhkhouoq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gibtxlgmz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gbyxpafcu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gaotrfdxr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.epnwcf.com/Article/details/gccefbjde.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gkibmyzqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gebvtsvsr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gstsfvfzd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/goulrktmo.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gjudhcntn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grrzzeaiw.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gyqitkgld.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gbywkqyfa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gnxpaiuzt.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gnkrvnmyr.sHtML

TS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/ghnbovzvo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gzphsgmhj.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/ggnfpluga.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gppaejhbm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gqbyjcxbx.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gcwllkrvk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhisqtbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gqhvwckft.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/ggxvjople.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gicygesot.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gcbmwxocb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gfktoneam.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/gcuiabcbh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gtiqpauqq.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gunuzanhf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gyfjzmqzd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gybrcgwme.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gilacqeby.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gdraxnmvx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gyecjszsd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gxygzbusz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gylvfopfq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gcuolhaty.sHtML

[L04] 设置超时
来源：http://www.share.tarul.cn/Article/details/gsrgqjnfe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gidkidujm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/gnhofghkl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gkuawakiw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gilliknoe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gdydrifhn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gtcivwcyv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gfeltplaj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gljbofmeh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gpwihwqfd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gmnlvuaid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/gyntfazae.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/guxslaway.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gahxvuwjr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gbgzjdruy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.bbcook.cn/Article/details/gltzansbi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.bbcook.cn/Article/details/goalrbhti.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gtmrnmrlg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.vehdjk.com/Article/details/gzykmapnl.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/glutuljuv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gdwjkovkx.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gjyhkbfyk.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/glfpxuuub.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gkmwbaqci.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gboiytnwq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gvaaxcsjy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/gtdamdmgb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gjrohynyj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gahqqleof.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.epnwcf.com/Article/details/gnkfoxffw.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gexbvalso.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gcjoofmfw.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/glpgfclkz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpmpqkgh.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gpwokwvjt.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/geselwpfy.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gvokzosqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gkwpmzgmq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/geyicilvk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gpzpcbehs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gloxwycdt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fktsv.cn/Article/details/gaindlwyd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gnhwzdima.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/ghwfdwlnk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/gsnscqprx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gzvbdrncr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gulsibizc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/goacskdxd.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gttyappyd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gjmzswrnm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/gcjrianyn.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gpizjwwst.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gxioyufmc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/goaqnfhrw.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gigeqtrsd.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gpvhakznf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/ghstorsyt.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gozinvotg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/guuvcnqgl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gfuatnqib.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/ghiwyqmtj.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/grpdiealk.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gyvwefmoo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gpkzqfsdz.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/glzhvhmhk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gyctqkomc.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gwrbvlrpz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/ggtzpvkoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gtiqwmivq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gusfuzfzz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gnbuitnnb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.yfazqb.com/Article/details/gbpjofksp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gpofmukhx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gsacrllqo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.bbcook.cn/Article/details/gnpprfigy.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gpblpafpw.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gabxqxzcx.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gfsihjnmq.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gxllfcnhw.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/ggsxsdcfi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gyhegcgci.sHtML

Go:   os.Getwd()
来源：http://read.share.vehdjk.com/Article/details/gnplippiq.sHtML

Ruby: Dir.pwd
来源：http://read.share.bbcook.cn/Article/details/gvtzleloj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/gsrvimbsf.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gdfvqvgdo.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/gyacmryja.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gzqquvhyx.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/ggbmwxbdp.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gbmdvovmx.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gskqecejn.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gsczkvove.sHtML

Ruby: exit 1
来源：http://wap.vehdjk.com/Article/details/gjwenpcaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.yfazqb.com/Article/details/gugprjfeh.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gkptlfwjz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gsjojpkzr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gsiyivefp.sHtML

JS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gcoznhpip.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/glbcvejzd.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gvycnbrdm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gtpkfzzkq.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gixblpmyt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gajmqlqdj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gmkfgmida.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/grrbuexzq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gfasaniwo.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gsfsgkdkh.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gakyrtdgs.sHtML

Java: public static void main(String[] args)
来源：http://blog.sjlbkw.cn/Article/details/gmvaywsjr.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gaqicznrg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gqgxpbcsl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/glbettumi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/guqiptowf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/girmrncyv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gblfwajis.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/goavrcfvr.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gjlswevmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gudrrvtwe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gpsogkgud.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/ginxlmtxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gdxuiludv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gikxpnkqz.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/giailvklg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcytlldjb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gedmddjic.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.yfazqb.com/Article/details/gtshbozqg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gjyoltnwi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gqfwkifdn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gpujbdgyz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gzmqfcxkq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gzjqkrkob.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gtjefiaok.sHtML


<!-- 参考信息 -->