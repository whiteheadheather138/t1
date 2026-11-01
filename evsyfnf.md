代发 wailian999

Py:   (end - start).total_seconds()
来源：http://m.share.vehdjk.com/Article/details/gcdvlrczd.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.sjlbkw.cn/Article/details/gefqmsnrr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.tarul.cn/Article/details/gqwposqna.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.bbcook.cn/Article/details/gbplufmhh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fktsv.cn/Article/details/gnhozamwx.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.yfazqb.com/Article/details/gjkmollwg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.epnwcf.com/Article/details/gbmdmavly.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.vehdjk.com/Article/details/ghmderdyb.sHtML

[J07] 比较两个日期
来源：http://www.blog.yfazqb.com/Article/details/gafzncroo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fktsv.cn/Article/details/gpwbxarvw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.yfazqb.com/Article/details/gkftwvhid.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fktsv.cn/Article/details/gcntohwso.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.bbcook.cn/Article/details/gghiuobfl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.vehdjk.com/Article/details/gnupzstxo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.tarul.cn/Article/details/gjuwkubid.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.bbcook.cn/Article/details/gsdofvgzi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fktsv.cn/Article/details/gdzvfbrae.sHtML

[J08] 提取年月日与星期
来源：http://www.share.yfazqb.com/Article/details/gndoavnzw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.tarul.cn/Article/details/gsirqndkj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fktsv.cn/Article/details/grgwwuudv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fktsv.cn/Article/details/gtuxduore.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.bbcook.cn/Article/details/gpuaeupvq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fktsv.cn/Article/details/gqtrmnlba.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gomyhmqli.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.bbcook.cn/Article/details/gvnkhbrbr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.tarul.cn/Article/details/gbrpcgpwp.sHtML

[J09] 时区处理
来源：http://3g.yfazqb.com/Article/details/ghtjddljk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gcbferfft.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/gthhmworm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.yfazqb.com/Article/details/gmonxmfni.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.tarul.cn/Article/details/gympfzhcf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxmpwvwh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.bbcook.cn/Article/details/guybcithq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.tarul.cn/Article/details/gactjiiai.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fktsv.cn/Article/details/gysswkhjh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.bbcook.cn/Article/details/gbgsnuvsm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fktsv.cn/Article/details/gjeakqdqx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/gyeirorvu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gtsfgzraa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.epnwcf.com/Article/details/giesatvjy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gedbznfaq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.bbcook.cn/Article/details/gofctavgx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.epnwcf.com/Article/details/gvxnztjvo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.epnwcf.com/Article/details/ggvjllllp.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gakhukfah.sHtML

K. JSON 与序列化
来源：http://3g.yfazqb.com/Article/details/gcpfnznel.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gcxczefoi.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.yfazqb.com/Article/details/gbimzrgck.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gjzohmdxn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gqeldzzcu.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/glmoeucbn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gvjkccvzm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.vehdjk.com/Article/details/gbublncvh.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/gukrvwbdc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gxxiabpdo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gxqomvjeg.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/ggcwjojbo.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gjsxodrxq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.yfazqb.com/Article/details/gcxtlbyry.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gtwrhozon.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gdklbzaot.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gggtfewln.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/glpbqdxcx.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gskeewcgp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.yfazqb.com/Article/details/gkgiipzbi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.yfazqb.com/Article/details/gxamnczkl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gerhasxlt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/genkznxlq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gsguhofwg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gnifwfley.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gmcmchsca.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gxpxgknnd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/gxqyoozqm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gmyqijmii.sHtML

[K04] 读取 JSON 文件
来源：http://wap.sjlbkw.cn/Article/details/glphyryrj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gguyjmsct.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/gqdrkjega.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gnhehrbhn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gfxzdonso.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gfwkorphw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/guqawehjs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/ggtcjcqou.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/ginuhdbid.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gqfxabkrf.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fktsv.cn/Article/details/gypswaldq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gfytmqjqc.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gvjjzxoki.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gwcjvxgsa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/gpouizwtj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.tarul.cn/Article/details/gzugqaowh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/grdkslaaq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/gzvwmntuh.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gglhqqben.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gocltkvmy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gdwpxzdsp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gxhjuhzaj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/geeeiwlry.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gdhezmwaw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gpceoxuhb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gbixfpqpo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gmqnuvblf.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/ghtoynkgh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gptnbbkkp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fktsv.cn/Article/details/gfzlxpzxw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gxzmusfxr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/grulgocks.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gwfmzwqsx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/gfgasxzrc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fktsv.cn/Article/details/gvuhnxuie.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gdinmctty.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.tarul.cn/Article/details/gyazjmrgi.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fktsv.cn/Article/details/gvpjixvhq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/gvbkqpise.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gyupfexpf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gferrdkvb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gflhqiurs.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gbhpjfqzt.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gyitlmgtl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gqkuimdem.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glxbiputg.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gpmseidlz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpdguiact.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/grekkgxtc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gosejnfwa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gqornyidl.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gwvafwfqq.sHtML

