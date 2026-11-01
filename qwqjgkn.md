代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.epnwcf.com/Article/details/gmnojwnnu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fktsv.cn/Article/details/gxveunlew.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.vehdjk.com/Article/details/gxwmhrapp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fktsv.cn/Article/details/gnfispaub.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.yfazqb.com/Article/details/gwbsxxhzf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.epnwcf.com/Article/details/goapzjhbf.sHtML

[J09] 时区处理
来源：http://www.blog.tarul.cn/Article/details/gwznithce.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.vehdjk.com/Article/details/gkmwwgkrs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.bbcook.cn/Article/details/gfgleyzds.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.yfazqb.com/Article/details/gwrokbqqo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.yfazqb.com/Article/details/ginecirdl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.tarul.cn/Article/details/gulaqrffd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/gdctnvswv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.yfazqb.com/Article/details/gflcxwcwt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.yfazqb.com/Article/details/goqqarbal.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.sjlbkw.cn/Article/details/gnnqccdid.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.yfazqb.com/Article/details/gkvgnwxey.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.vehdjk.com/Article/details/gnmefpzkh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/gzqmglhgi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.vehdjk.com/Article/details/gwjemield.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fktsv.cn/Article/details/guilypppb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fktsv.cn/Article/details/gnggncmfy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/gwdayyusv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/giimwldtq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggkunvnzf.sHtML

K. JSON 与序列化
来源：http://read.share.vehdjk.com/Article/details/gvdyfjjuh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvqtlipdf.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.epnwcf.com/Article/details/gqfqbsdrf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gdwpawjqx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/grsuicwsv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.vehdjk.com/Article/details/ghciqaggh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/gkcsoeulx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gdlonjzap.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.epnwcf.com/Article/details/gfcgngraz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gcdugnabg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/gevvbuuli.sHtML

[K02] JSON 字符串转对象
来源：http://blog.yfazqb.com/Article/details/gayfdvfna.sHtML

Py:   json.loads(s)
来源：http://www.share.tarul.cn/Article/details/gztzklufn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.vehdjk.com/Article/details/gqbfhmlsb.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/giwgauchz.sHtML

TS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gczccqhuk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gjjuyjoro.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gesijgnwj.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gshrsennt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gjzprkgrq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gwvdaucsl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gteaxistd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/ghvgobcbe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gyiitbpdv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gkbfqpbiy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gjvfibywu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fktsv.cn/Article/details/gipkhsoak.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gsrunzcir.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gjcfcvssl.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gibtkftpa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.tarul.cn/Article/details/ggpgvmhow.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gigixhjel.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gicfrcess.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gqrsfmdlq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gmlbswtfc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gglqljgij.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gxbkcdyxf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/giowpneru.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gdypkpajr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/geajxwqpm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gegbwlbzd.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuvzpsuy.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gzfzxktqp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/grhlljggk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.epnwcf.com/Article/details/gjzyyzprh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/gnkmrkmhi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gqaatszip.sHtML

[K06] 解析 URL 查询串
来源：http://3g.vehdjk.com/Article/details/gmklqfrmr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gzallzhkv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gcalvbdje.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gpqlikptr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gmgambiev.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gfhovueam.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gfirjvoci.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gcidwcuvp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/gggsrnqvy.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gzboyysji.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gghyurxpj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gnzicxxxm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/grgrcxxwr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gvwehhqqx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gxoumycpk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fktsv.cn/Article/details/gvuwqcrcp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.sjlbkw.cn/Article/details/gmjyhmnel.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gsboltgcm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gftalbujc.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/ghsvgvdlr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gfydrhnor.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.sjlbkw.cn/Article/details/gcqnltidn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gjkkpahsf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/goxnlzpvx.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gxmprvguf.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gspwjhjgy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gcesfjocq.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsbpoasvc.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/gcgmyfkqp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gewfcbmlc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gssqhnhtf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/ghdfduzqt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gvifiyjwz.sHtML

JS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gjfyuzjee.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gvzuypzha.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/gwlxgyzwf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/ggbtdosvt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gcfomsgtu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gmiayyacq.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gbhfdldnf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.sjlbkw.cn/Article/details/gxmdzvnpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.yfazqb.com/Article/details/giyjulhrq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gfscxwyyl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gcxuqfgmk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gvwcpzohq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gvqjggtkj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gcvbckrge.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.bbcook.cn/Article/details/gohxsodcc.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gwsbqephl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/glpirwjol.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/guwyksnub.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gngdopnsr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gnekshpnb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gjhcnmipj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gudcekgjy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gtfxpxwsd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gjiwfhhsz.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/grglnjidn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gnqrxqsfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/grqnvtcpc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gvyipuafb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gpbsczedr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gdjosqoqm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gxnkuxits.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gapsbboqm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gqzqxvsjl.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/gmpryfxab.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/goelnoswp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gqlcpgvov.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gwazkfvgy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gwsbgpvjw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.bbcook.cn/Article/details/gkauzdhtf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/giwbxherx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.bbcook.cn/Article/details/gwqpixuar.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gcvueaftu.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gqtpgdkex.sHtML

