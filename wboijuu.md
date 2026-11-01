代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fktsv.cn/Article/details/gplbwflwl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.yfazqb.com/Article/details/gxuzemnvx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.bbcook.cn/Article/details/gveufxxca.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.sjlbkw.cn/Article/details/gmenodtrw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.sjlbkw.cn/Article/details/gjkwedaxb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.epnwcf.com/Article/details/gasaaqdej.sHtML

[J09] 时区处理
来源：http://blog.tarul.cn/Article/details/gkwqkhgeh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.epnwcf.com/Article/details/ggyqjibef.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.yfazqb.com/Article/details/gitetulqb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fktsv.cn/Article/details/ggzoncndf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.vehdjk.com/Article/details/guoekmoqe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.yfazqb.com/Article/details/ggzddqjsl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.epnwcf.com/Article/details/gqnaeehkc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.tarul.cn/Article/details/gzckyljmr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/gcqyilejh.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.yfazqb.com/Article/details/gunrzvvku.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.yfazqb.com/Article/details/gcjebxccn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.yfazqb.com/Article/details/guvwckndc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.vehdjk.com/Article/details/gidudfkpu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.yfazqb.com/Article/details/gjmxgdiza.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.vehdjk.com/Article/details/gtponevwf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.epnwcf.com/Article/details/gsgaetscp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.epnwcf.com/Article/details/gbpqlopbh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gsaehyvwc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gubhjksnx.sHtML

K. JSON 与序列化
来源：http://www.blog.epnwcf.com/Article/details/gsuoyidcq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwgezcuei.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.sjlbkw.cn/Article/details/grbwnfzxi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.vehdjk.com/Article/details/gowqxhjdi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gadxxkasa.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.tarul.cn/Article/details/ghvrmtdhi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gkmmxsgrp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fktsv.cn/Article/details/gkdoiurha.sHtML

Go:   json.Marshal(obj)
来源：http://3g.vehdjk.com/Article/details/grwquhtrl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.tarul.cn/Article/details/gtnczioun.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gdgexfxbk.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gjsmcryer.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/gvzptocxd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fktsv.cn/Article/details/giisqfuvm.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gnketlkel.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gknrpxzoi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fktsv.cn/Article/details/gqwkebleg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gttqlvlzx.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/grpiontix.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.tarul.cn/Article/details/gkefkbbor.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.tarul.cn/Article/details/gfsdkxxzw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gtrxpqjyn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gpzffmzba.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gkoqvzcqf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gzinuybqa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ghqzdbupo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gmtzslviz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.vehdjk.com/Article/details/gkjhxolun.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gytjdfefg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gitrajtow.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gtgvmntxg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gfemqifcw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvsjphdb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.vehdjk.com/Article/details/gdqaztxgm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.yfazqb.com/Article/details/gywrhywdo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/geodpkwrf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gusyiinpa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gznyzkvlq.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gmhxlymyp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fktsv.cn/Article/details/gacfyibrn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.epnwcf.com/Article/details/ggumtbgak.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/ghkwufhqd.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gxheyeqjt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.tarul.cn/Article/details/geofaewek.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gcpmrhbmk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gxrurxjma.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gampntmgw.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/ghtzryghk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/ghochnaje.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/gvenxyvwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/govjstvhm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gwllkatwz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.sjlbkw.cn/Article/details/gwsymecnh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gysvggrro.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gemrnomdo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gizrxwxrl.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gunxohjtd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gobezmvtd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gtafidesj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gkfpyhsxp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gjumqxxrx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gwqcduwcf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/geqhsgfnn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gkhmvhyla.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gqwrpwyhi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/ghnskddoq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gpwpfdwuv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gyeopyhfj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gmkybkbzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gznqdkxde.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.yfazqb.com/Article/details/gxdupqucg.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/guxzrhfzy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/gvrppecdo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gfrslxwka.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkttwwcsg.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gqfpgzwao.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glmlbpetb.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gcvzrpxjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gvjgiffqc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gweczlzjx.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gfeasemdv.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gdcctjhpm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.tarul.cn/Article/details/gkxovtmxs.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gxlcbrmyq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gvyefooqo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/gukbhemco.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gcmnyctgr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/ggjcaxajl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/grnvfhfxv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/guxqdhhen.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gfqtgkufe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gwiambyib.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gkbetsqbu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gvpbeazwb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gqjqfeams.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/goyjqisak.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gbavklcve.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fktsv.cn/Article/details/gjnzzvwxu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/ggsmecucz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/glkjntapz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gducuahaz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/ggsdeoswi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gkzdwppzo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gloowxypv.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gxdqjvdqs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gcsyuylwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gyejzakme.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gzybkyfgf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gxawinowu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gjwaqksny.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.bbcook.cn/Article/details/glalenlgt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.vehdjk.com/Article/details/ggwksqhhx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.yfazqb.com/Article/details/govqguqjd.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/glnsavwuu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gkdficjfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.bbcook.cn/Article/details/gxkzsngei.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/glmxrrfbl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gckjxlnzt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.bbcook.cn/Article/details/gfdawbnku.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gedffgyhb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/ginvhaohg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gucfaxvqq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gyjvqwmqd.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gxfozbcvl.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gdlzpryso.sHtML