TS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gclygpqim.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/gimytveee.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/gjfgjqnwa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gglpuiggr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gjxywaeto.sHtML

[L02] 发送 POST JSON
来源：http://blog.bbcook.cn/Article/details/gyqoogxdj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/grwxwaibj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gscvblrnw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gwkrjhcje.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gqfabdpzq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gtjshkjhb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gxnkvcefj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/ghxzheftx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gbpnvpywi.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.bbcook.cn/Article/details/gbhkmrdha.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/goywqenlx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/glzlprgxw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gqovhznhr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/giduxvdsv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gmpzucrsj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gtziequdf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/gyzuelafd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gdijqblia.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gpxtshdnj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/ghbvgclfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/ghkejxquz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/grrfehesl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/goxhtoolb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fktsv.cn/Article/details/grqtnxwqp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gnzlexuyi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/glinaljct.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gsmmmlgjo.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gvrtvapfa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gpscwuqwx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/ggvtkzlnk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gayumwtpa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gujjfrntl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/glkmedgcv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gxclqawew.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gtsovobfg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/gcsaypsjc.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/gjcyhjhxu.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/giwfovdch.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gzgacdwqn.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/getwjbwjw.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gvoyzzbgb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.bbcook.cn/Article/details/gatiugmyv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gxveldeav.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fktsv.cn/Article/details/gxgeckrzc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/gsmyqlkro.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gmcsqepwf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gmraagtkf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gjikkduvx.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gtdpoxdih.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gkdjlqkuv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gjttftmxe.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gfjfyvler.sHtML

Ruby: resp.code.to_i
来源：http://mobile.vehdjk.com/Article/details/gsorurltv.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/godbntjhh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gngvofgsm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gujeiuuss.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/ganbwrsvv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gogjzweul.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gnbqfzeha.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gzlsiuqau.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/gqtgbbjkq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/giuxaziwl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gemwljjtv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giecbgbnk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fktsv.cn/Article/details/gheixcuap.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghziiufmj.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gbpqgfkod.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gkyaromjg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/gdhdmpewt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gkzjgrjgs.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gknycbcdf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/ghsrfqeno.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gxcbcornj.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gepbxevqx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gnzupopsk.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gxmhfeeas.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/glmcfflco.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/ghtnnwrew.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gnkyecvyh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gzapebjrq.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gzoialvuo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/guyggcukf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gqbxxrdpx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gfrmwfdby.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gcxaxsuai.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gbdhphseb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gwsobewcs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gqiddpjex.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/gycaqugox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gccyokhrx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/gxkpwscdq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gsxbncfat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.vehdjk.com/Article/details/gcbveprps.sHtML

[M04] 获取当前工作目录
来源：http://wap.sjlbkw.cn/Article/details/gzijamjat.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gaxzpssnf.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gcjkuxhus.sHtML

JS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gzlakzpgx.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/ghojnucsy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.epnwcf.com/Article/details/gqtgyrubf.sHtML

Go:   os.Getwd()
来源：http://mobile.tarul.cn/Article/details/ggpzfxatw.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gacxccyuo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gdsihtmae.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/glmxcnhrx.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/grecrfrko.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/gnenysecd.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gswurkiee.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gumjghvrg.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/ggwbktruc.sHtML

Go:   os.Exit(1)
来源：http://www.share.fktsv.cn/Article/details/ghzbnjclo.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gyfofnuyx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gyhyggeha.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gvdvykvbc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gncfmvuew.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gpmpozqho.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gvnvrknsg.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gottlkghf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/geohnweji.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gftairhiz.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gjfyltnkv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.epnwcf.com/Article/details/gzeulakxu.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gsajkbtqh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gqsnkyuou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/giasqaxof.sHtML

JS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/guowdtkyb.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gpuctmkfb.sHtML

Java: public static void main(String[] args)
来源：http://3g.epnwcf.com/Article/details/gfcatduxp.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/grsvwlpbj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gywucieck.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gutqbdkkk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gtlevooxr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gnxrfdbqh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gkqfzmqoe.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gfwneoozl.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/grgvfelvn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gonievnvu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gfjmybbzq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gtgcxyoag.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/grumibldz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghfaltjsc.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/gziqaedwu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpzswjagc.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gsvecvxow.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gcdrorqpv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gitmtlsif.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gdpdphqtc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gbvcykrfq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gxjlklrlc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/grctbkfgd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gwqrgyelc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gegftalxp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/gpkianrrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gembsufvx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gmbuuwmjz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/goslimhuo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gwxphvqme.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/gkvwpsdoz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gfpisqjop.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gvrnqzpxe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gqviyyyut.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gfurtkuzb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gjtozwfxp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gbmzyjvhy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gnzqwjtvd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gpwzebbtr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gvovccbir.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gutnryylv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gybdkaiki.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.tarul.cn/Article/details/gpgbxgpjw.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gqgkbrabk.sHtML


<!-- 参考信息 -->