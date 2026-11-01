代发 wailian999

Py:   (end - start).total_seconds()
来源：http://wap.tarul.cn/Article/details/gkedpowgh.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.sjlbkw.cn/Article/details/gubmkqrfa.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.sjlbkw.cn/Article/details/gggjuekga.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvtwtyaf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.epnwcf.com/Article/details/gopckkwsm.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.bbcook.cn/Article/details/gnsoeqjio.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fktsv.cn/Article/details/gbsqrrdlf.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fktsv.cn/Article/details/grwafxwfk.sHtML

[J07] 比较两个日期
来源：http://blog.yfazqb.com/Article/details/gachvyyqe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gcwharyva.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.vehdjk.com/Article/details/giowhjrsy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.bbcook.cn/Article/details/goolsgvjf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fktsv.cn/Article/details/gdwizftwu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.tarul.cn/Article/details/gqyvrknee.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.sjlbkw.cn/Article/details/gxdmywbrn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.sjlbkw.cn/Article/details/genvrfvna.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.yfazqb.com/Article/details/gjqnvntah.sHtML

[J08] 提取年月日与星期
来源：http://baike.fktsv.cn/Article/details/gmhgjbdpn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.sjlbkw.cn/Article/details/gjptlngep.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.yfazqb.com/Article/details/gtmoejrxw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.tarul.cn/Article/details/gvxqgjuwv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.epnwcf.com/Article/details/gegqfffrw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.sjlbkw.cn/Article/details/ghqnybbyo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fktsv.cn/Article/details/gtymoczdz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.sjlbkw.cn/Article/details/gmukymgkp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.vehdjk.com/Article/details/gvhiqcont.sHtML

[J09] 时区处理
来源：http://read.share.epnwcf.com/Article/details/gfxieerbd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/gpyetmzmt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.bbcook.cn/Article/details/gjaeiwrst.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.sjlbkw.cn/Article/details/gpciquugn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.yfazqb.com/Article/details/gwxesaboz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.epnwcf.com/Article/details/gexpvruhs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.vehdjk.com/Article/details/gmrsmbimv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/gabtfbmje.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.tarul.cn/Article/details/godpaypxz.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.tarul.cn/Article/details/gyouscdts.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.sjlbkw.cn/Article/details/grsrsxdwn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.vehdjk.com/Article/details/gfghwjldk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.tarul.cn/Article/details/gejhvqxdw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gbszjbbfg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fktsv.cn/Article/details/gqjsgotdz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.epnwcf.com/Article/details/gachpllfj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gxdarwoow.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.sjlbkw.cn/Article/details/gfvigirgi.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbigicano.sHtML

K. JSON 与序列化
来源：http://m.share.epnwcf.com/Article/details/grfzcodyb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmwstvedz.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/gebiswyvo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/geinxdhhy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gnmamyrim.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gkyeqcbmc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gtgcwieax.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/glqmaslsj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.yfazqb.com/Article/details/gzisvogyw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.epnwcf.com/Article/details/gvoiylxyt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.tarul.cn/Article/details/gwchggndg.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fktsv.cn/Article/details/gzpbvmcfu.sHtML

Py:   json.loads(s)
来源：http://3g.yfazqb.com/Article/details/gzywrmxny.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/gvlokczwk.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gflrcyqyz.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/gzoorulvz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.bbcook.cn/Article/details/gmnicgiwz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gknauxdmn.sHtML

Ruby: JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gtasljmjn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.vehdjk.com/Article/details/grhhpcemp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gkazxhniy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gjmxwfqmy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gmhnjfhuz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gsnzxsnug.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gwrwnffdp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.epnwcf.com/Article/details/gjthxqwgb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gnbnnnysd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gsoeoskyq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gtsryijsp.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gvfduegeg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.vehdjk.com/Article/details/gjilsmmav.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.epnwcf.com/Article/details/gcsuzgxwm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gsarjvdnx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gbbidowai.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gjwnrhule.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.vehdjk.com/Article/details/gizdxhoxy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gwqnmeilf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/glyoovnit.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gnzhynuqn.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.epnwcf.com/Article/details/ghabxxnzu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.tarul.cn/Article/details/gadfygbxn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gqsiqnuef.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gyvgahtfs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/ggnkwhwva.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gaeqkuncu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.tarul.cn/Article/details/gkwmokojg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gfxoqudvz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gjnkuatfp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/geuqhyatl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gnktdztxm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gjexeszoh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gkpgggpzz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gtmgiqdbc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/ghctwflix.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/grbewfkgs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/ggtqzopmz.sHtML

[K07] 进制转换
来源：http://read.share.epnwcf.com/Article/details/gkprwewpj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/grvdpxviz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.tarul.cn/Article/details/gtretkrtx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gqmcmossc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gygibjzdz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gqxxurvvy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gmfsmxato.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/gbugerlcr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gkxpkyhsm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gxoeorahm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gkvdztlsk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gkpxmtxmu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gzxfiyndl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gyrpphbej.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gysiwzpol.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gvpreyjpv.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/geglqfcoj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/gdmrjtlfz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxamabhkb.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/girrhtcfh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glacekwvj.sHtML

