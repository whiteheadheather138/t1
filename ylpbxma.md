代发 wailian999

[J07] 比较两个日期
来源：http://3g.fktsv.cn/Article/details/gyjxcppns.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.vehdjk.com/Article/details/geaavqcru.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.vehdjk.com/Article/details/geirjwiud.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.vehdjk.com/Article/details/gvwexgbsg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.epnwcf.com/Article/details/gfanivsse.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.yfazqb.com/Article/details/grdwzrjjv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.yfazqb.com/Article/details/gaitdsmuq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fktsv.cn/Article/details/gaibhqicl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.epnwcf.com/Article/details/gappfgdye.sHtML

[J08] 提取年月日与星期
来源：http://blog.fktsv.cn/Article/details/gjgytdyqd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gbhzxrart.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.yfazqb.com/Article/details/gacnrdrdh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.vehdjk.com/Article/details/gqvfcisko.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.yfazqb.com/Article/details/gxqvrhiuz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.yfazqb.com/Article/details/grkgpqurr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.bbcook.cn/Article/details/ghjgpxdzo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.sjlbkw.cn/Article/details/gwfdprdmy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.sjlbkw.cn/Article/details/gdgyltunb.sHtML

[J09] 时区处理
来源：http://www.share.fktsv.cn/Article/details/grhkmtgki.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.epnwcf.com/Article/details/gzjlkdbak.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.tarul.cn/Article/details/gkqcvhxqv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.tarul.cn/Article/details/guajgngxl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.epnwcf.com/Article/details/gqcpazfrg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.bbcook.cn/Article/details/gpjoyokec.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.bbcook.cn/Article/details/gvgscuoyp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gbjzyxizi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.vehdjk.com/Article/details/ggcphomyw.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.yfazqb.com/Article/details/gkfotnskl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.tarul.cn/Article/details/ghwjsaxjz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.tarul.cn/Article/details/ghwrrjumw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.epnwcf.com/Article/details/gsnravncv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.tarul.cn/Article/details/gscnvqkbm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.yfazqb.com/Article/details/guedesxxg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/gpsphubxu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.bbcook.cn/Article/details/gygcknqdv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.epnwcf.com/Article/details/gncgbpzju.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcdmfgeyc.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gtgzgqgup.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkbwzinwv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.vehdjk.com/Article/details/glelwzszx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gcpvolnqw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gcvlimlhc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gphpjohdr.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gycfumxfe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/gdclvdave.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gbdpcgzjt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/gifewecgv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gvmdjlzza.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gnfxfttqe.sHtML

Py:   json.loads(s)
来源：http://m.share.fktsv.cn/Article/details/gekzrisel.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gjcmelbde.sHtML

JS:   JSON.parse(s)
来源：http://m.share.bbcook.cn/Article/details/gvyzsrqvj.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gczsbsape.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/godqkmnph.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gkiotmmym.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/ggknwtdyc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gtgmyogtt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.bbcook.cn/Article/details/giowjligp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fktsv.cn/Article/details/gorfbvnun.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/ghuqmaifj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/glattktui.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gooooplul.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.bbcook.cn/Article/details/gtmvijijf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/gzcoaudtf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/glavqipag.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gmnmawipo.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gtltzmuwx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gtyogvthn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/gqaecmngr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gtlfycypk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/glcqbvrhl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gubjtotcw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gjjixfyqw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gjmysykib.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gtctoorpi.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/grplgnnsa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/grrnzpeip.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gemdmabhs.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gqzswdvmz.sHtML

TS:   structuredClone(obj)
来源：http://3g.tarul.cn/Article/details/giadakjab.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.epnwcf.com/Article/details/gyfpgcfjx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.sjlbkw.cn/Article/details/gzrgruncw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/ghpmpacdu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gvjjrskit.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gtchxjyer.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gfpmcwxbj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gufjnfjcr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/guwkbfcsc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/gznpzsmvw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gqfkjbihz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gxprhdypz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gifrxzwlr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gbacpmvgo.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gmomgssqf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/grhswuags.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.yfazqb.com/Article/details/gipfswsyy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gsexipokn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gfrgoqgzh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gahjtanrp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/gjmgshnkb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.sjlbkw.cn/Article/details/gqmfobbtt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gcobotyee.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gtcmswmhj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.tarul.cn/Article/details/grqkwbhxi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gljlthsqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gvnsxvlpk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gjovpqllm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gkdailgaf.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gixtgiwhm.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gyjckhncd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gkwxcydmp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjfoodvpq.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/grdqievoz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqbykkukc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.bbcook.cn/Article/details/gkumhmfug.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gqcveiuzw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gcvflomju.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gzjzavlwg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gijaazybs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gaauvtybf.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/garxmoabt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gmfljhdmt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gamexwlnp.sHtML

[L02] 发送 POST JSON
来源：http://baike.tarul.cn/Article/details/gtkkitngd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gwqzcnypl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsqixrto.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gsptqwbqv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gegiftzok.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gxzafqisr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/gjpvxlzwx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/ggawtxmfi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gzoagybde.sHtML