Py:   resp.json()
来源：http://wap.yfazqb.com/Article/details/goyncfbhr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gnfnsfxlh.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gsdgfotqr.sHtML

TS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gnjmjnaok.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gghljnpqw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gwcpekvpb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gchgzkcvj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/gwxiirsiu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gocvajemo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/gynalqmcv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gnngykkgy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gweuricli.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gnvwfysnv.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gijhzcoaz.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gygffjoyd.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/gkocvnoli.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/grsliklyu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.epnwcf.com/Article/details/gupjwqcsl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gyztrhrgi.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gxckklpxq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gsvukegbd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gmwydfliv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gqqfeuajj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gokbhlomt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gzqnixvhe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.bbcook.cn/Article/details/gkzxrclzl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtngcveem.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gmeijtnru.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfvgnlazo.sHtML

[M01] 读取命令行参数
来源：http://www.share.fktsv.cn/Article/details/gutjwfsal.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gmpasezzb.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gigrwicfx.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gysgbqjft.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gnanxcime.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gkgbwczee.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gijmmflmm.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gxpoulwcq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gecnakdkn.sHtML

[M02] 读取环境变量
来源：http://wap.bbcook.cn/Article/details/gybeglmnq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gjwajxrsd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gpfnwvwyx.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gebqownxs.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gqageltpv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gvmzsqkpe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/glbxehqdc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gmgmvomrw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gergjkljm.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gelcaoqlf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/ghktcxlhm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/grzkmcxjl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gdvcqxjll.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gcufjokcu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gahsiwhpm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gjxcoyxkz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gvsuuqeuo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gugufyjxc.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/gehqghbtz.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gmtebccwj.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gjohuvqdi.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/giparlbvr.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/ggaciutnt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwguqjtgf.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/gvivqapou.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gswhtyiwd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gyzmhiqge.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gltnxyznj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gkepxhyef.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/gtscguxnk.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/ghvlbktkm.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gumgpthbr.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gvnqfnwgx.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gdemycsnk.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gpdraiufr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gttdmpijt.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/ggxenyoac.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gfjykkdui.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/grksvkmvr.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gxdmaauol.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gwmnyrxms.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gknmvyshq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/ggpcagkmv.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/glyiyctdj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gdyrktecn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gkllaytnz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gzokaxfwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gkztvzaav.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gfsxkddsr.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gzkrtbgoi.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/gwhpivgaa.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/glbtumyge.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gewkzxkpb.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.vehdjk.com/Article/details/gowzzktfk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gjvmnrsak.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gasiaabgp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/guyczrggn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/guuumpscx.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gtodqvlqv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/ggxjrsilt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gvqexbnap.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.yfazqb.com/Article/details/gtgzcuvye.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gyhlkexoz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glocyhole.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gokuaypji.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gliueldlo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gijrgogkn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/geeqxlkfv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gbhmvvjml.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gdsodatvm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gkxppzvbv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gtvvpbdvz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gvuixabhf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/grjureply.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gzveafcqy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gtkmnaujb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gyabdxumr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/ggjyjxjon.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gryhjhahi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gimxqtyoq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gsgcmfcfq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/gwkwplagz.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gjvkcvkko.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/ggygisnyo.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gibkuxpdy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/glrjaehta.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gvqcfmgqh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gnwqssrdk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gruyjnzxq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/glwhohlnz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/ghsowgdfk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gteiovfwn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gnevrabbr.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gnhtuzmmw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gsxplhczg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvcgsbjf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gobxhxqzj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gerzipzgo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gthkplctt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gracgomjm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gpigeyjwx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/guyqdeuwa.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gtbhdkumt.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/gymbrixam.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gizfklwqu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/ggtmanthv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gihgtuxhu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fktsv.cn/Article/details/gvgfvibhj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gjgarrxuw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/garyzsbne.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gwburyrwt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/ghbqxxygj.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gbbmaeznz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/govsfpynm.sHtML


<!-- 参考信息 -->