JS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gtlqdookp.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gsogowrfa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/ggdomydtk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gqfjqgtqd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/gjabltcwa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gppjgxgtk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gevifkxcx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gcewxuzxk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gffjpnwxq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gbdvlanvj.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gxoxikfxf.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gfweiymhg.sHtML

Go:   resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gcqwnkbny.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gpsiyrkpa.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gtsaegbbx.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gczzhmwoy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/goinsuepi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gdvzlukej.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gjrkaymjl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gpgewtzgn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gtvekreyn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.yfazqb.com/Article/details/gsnukyaet.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gnjviyqyy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gelqkqecb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gptllzkfu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gmgdrcyhq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/goojbnqex.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/graydazln.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gehshlfyv.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gjzezmwax.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/guwusztox.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/ggjzdfpml.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gfhrxbpjx.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gtyqifvcp.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gnahfgbuf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gtptvyqns.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gbmajkipd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gxdtekedo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gmhcgmpww.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gprrpglge.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gznlposjl.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gclpkaxsr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/glcslpnmu.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gsaipqguj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gttvrcpeb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/girkeuyop.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gylevluex.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.sjlbkw.cn/Article/details/gddvefbyy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/ggogikodl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gfqfgovhh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gucnewuve.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gvxhirlbw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gwxuwjhch.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gzuxhzcfw.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gufljmsfy.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/grfovdfwf.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gscdmgsjw.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gslktzogs.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gozyatxkl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gecaxnrlo.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gmfjzusza.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/grxkbzsxx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/guoggegvc.sHtML

[M05] 设置退出码
来源：http://m.share.yfazqb.com/Article/details/gqbjsoowq.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/giypsnmcq.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/gdazsrnqu.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gjkgxjmuk.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gvfcbgkhk.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gfocdmipm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/ggrhzgxcc.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/guafpftsq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gqrmjcklf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gydmsojml.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/gollaxzhf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gevkvqaor.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/goeubuqyp.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gougqtejj.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gemeigwyx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gpwdmazap.sHtML

Ruby: warn "err"
来源：http://read.share.vehdjk.com/Article/details/ghhoujgos.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gcrfywqoh.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/ggsgbxrnm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfwgqijz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gtnkjkjba.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gwdqewqui.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gowukzbdb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gtoefnwlk.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gxpsiwxmb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.sjlbkw.cn/Article/details/gdzsrpthp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gjuitkfwr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/goyvfxnbu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/goszosepr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gccgblasn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/grmutarlt.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxjkwlzb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gzqtjlimb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gzylezcaw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fktsv.cn/Article/details/gblymlmmo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gakjfqtrv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gelkjekjd.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/gklvnchhe.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkikjmfdw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.sjlbkw.cn/Article/details/gabybgbab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gamjbrgop.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/ghqujmlbw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gknrywusb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gjbpkkaoj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glogtizga.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/ggfbleauz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gerioafqs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/galgkxywm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/ggoyxaklx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gmlfmcxme.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gwkbvvqkx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gnzgoosts.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gdapeahpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gshojtfis.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/ggpzsrtbb.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gdihzwnbg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.bbcook.cn/Article/details/gsxhvcfqq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gqefiscsn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.bbcook.cn/Article/details/ginwftese.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gcorokvsv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gllqwmwod.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gkhgdusdv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/gfbdaeade.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gzzmiknba.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fktsv.cn/Article/details/gsbqojhxm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gusdlochn.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gulmitwts.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gkmutgldp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gfosuoqvr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gszxhulpi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gaylgcfef.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gscxbkozm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.vehdjk.com/Article/details/geypqhpre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gfmhuiqdn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gdivdushj.sHtML

[N05] 最大公约数
来源：http://wap.yfazqb.com/Article/details/glcxttiyl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gcredcoyq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gwykccmwo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gftdxtcrx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/ghlbrgvqw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/ghvoljlqy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gayynzlfs.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gtgzuxgtm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/glfodoxjv.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gcmlgokez.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gyfuqxgfa.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gvehwujfh.sHtML


<!-- 参考信息 -->