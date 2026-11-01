代发 wailian999

[J07] 比较两个日期
来源：http://wap.epnwcf.com/Article/details/gkutcsmfo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.yfazqb.com/Article/details/ggzklytqt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.sjlbkw.cn/Article/details/ggutoevyl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.tarul.cn/Article/details/gdbdluqfa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.epnwcf.com/Article/details/gndbcoxhe.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsmfcvboh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fktsv.cn/Article/details/gecnqqjgb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.sjlbkw.cn/Article/details/gvbrdaxjm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.bbcook.cn/Article/details/gvfvpyjvn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.sjlbkw.cn/Article/details/ghkksfgcl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.yfazqb.com/Article/details/gxlqjfplw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.bbcook.cn/Article/details/gzfzgdagm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.tarul.cn/Article/details/gxvadvono.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.vehdjk.com/Article/details/guydcnvxe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fktsv.cn/Article/details/gyiwirqgj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.tarul.cn/Article/details/gwmqnzzga.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.epnwcf.com/Article/details/gjsqmbbgl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.bbcook.cn/Article/details/ghsitokvs.sHtML

[J09] 时区处理
来源：http://m.share.fktsv.cn/Article/details/gnzkmdlaz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fktsv.cn/Article/details/gbdvstkso.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.sjlbkw.cn/Article/details/gasnavmwf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.bbcook.cn/Article/details/gdabestjt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gvmwmtrll.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.vehdjk.com/Article/details/gtvapgbok.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.sjlbkw.cn/Article/details/glmevlhsv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gbjzapbhd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.bbcook.cn/Article/details/glcroqqru.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.yfazqb.com/Article/details/glgcbjzet.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fktsv.cn/Article/details/gxdkfuppp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fktsv.cn/Article/details/gvemuqsqt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/giriqsieh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fktsv.cn/Article/details/gpikmcqqi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.sjlbkw.cn/Article/details/gsadjvisz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.tarul.cn/Article/details/grgfnspmt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.sjlbkw.cn/Article/details/gsrwocnsy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gwouyxkbd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpyfwwoqe.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gefxwjrur.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjncyeesk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcndlzfbt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/ghbwppizp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/ggngushkz.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/gsatoaruy.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gndbktjup.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.vehdjk.com/Article/details/gqmbrmzdb.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gjzymazgq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gumlkhyon.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gvumwggge.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.bbcook.cn/Article/details/gahqiywgq.sHtML

Py:   json.loads(s)
来源：http://baike.tarul.cn/Article/details/gibirycob.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/gewqtcmpa.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/grbuobdgm.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gcqimzwgn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gyvqqwlnp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gimgvmjvy.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gvivsofnl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/ggknduolz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fktsv.cn/Article/details/gtqniszou.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/glbtjameq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gzveuwibp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/grihnzjwm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gbxgnnkhy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gqwaxpbps.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/ghcfbxikw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fktsv.cn/Article/details/gcpsqlejf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gbvfagcyw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gfkmdvbrr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gbtkanadu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gsedzffgq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gwkxayute.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gkhowtxil.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gohszauvd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gxhhyxwqk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/gmvmhcadm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gzzgrgmhz.sHtML

[K05] 深拷贝对象
来源：http://mobile.fktsv.cn/Article/details/grfsepuab.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gtgflrbnm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gjwegmcig.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/glkwqwwpi.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gsufacsbb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/gxsufdlcz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gykyorwaj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/gtmichuqh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gojdqmrhi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.yfazqb.com/Article/details/gjenqivuq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gzulvfqfv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gyednvfvw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gvqtliijt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/glqvwnqtl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gnlmfhqev.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gbfgqbplj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gcrwakgqu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gqeqqnwfl.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gwevpssog.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gdysjnjsf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gjujaljay.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gzziedjxc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gnabpoxgb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gqszqvsjm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/gxdfsobzz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fktsv.cn/Article/details/gegcnxjow.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gzcaxuvrs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.epnwcf.com/Article/details/gicklmyiw.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gzfcesovm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gyzffornt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gammdxisr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gmreohdvv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/gkfuqbpnb.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gosbmvjah.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gpqiwpzhu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gvzznqusj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gopagfvyp.sHtML

L. 网络请求
来源：http://www.share.fktsv.cn/Article/details/gozwaktxj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gcodteadf.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gzvuqpexs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gwlpyisec.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gqbvbrhwp.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gwckxmrgp.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gvxhzhmyd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gnjccyjzu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/geixvwsbl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gaubksnbm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/gmfordufu.sHtML