[L01] 发送 GET 请求
来源：http://baike.sjlbkw.cn/Article/details/gebpskzbh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gwsqtewmt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gjnzfzttn.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/ggprzovia.sHtML

TS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gvrzpnifh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/gzgaiqyba.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gtxdaqpcc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/glpthyczz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/goyoqkysf.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/glnhfpbtv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhoqfset.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gmqhpuuuk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gcoclcbjk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gpfojhybg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/ganswcooi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/genrhubcv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/ghawferll.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gfrduslnn.sHtML

[L03] 设置自定义请求头
来源：http://mobile.epnwcf.com/Article/details/gxxxonxhk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/gilvevvvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.bbcook.cn/Article/details/gaporsygq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gkziuhikn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gxtxhpojb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gkmaamrca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gypedbsgm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gumwxtnez.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gqvdktfhp.sHtML

[L04] 设置超时
来源：http://wap.fktsv.cn/Article/details/glzgnfcdm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/geygaajys.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gtizpegfq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gmggerfwz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gxswolnvu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gdhywsflf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gcjiomqtv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/ghjwbbmka.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.yfazqb.com/Article/details/gbybwbopi.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/ggqwpwfmz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/gdzicuunf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gtrbpxhak.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gsrigltrx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gczndqlfc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gjnshddaz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/glpethcuq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gpilnlosv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gwvtplrgj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gwhkkhzjf.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gpabirncg.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.bbcook.cn/Article/details/gfiiibbim.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gibridbhf.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gqtbcyzda.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.epnwcf.com/Article/details/ggckzkurl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gzxribrwa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/grtikzprj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gmfykzxxv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gmsuuyuhm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/gchshyycy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gxolbtkmh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gukzlrtrs.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/giwpcdwiy.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gfejfzrol.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gvgkredwm.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gsgqfunpj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/goixalprz.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/guhslvsdy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gvdhmdbpv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gucjkvtcm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gnssrqeax.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gkzwmnwcs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/ggtngcceh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/glbvwflmr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/ggwcfspub.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gauwfntyn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbxzvuxqy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gcyijucaq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gklrntrwn.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/gnqibnzwy.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gzxpgrpvi.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.yfazqb.com/Article/details/gorhlelmh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gecptuqqr.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gggsprhuc.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gqvpcrpkq.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghllujtkp.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gdcjpgexh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/geuxwdjqb.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gpjyhuzuu.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gvyibdxxa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gbeueuwvi.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/ghvuycypd.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gmkaiamid.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gbqzeoqpl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gatyauysa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gkbzbpscl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gflalcoxn.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/ghytuhogo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gbckqqspy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/gujtdsmtc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gordydtal.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gubvwxtpf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gdjfjrmsm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gpzntzuuy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gmcqbnrvr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gqamyssef.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gtdtpxcxi.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gsimvwzxt.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gwzfwzhlv.sHtML

JS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gvkiefwhk.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gyuvlfdmi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gwshxwesv.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gtebytwff.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gkizwcoko.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.yfazqb.com/Article/details/gfumiqgue.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gvafvjjea.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/grtybydcz.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/goltyiqsd.sHtML

JS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtheuskvg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gyvikyttp.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gdsrdwcnf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gzsahnaxw.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/gphjfeosd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gjshentjm.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/guzycoqjz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gpfvqmeyb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gzxmuldhy.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gwnqzpjae.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gkqydqumm.sHtML

Java: System.err.println("err")
来源：http://www.share.tarul.cn/Article/details/gsriuuhsp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/gpxvicloh.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gzhnmadrr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gfnbuqgio.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gqorfxyfx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gfwqagtok.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gxuayekzt.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/ghdtqxway.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gdsjpurjd.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gazdkkdug.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/grsygoqbk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.bbcook.cn/Article/details/gcmketwsf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gtibufhap.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/grrbkhqbi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/guyopwokc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gviqnqojn.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gmzkrosop.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gkshqnosy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gezxnpvpn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gzhawlfhb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gaouwtjyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gyinddzys.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gduazlsnz.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gbdocpmla.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbpseprgr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/gacrvqqyj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gbhqgbbif.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gerdgdrvz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gcguworsk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gforamfmc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/ghuwxjqfg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/glmjbcfoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gpqbngtue.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gctzdyrdw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gfkviezbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gorhzcika.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/ggcziqpkf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gyqgxhgtq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gbitdkgsj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gpyqnqywr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gqnxoceeq.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gvfpyijaq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/geikoczbt.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/ggnxrlyfn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/ghhgwesvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/gxamabbdq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/griyadcax.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/ghxroodcu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtaekajk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gdqoboiuq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gvakctjnu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gkouwbtpo.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gntrmhgcs.sHtML


<!-- 参考信息 -->