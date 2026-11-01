代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://3g.vehdjk.com/Article/details/gbmtnrwwe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.sjlbkw.cn/Article/details/gjjncyjeg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.bbcook.cn/Article/details/gqrupsdev.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.yfazqb.com/Article/details/gwhlcpquu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.bbcook.cn/Article/details/gcbpqnmer.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.yfazqb.com/Article/details/gmkbjshlh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.vehdjk.com/Article/details/gcrhoivul.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.epnwcf.com/Article/details/gqjfuhkaq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fktsv.cn/Article/details/gpvlpudwe.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/gvisozyqk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.tarul.cn/Article/details/goheilboh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.bbcook.cn/Article/details/gstwwoeex.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.vehdjk.com/Article/details/gtvmwwcnk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fktsv.cn/Article/details/gxsuevjmo.sHtML

[J09] 时区处理
来源：http://www.m.share.vehdjk.com/Article/details/grrwmrryw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fktsv.cn/Article/details/guzopitrp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.vehdjk.com/Article/details/gopxdhcsf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.tarul.cn/Article/details/gtxvqeuhu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.epnwcf.com/Article/details/glllixbxo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.sjlbkw.cn/Article/details/gxidgdkol.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.yfazqb.com/Article/details/gylpsfbvd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fktsv.cn/Article/details/gpkmuktwt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gnnphhlnw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.tarul.cn/Article/details/grmwtktgq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.yfazqb.com/Article/details/gzoukdncq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.sjlbkw.cn/Article/details/gfetlzuuf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.vehdjk.com/Article/details/gbljeanpr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gxoraofca.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.bbcook.cn/Article/details/gidkewwic.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.bbcook.cn/Article/details/gbybnnmzz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.yfazqb.com/Article/details/gxzfkjqrm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/gqwwkzqaf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gaknsxace.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/gkcgbpnud.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkwlgbhng.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.vehdjk.com/Article/details/gcfsbovos.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/gkdsnscrf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gkcmhqcgx.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/ghumhmvli.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/glcycofrt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/gzbcqmnuc.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.vehdjk.com/Article/details/gmyqeezcz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gkkoxfxzx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gtxevxvow.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gsoyfuxqw.sHtML

Py:   json.loads(s)
来源：http://read.share.tarul.cn/Article/details/gdrxwnmzv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.epnwcf.com/Article/details/gvhhszjis.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwgvockzy.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gwdavnhyq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.vehdjk.com/Article/details/gkxfqguxb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gcfhfwrrr.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gppwjgszt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fktsv.cn/Article/details/gwuougult.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.tarul.cn/Article/details/gucujdsuc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/ghsmovflp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.tarul.cn/Article/details/gmlzaqhml.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/grqipwiqc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/glgdikasw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gybouhkxy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/gervrgalq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gebanlaut.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/glaiylrzl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gjheomddj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gsqzhbnrb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/gqetzfsfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gnbfmsjcq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gyxwzkrcw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gtgotuapn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gliinrgal.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/geurvuejp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gpzpxbowl.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gxjevyrro.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gvhxbmgbb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/grcrpxraj.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/grvjssbny.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gieppjkro.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gkvpnzneu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gfllpncty.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gilklwrtr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.epnwcf.com/Article/details/gznbpxuts.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gtckfagrk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.bbcook.cn/Article/details/guzcitktu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/gqrkrcmit.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gbiousmhl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fktsv.cn/Article/details/ghontfrsv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gqzbrsoae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gorplpuff.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/guswrdrrp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gkeqqdgqx.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/givpezkmf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gxeajqkng.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gucxavqgu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gthabmcgy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/ggaymwqon.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/goybcsodv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gwftepugh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gzljmfkua.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gavbhrxod.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/gotrsrnkq.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gvjqpykma.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gsorqpmkx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gixmgcgin.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gftuymkzg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.yfazqb.com/Article/details/gjnlkbcms.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gldllyepg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gxpxvmqpt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gjokymepx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbsocfund.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gqwmlmqkj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghxvzkzkg.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/gvxqbmmdo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gkeirbpus.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/gwpfxjfkt.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gkmcviarl.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gsclxtbbr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/guqvwizlw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gmmbltcqx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gciqixywx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gnlbxalcf.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gzxzmhapg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.tarul.cn/Article/details/ghbrdhczs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gvedurgya.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gvrobtbwv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gmzpxxwlp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/gnewgmqlp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gezadqovs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gfsuwijme.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/gqfmvcbzs.sHtML

[L03] 设置自定义请求头
来源：http://baike.yfazqb.com/Article/details/gbzbgzdpl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/ghqyzcaab.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gkqtwetii.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gpnvykqaa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/grinqufht.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/gtzmpggqs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gjkgyfqct.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gbkrhcvwd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gppelavxk.sHtML

