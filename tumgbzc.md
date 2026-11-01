代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://3g.sjlbkw.cn/Article/details/gkxharmop.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.sjlbkw.cn/Article/details/gjebnxbll.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.sjlbkw.cn/Article/details/ghspivtrq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.tarul.cn/Article/details/gsyrzoqkg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.tarul.cn/Article/details/gkielddbo.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnnacgfc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gqdafklrd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.tarul.cn/Article/details/gmobnbecs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.bbcook.cn/Article/details/gknbfwjxs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.bbcook.cn/Article/details/gbegykcvf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.epnwcf.com/Article/details/gldjpmnmn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.sjlbkw.cn/Article/details/gdgiqdlcl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.tarul.cn/Article/details/gpshybdwi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.yfazqb.com/Article/details/ggplgekmr.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/gxgtolxop.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gjaikynhv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.tarul.cn/Article/details/gkqgdroko.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fktsv.cn/Article/details/grwkbqcib.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.vehdjk.com/Article/details/gdylarkes.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.yfazqb.com/Article/details/gtexzupzs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.tarul.cn/Article/details/gzdiiikcn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.epnwcf.com/Article/details/gygztxcua.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.epnwcf.com/Article/details/gmfxuwgse.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.sjlbkw.cn/Article/details/gxvlyxzif.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fktsv.cn/Article/details/gphkakozt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.tarul.cn/Article/details/gqunbjyam.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gdismjxyi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.tarul.cn/Article/details/gguzolhpb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.yfazqb.com/Article/details/gxvngrcqj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.sjlbkw.cn/Article/details/grnedkyiy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.tarul.cn/Article/details/gwokaqksw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gscmhfyvc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfcpapvrp.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/gvmcmpnjl.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gibexsuoh.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gsqucxgjj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gosfxaoie.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gfnvetpce.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gibspxxsv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwrnzlgkh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.bbcook.cn/Article/details/gxxnbnkym.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/gqyjckyzz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.vehdjk.com/Article/details/gzddffvvr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/grlujxyso.sHtML

[K02] JSON 字符串转对象
来源：http://blog.epnwcf.com/Article/details/gpyuaauzu.sHtML

Py:   json.loads(s)
来源：http://m.share.vehdjk.com/Article/details/gknhehpwj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/gurzdavom.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gqxkebrjc.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/ggpyogrig.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gajfjmyyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gosbefimd.sHtML

Ruby: JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gjopmjxoh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fktsv.cn/Article/details/gkyooaocs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.tarul.cn/Article/details/gzqmxkxfb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.epnwcf.com/Article/details/gmcbhpfbc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.bbcook.cn/Article/details/gnmkpejdo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/ggkoodzxl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gsufjiujh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gmcjfvozb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.vehdjk.com/Article/details/gaocmxseg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/gfcifcmvg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gydsykpbg.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/ghdkisobs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gxbvbghtm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gowtocjfi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/glmyylxid.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gdyavuest.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gawybcacp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gjaezygny.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/glnmozpqg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gcxionatq.sHtML

[K05] 深拷贝对象
来源：http://wap.epnwcf.com/Article/details/gpmvelddy.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.bbcook.cn/Article/details/grihpzowa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gomaepafu.sHtML