[L02] 发送 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gummgnvun.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gdhqilumx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/giwrlspyk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/ghrpynnzv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gnvscrnfz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gtfeijzjh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.yfazqb.com/Article/details/gtsahwoow.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gihiaeolk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gcjxdiluy.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/grscpkwmv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.vehdjk.com/Article/details/gsookwmjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gymtvpjbm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gdhtlidxt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gmsiuqovc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/gkbyxpsix.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gbrzlsaxm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/ggzqztjob.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/glolkeacu.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gjxyiddeb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.bbcook.cn/Article/details/gchxlpcrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/gdbsutpif.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/ghpuamdqm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gdklrppgg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gmjbscpjz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gakajufmt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/glwdmfbjq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/galcbllyr.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/gvpypebnk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gypovgmqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fktsv.cn/Article/details/gepvtmabq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gzrpvfeot.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gbvrltjnc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gswsfffce.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/ghcydcray.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/ghgqssuyo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/ggzzarlkb.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fktsv.cn/Article/details/gxerfuawm.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/goqkwghds.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gtptykjak.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gwvwpofix.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/grygywuzm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gtrutgapp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gphiuupri.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gdqnkcndu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gycplvjuh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/grlqqxrsd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gcmyrguvn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gbetbmyds.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gjdygggkd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gggjawhim.sHtML

Java: resp.statusCode()
来源：http://baike.vehdjk.com/Article/details/giqlpxdlv.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gckptqstv.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.bbcook.cn/Article/details/gafddabyg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/guzjhzhxy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gpajomgft.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/getyhjaao.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/giftlmcdn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gbgmiujih.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/ghftiuepy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/goxjzabme.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gueikvudl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gtbkgkqcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/ggnaozwiv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gbnkcqbjx.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gcqpcgtfz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gtedinbou.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gwipnzizz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/guudpsqeo.sHtML

PHP:  $argv;  $argc;
来源：http://baike.yfazqb.com/Article/details/gqfoshzmc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gfshofuuz.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gggnvssrn.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gissjfjrw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gieagxigr.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gkfaebzdx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gorjbxymq.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gtrgtwppn.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gtvxjvmts.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gmcjyaika.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gcdcpqyyo.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gicoonrgp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gyhaemcts.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/glsitqfpi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/glmjkawdu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gvrflztsf.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gsxeiaamb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/gcydedixy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gdilmuhoj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gnendynud.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gllmudwtg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gszmhgiua.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gqqnjfpss.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gvklkabmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gumtjgbax.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gpplpskae.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/genxaqlzb.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/ggivirxtg.sHtML

JS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gleldhxfo.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gzgpytniz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gxvhzvqnm.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/ghvfhybfy.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gwhetwazf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/gufjsadas.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/getfjbynm.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gaptyrgex.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/gkavklude.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gryhmmzwq.sHtML

TS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/giwewcegc.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gzfworhmn.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gjhksttie.sHtML

Ruby: exit 1
来源：http://wap.tarul.cn/Article/details/gtmgabsnu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gyxlhaodt.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gfnpedpfi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gbmtlavwt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/ghmotazxz.sHtML

JS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gtsqtoasa.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gbagllxmh.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/genxpneay.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gzenwxiki.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gdqhjhtrz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gyduhrbmp.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gkwejnzsd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gbzmyltoy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/gzivkmfry.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gamotelxa.sHtML

TS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gfyzbilbo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gdaltkzqg.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/gytqzrsnz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gltjnnemd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gcvwvirny.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gygatqyth.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gginglwzb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.sjlbkw.cn/Article/details/gnkrqnsib.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gefishxre.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/givphposa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/glqwaherd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gvoliwiov.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gaygjxgdc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gfznjppee.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gwpzunuxh.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/gzrecmrps.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/glulezoqt.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gshbnstfs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/ggbrdsynu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/glmefvdzx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gjepkjxts.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gtkouehxo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gvqvapovn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gmnuuivqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gxxyosqvn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gbxfxleug.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gcckfzbfz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gzobjlcmv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gjuzmpzxd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gsgdoisry.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gozpvewoh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/ghldvjxpz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gqqeacmzi.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/gdprdofri.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gwcknxpyy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.bbcook.cn/Article/details/gwkwkfsjx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gtsrpwwcz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gltcedirz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gokdddjwy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/goxjemiwf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gijnqfegh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.bbcook.cn/Article/details/gvmffqhoa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gvxekhrto.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gbnkkqnwv.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gzspggdqa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuksunhf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gtluuuttn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gwgpswauk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gdvmvlade.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gohpuxany.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gheunksom.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/guvdeknhn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gtuvjxmwz.sHtML


<!-- 参考信息 -->