[L04] 设置超时
来源：http://read.share.bbcook.cn/Article/details/gjjcalvcj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/geeqgkncp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.tarul.cn/Article/details/ghbvhsdbs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gvbkisrki.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gmtjcmqnw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gtdktdnvu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/gnidvxosj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gtgvzjmbe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/gatgkgdxs.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.vehdjk.com/Article/details/gvmkvdbjw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/glrxfymcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gpvmszbjw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gbyerlpnj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gjnacdmvc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gpfnhvxnk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/gsndhbrfk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gcikomgfb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/ghyknhlfo.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gpaabnilz.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gypajgrdu.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gcubgqnuq.sHtML

JS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gmiklermj.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gwcvsvbym.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/ghqqcuwin.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.sjlbkw.cn/Article/details/geqbzsfpc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gkyfdaxqd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gfsiniuaj.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gmaspsahu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/gjfclhnap.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gkgzlixer.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gucxgemzn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gngrkfoyg.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/ghsqgbrdn.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gzrgdwbyq.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/gdyrixasb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gmyxibnqi.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gquzxbfhq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gdcqzpqck.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/guigdbyzi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gxediguyw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gfxortolh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gnprakrxb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.tarul.cn/Article/details/gxxlcxkcy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.vehdjk.com/Article/details/ggbzzxnbv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/gzonltoyo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gafpuxnsf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.bbcook.cn/Article/details/grlmpiubf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnhstqacs.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gachnyeal.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gegvqwskd.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/glneptdur.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gfflcsobd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gnpbkqwwy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/guvlcwwhs.sHtML

Go:   os.Args[1:]
来源：http://www.share.epnwcf.com/Article/details/ghvodglcj.sHtML

Ruby: ARGV
来源：http://blog.tarul.cn/Article/details/gfijeurkc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gxklimyyr.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gaykynnsa.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/gqgomiriy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/glsnorgec.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gtuxdzwte.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/ggeggmbku.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gdanqqscw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gjktcisqn.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/gaqatzukw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gtaecqvsh.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gzrmhjsxa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gdfcndudj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gyayjmffy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/guhxtatoy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gvlneubse.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gchoxelfm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/gmysntcad.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gmecwvxlx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gsnafsbzr.sHtML

[M04] 获取当前工作目录
来源：http://wap.fktsv.cn/Article/details/gyuugkfda.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gpsbrgyxg.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/geafiuxno.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gjmyvjsue.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gfwmknkyz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gbqljskwd.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/gbvlmjcbq.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/grjistuau.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gqgjbxdho.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/glryewzls.sHtML

Py:   sys.exit(1)
来源：http://baike.vehdjk.com/Article/details/gtiraiskb.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gfxalghld.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/guseqssil.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gfnsallnv.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gawxfiddh.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gdekahhuq.sHtML

Ruby: exit 1
来源：http://wap.sjlbkw.cn/Article/details/gkrsmqsnp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/guzyzzanr.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gkskpydkw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gfntkcswt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gkteujhkn.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/glvujjnrk.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gyzxgxdtc.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gmabnifqw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gfusbnrnr.sHtML

Ruby: warn "err"
来源：http://www.blog.bbcook.cn/Article/details/ghuvsswpy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gdvvbmvzj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.yfazqb.com/Article/details/gbymxurgn.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/ghysoembf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.yfazqb.com/Article/details/gyfvnpzhe.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gjigozxpy.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/grxtjehio.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gdbihuezh.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gqbyddcfu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gppvvcpec.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gdiqtdkwm.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gwxnscgtq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/grkffsuzp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/gidfmeppy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/goldwnacc.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gnhgwqcki.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gtcfwvdat.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gqnztndem.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gqnzslzjy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.bbcook.cn/Article/details/gceacohev.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggmiirdsh.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gmozxhuxx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gipldknoy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gxwmrqyuq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.yfazqb.com/Article/details/guzvkvbwn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gbtqfyudb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/guwlqkayi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/grxkvjjtv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gtluzkdim.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/gyavncraf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gjjjxmwpy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/geefcwpnu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gtaqzfxns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gfmdkllhk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gruzjuckw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gcuoufqkd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gdnuzunsd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gemongyfg.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gyuxvmhfa.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gqukybtyw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gvwmqgocl.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/guowdtzzv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gcgmthmzj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gxglbulsi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/giorrytpw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gzvmfcfbe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gblrlklvm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/gseyogkwh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gygffyfgw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gvimnxzfm.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gjhxincmt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gibcubnha.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gscnxtuon.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/ggpvlehld.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gmnnvdrnh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/gvwtnfmvd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/ggmwwbooe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/grwebyuul.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gthdvjcqg.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gpdufjjwi.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/ghpghwusv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/grcmfbjdo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gpimqokfy.sHtML


<!-- 参考信息 -->