[L03] 设置自定义请求头
来源：http://m.share.epnwcf.com/Article/details/gjzuasqea.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gxbyivfja.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.epnwcf.com/Article/details/gjutoljum.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/groxgspfa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.bbcook.cn/Article/details/grxigikee.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/glubmltci.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gijuiwthi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gwiqjtjyb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/getvfhdvd.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gxsnhxjao.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/guxgsuzbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.yfazqb.com/Article/details/gjwvrirvc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gwkfguwjx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gixdahpit.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/gafadnoxv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/giznpqylx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.yfazqb.com/Article/details/ghmanxwar.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/gdlevzsvt.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gmytgbaxo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fktsv.cn/Article/details/giseouwzw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gjeiomsoi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gmunbipwr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gaearkrlj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gvldmelyn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gfumfheqj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gfmjagpxl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gxzowchat.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gzjyzdyhv.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gfnjkuoqz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gynxfxujo.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gsjyedlxp.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gvenptjgu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gumadkxft.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.tarul.cn/Article/details/gexjfnwyc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/guvpmxkuc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/gcqwysemp.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gonmgieqn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gjnaeuhtm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/glbavlllx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gmxinbcwq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gnedrgobq.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gyaxzlveq.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/ggsnriiud.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gwbqhvlbl.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gtqcjhnnq.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gxsnfmujo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gmuuoyvxu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gltffwykm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gzcqhlhgr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/ggyygppve.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gwlclbxvt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/goauuzgjt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/gctglohmn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/gbkwcmxuj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goliqmewh.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gzkhcvuwn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grntapwgw.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gheomqzgo.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gezqpfhxu.sHtML

PHP:  $argv;  $argc;
来源：http://wap.yfazqb.com/Article/details/guvqtwlif.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gaflcabno.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/guzxdgevn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gjbacunql.sHtML

Go:   os.Args[1:]
来源：http://www.share.epnwcf.com/Article/details/ggtystwtw.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/ghqdhmbiv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gsachjtov.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gooyzwebv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gwwlmszql.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gystiqxmx.sHtML

JS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/grkcfhmee.sHtML

TS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/gkwcypsex.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gqnriyawr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gjkufmyhe.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gxlwfcqxp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gavuakekw.sHtML

[M03] 执行外部命令
来源：http://mobile.bbcook.cn/Article/details/goqjqzyih.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gmrvotisq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gwrzblazq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gcarkydjn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gmffiuscz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.sjlbkw.cn/Article/details/grhfhakuw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gqkeepkwo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gggdsxcip.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gxnbhervy.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gyyzecsfp.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/ggujpqmgc.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/goegxcvel.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gouvtaplm.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gqoreovou.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.tarul.cn/Article/details/gwzjpmgxe.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gxenltpsy.sHtML

Ruby: Dir.pwd
来源：http://wap.sjlbkw.cn/Article/details/geqhlandt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/gxbahlkei.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/grqshpdvf.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/ggbsclcrv.sHtML

PHP:  exit(1);
来源：http://blog.fktsv.cn/Article/details/gcrockzwy.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/glwwrtibu.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gdpbmjtze.sHtML

Java: System.exit(1)
来源：http://blog.epnwcf.com/Article/details/gnvmckiuv.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/glnibimvu.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gjipiddkr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gftqedyhp.sHtML

[M06] 向标准错误输出
来源：http://wap.yfazqb.com/Article/details/gwckpauiw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gesqomzix.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gohsciegw.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gddjvvfyi.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gvbrakgdq.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/gwrbdjibv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/gjczkmyye.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/gozhgpsln.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gvcewajqj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/glpoidnbz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gmzwhwrmh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gvfyeqxpf.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gjnsffqms.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gselwoguf.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gwzpyjyee.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gbrzlvkty.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/geokqkvpl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/grifdgfzn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gciddnqfs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gvlcriefq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.epnwcf.com/Article/details/gkpjyzahn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gjaxytjku.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gkzyqvgmk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/ghjzwoeas.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gumbzuiek.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gyxbjpspr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/giexevyow.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gucuubvof.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqxfzlzx.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geadqvwag.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gxbbmwomz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/glgukoyaf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gxpxcbdof.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gknoabqkp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/ginqzgtad.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gejeyfyiy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gaupdrbdf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gsnxvyrdi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gasxkrpad.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gdrpolkyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/grceqvewh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gxrxqjuwa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gsiqhdbxz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gvpfemxtl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/glwtvdihm.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gbqbqwoki.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gcayavkmy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/grdtfomih.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/geiulizww.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/gxizyvhfy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.yfazqb.com/Article/details/gzormbjvk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gbzjoueiv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gsehojplp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gfpgvqvyr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gmlcewisf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/glwzkvvcv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/grcsuridh.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/gtbixtxov.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gsvsxissd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/grzhkuulr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/ggnhfhazs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gazlohbde.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gatqtkclz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/gbatueqdw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gwxcxmzja.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gbzxqvyfb.sHtML


<!-- 参考信息 -->