JS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gbxtzlkpl.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gnytgjvdt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gtvzarjey.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gwcfqjmdd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.sjlbkw.cn/Article/details/gkmuqwxqy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.epnwcf.com/Article/details/gftkgrhia.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gxglzjplt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gyvvgkirs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/gjykdbvye.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gpvvovslt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/guugnguyo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gksqmuvfh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/ghzqhybxv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gnheqoaus.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gjgjffpbd.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gzdouaxqd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.bbcook.cn/Article/details/ghjpxswyq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.bbcook.cn/Article/details/gufmvxfck.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gpxvvksuh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gnhemxhwh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gdoyyzyyb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.yfazqb.com/Article/details/gawgiqduy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/gmimrcqrq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/geuhkqkkp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/ggrhtqlto.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gdlkgegsz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.sjlbkw.cn/Article/details/gzeicaaav.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gwsiewgjz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gflkyfgrm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.bbcook.cn/Article/details/gfilnbder.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gnqcguidc.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gmlrlgpyf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/glcnwldxt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/giburougb.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gcpskqyef.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gopvekwgh.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.vehdjk.com/Article/details/gixbflrbd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gqmiduwaa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/glqfzsedj.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqguxkxsr.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gelwmieyg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.tarul.cn/Article/details/gutksglkn.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gmruqyven.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/givywpwcx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/grttvcrwl.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/goupvweor.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gjomtghgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/giljbsqap.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gzaydvdkw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gvwhoewcr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/ggebipzph.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.sjlbkw.cn/Article/details/gqqyeaqlh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gztwioppm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gecvhaemx.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gbzuipoxt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gcgqlivpn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gvjodrytc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gmqhqoehf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/grisevdip.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfepfpuw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gxfenufdq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/glpzofqxi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gpglorpgp.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gvruykecm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gzvhnrsrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gtjomqkzi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/grahjdvws.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gkmwtwfks.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gkxkppuyn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.tarul.cn/Article/details/guyhzotcm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gylrfczik.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gdqsmswsr.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/giwwbzcgv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gtztmjbgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/ggdewoxcf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gqdkfjmjt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gpugfypoo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/glvsqmsqi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gcdoewqxg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fktsv.cn/Article/details/glozkhtfc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gtcedyoov.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/grljaveee.sHtML

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gqkdfmjpy.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/grkzszkse.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gzqnmooju.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gsnfibqia.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gdibnwdmv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/glhcbscgd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.epnwcf.com/Article/details/grcadbdtj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/ggcxackto.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/glosjomvu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gnikomzne.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gakfjspnh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gjwogluaf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/ggqtubyds.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/grkdjpgjp.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gclzpnmhq.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gqbuwcklf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gjdvzcpkv.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fktsv.cn/Article/details/gexpbzkwh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gwxoxjmme.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/guooqsopg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gzlyvuhuz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/glcpiorxr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gvvjaftvx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gybrbpvrq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gnmlskxpq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/guafimkda.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/guvaomnby.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gvsbalnex.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grgtywrfp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmluqezk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gqfomhmvn.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gtnztfnco.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gyemhjqlt.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gqyiowhxh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gnziidoey.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/ghkegdehr.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gaxktygpe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.epnwcf.com/Article/details/gjvwpmrdv.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/grdmunzyq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gnbcpofsg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gxodzgclx.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gpjvchqff.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gwjnoypcl.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gmpcdqtbm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/ghqucavbg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gdsalynrp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gdhhisiot.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/grsmiredw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gmmehssov.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/grrgjkykl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gbfspylqt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gynshgvru.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/gksrelyoi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gkmxsmovm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.vehdjk.com/Article/details/gfsxcqvdv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gvlinekgn.sHtML

[M04] 获取当前工作目录
来源：http://baike.bbcook.cn/Article/details/gwiqpufkq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/gtmootutd.sHtML

PHP:  getcwd();
来源：http://www.blog.yfazqb.com/Article/details/giocbpmok.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gvvnqtybj.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gomfvntqo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gvunkblok.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gnaytzjpm.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/guybeeukp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/ggrafopkm.sHtML

[M05] 设置退出码
来源：http://3g.fktsv.cn/Article/details/gdnkufonv.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gnogqooci.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gevticqks.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gaaqwophx.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/garektheb.sHtML

Java: System.exit(1)
来源：http://blog.fktsv.cn/Article/details/gpsejlbkq.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/ggiixsnko.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gtxoyptsa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/godmfuvsr.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gzfgkvjvt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gbxretqvu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gehalqyyc.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gjsrcbasr.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gvpeofezi.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gscottknq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/gzgvfdnbb.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gnfkqseqy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/ghhzsxtaz.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/glgikdetm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gxmjmozsk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gyhytapxd.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gbdebrngt.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gugppojrj.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gmiegifhk.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gvdbszinf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/grhcwceqr.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gsafpnaso.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/ghqgkxcnq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gqaastvym.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gssqykwni.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gfuzitzgn.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gawbmocic.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gbslqkvcy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/gvquebfmk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gdqttdmih.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gvvanbdzr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxwemmeax.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gugqezwkj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghtvyjuah.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gyqnzthka.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gohdnpytb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gowvgrlcr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gtjmgeuck.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gtpscyvcv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gtexjirik.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/govoyixrc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gpudatxvz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gdqljkfbe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/ggasbydzh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gflqtiqeg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gyjflpgat.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gpxtrdjnr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gcxvfklzd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gpfhncduc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gyrluqkzs.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/glmdkojiw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gorsnwsxe.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.epnwcf.com/Article/details/guxqdycat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gkvbmrxln.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gwmwwyyiw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gvihaknmt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gtbhcqwnk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/ghzpyeifb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gyhttrhos.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gunkfsuvd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gflbsvmlg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gekdwuwkl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gukboxvff.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gppmtibdj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/giygwvkcu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gxdvngbdi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gerqhwerr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.bbcook.cn/Article/details/ghvomrddy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gxgkfrnjv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmklqwcem.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gzatrssyu.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/ghlopqjqy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/ghnuggebg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/geaqrrytf.sHtML


<!-- 参考信息 -->