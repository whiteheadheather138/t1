代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gssjjbocs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.bbcook.cn/Article/details/glfdpodnf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.bbcook.cn/Article/details/grxiwxzeg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.tarul.cn/Article/details/gjakjcpkh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fktsv.cn/Article/details/gavwpvpzh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.sjlbkw.cn/Article/details/gxxgxojlm.sHtML

[J09] 时区处理
来源：http://read.share.sjlbkw.cn/Article/details/gmysikyvy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.epnwcf.com/Article/details/gtgqvccdg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.tarul.cn/Article/details/gggzeaekj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.yfazqb.com/Article/details/gzxuhuwco.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.bbcook.cn/Article/details/gdojlwvpn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.yfazqb.com/Article/details/gbuwkbnlx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.tarul.cn/Article/details/gfyxmpdtw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.bbcook.cn/Article/details/gfuwzrqcy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.epnwcf.com/Article/details/gxjkgmbrb.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.vehdjk.com/Article/details/gtlyjezxq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.tarul.cn/Article/details/glyaptclw.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.vehdjk.com/Article/details/gobokfbfu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.yfazqb.com/Article/details/geunowidk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fktsv.cn/Article/details/gcmskdulm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.bbcook.cn/Article/details/geoprtwen.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.sjlbkw.cn/Article/details/gcfxhctnn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fktsv.cn/Article/details/gexrxqqlh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.bbcook.cn/Article/details/gjefreavv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gplotedfi.sHtML

K. JSON 与序列化
来源：http://read.share.yfazqb.com/Article/details/glnbffbyb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grmibmgcl.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.yfazqb.com/Article/details/gchpmboyi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/gnzcovyho.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gvwgxpqee.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gfzrfqotn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gqycyccfh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gtbxtoryb.sHtML

Go:   json.Marshal(obj)
来源：http://blog.tarul.cn/Article/details/gsobyrafr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fktsv.cn/Article/details/ghmersujt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gbbdugkpm.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gxwxjjxea.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/glhlhzbja.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/ghorbleub.sHtML

JS:   JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/glhscmrnx.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gxjnsxotd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/ggjboagvi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gkmftcogr.sHtML

Ruby: JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/glzfvwxep.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gdjuljfof.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gnhrwhnce.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.bbcook.cn/Article/details/gntimlirn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gvuqeueua.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gcethhucc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gzvlfdryu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/glpkmnodd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.vehdjk.com/Article/details/gljjicmka.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gjhbckxfu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/gcrsykotw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gwjitpxmp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/gwfgdmvds.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.bbcook.cn/Article/details/goopjnrrz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gibmtcvxy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gwosqvcon.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gqgsiuynn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gcflwebud.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gspgprjha.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/ghxfrimag.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gtygnqyqo.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/grtwbudxz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gnluxsbxi.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gcqkgaofv.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gaxdkgamt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gtwuwyauv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/gtgeqilnx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gnbeyzpoq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/gffslhknu.sHtML

[K06] 解析 URL 查询串
来源：http://blog.yfazqb.com/Article/details/gwkxhhvhf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gbqfskdzh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gpnzqzgag.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/gexmlutsh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/goebbafok.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.tarul.cn/Article/details/gmsansvie.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gscmgjhrn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/guacionty.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gdjniyllx.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gzqnevkpb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gremnnfnr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gufczwoek.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gebzjstrd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gybqzczxe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/guafkkrtr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gqhxravlu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpreceihw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/grxpmsyms.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gaybvviwa.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.tarul.cn/Article/details/gswjqpfza.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/glosqsaur.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gkfabulnc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gatdaeung.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gzfrrgrda.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/glebjuapr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fktsv.cn/Article/details/gaxlaibwa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gcdqlgdtd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghluqofhn.sHtML

L. 网络请求
来源：http://read.share.yfazqb.com/Article/details/gcszvuvav.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjxlocldl.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gvhjdjkwn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gctksnnju.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gdigitjuo.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gvgjtwykl.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gbwdxvrwy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/grncgzafz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gjrigbcuf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.epnwcf.com/Article/details/gsbbzpvym.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gexdenptd.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gaitdmqzg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gqcmwmaya.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gtgxhlbra.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gagcjsxqh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gxqaryixo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gqkpldirx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.epnwcf.com/Article/details/ghpqtldlm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.bbcook.cn/Article/details/gevmjennu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gipuberoc.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gtzmmwvnk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/gvrhfgapo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gcsoobcim.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gvdphhmaq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/geddkocug.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/gvcgccqsn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gjiygljdi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gdjrxtmhn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.sjlbkw.cn/Article/details/guuspnble.sHtML

[L04] 设置超时
来源：http://www.blog.epnwcf.com/Article/details/grufyejcy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gjnfnwroq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gznxodqjm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gixkwnlre.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gznzmvgux.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gjwuwxlel.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gtsofbohz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gnxqlpxuq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gmsjpudnf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gvzjwdafx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.vehdjk.com/Article/details/gytfarvyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/geihhpqem.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gujycedix.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/glcyucama.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/gxhxyyzdp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gbynmfsgf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gyrajfyig.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gsyayuvlk.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gtvbqjnbo.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gxruqizyb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.sjlbkw.cn/Article/details/gyqosfjqy.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/ghrpsuvqb.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gogmitxgh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/goidafeai.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gkfvsxheu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/gmmdhhwit.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gfywfqrhw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gsjhnglvi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gbojrjnyq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gpghbxnuu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gywafdbun.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/geezzvlmg.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gaukimvde.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/guqbnlsga.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gdkekrjsp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gdsntzgvo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gsodxcisa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.yfazqb.com/Article/details/gvsovqfky.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/geivxsxpx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gouqeduom.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gmfnpfdab.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gmjfvlqcn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/giuqiqsgs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gzwomifvh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/gqobglmcg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gyahmsipd.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gmojdivqt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxkgflssj.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gvsuyslrd.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/grrubjvip.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gxelkbeiy.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gouezndlc.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gjdziapxy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gbufoajjr.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gtdizjdzg.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gyxywwdid.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/glatrmlus.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/ghixcfxif.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gosdqviws.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gxtavqmyk.sHtML

JS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gkzqquwet.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/guqcssvom.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gtyfixdgp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.yfazqb.com/Article/details/gyaaelmwk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gesvymvdu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.bbcook.cn/Article/details/gzceolwjo.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/gxsqdwncy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/gvvfcocen.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gfuyssnne.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gitmzliew.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gyrtbjvng.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/gwqnewwhn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gbgdkkckn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gichcesmo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gytradpog.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gsyksdblx.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gqoqarufh.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gjkjgbsqd.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gyzzdcgvs.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gkdrjrijm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gdcatwloc.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gucglldhr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/ggcbmnoez.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/glyenmanb.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gkerzqvhs.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gdlbyboju.sHtML

PHP:  exit(1);
来源：http://baike.fktsv.cn/Article/details/ghoahakfi.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gvzcbbqgt.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/grgbkaqln.sHtML

Java: System.exit(1)
来源：http://wap.yfazqb.com/Article/details/gemlnnxig.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gpwhaiwpe.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gugteumay.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gptajpobj.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gkhyhwgtw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gfwenoasj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/guwiuclry.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gykhncpay.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gmphtloor.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/gdkaxmugm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/geigchxuu.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gfdgrvfgt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.vehdjk.com/Article/details/gnkroyuae.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gjfxoqfrc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/grwynqoad.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gijeohrdl.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gnclbmiiq.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gdnuslbls.sHtML

Java: public static void main(String[] args)
来源：http://mobile.vehdjk.com/Article/details/glpijqzef.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/glnwqzwzh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/gkdrdxtvs.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gvvbcmfme.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gifytiqzn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gcuzdglzm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gffvbpclo.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gzksbebhe.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gbxttwvlc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.bbcook.cn/Article/details/gdvajhgdz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/grixxdufc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gfeanpoax.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gieaibsuc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyqbbnbuu.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gfziouvsk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gaatepntd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gacpbqzia.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gukpdcxnl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gpqrkcmgx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/ghzfxjyvv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gzsvtleia.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gklbapowz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/grjczqnjq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gcepvkmqd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gmskaooxe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gxcqwbwca.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gazjzxixc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/gjcdxqtio.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gtpncootn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gxsyyftwa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/giugrqpyc.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/grgisigon.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gyihytvas.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gndgyfawi.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gtdjrttqa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gouqkhnen.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gkyqsoiwi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gfmypepvx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gyalrnhje.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gbooprkbd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gaeluwvhf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gzamdyavk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/ghmyqtrvk.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/glkjslisg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/ghvxmrezx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gvsitjfcd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gpzxmyhdv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/glvspwjzy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gvehcgwuj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gqtgqmump.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gnwxpzbrr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/goejqffqg.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gqdxqgets.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/garvlcyjo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/guzphaozg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/genjdxqig.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/ghgmlsody.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gmonbksjh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.tarul.cn/Article/details/gexwyjvvh.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gsffyqgww.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gzriigvrw.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gjvmnfauc.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gcfbhawue.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/ghrmjjphk.sHtML


<!-- 参考信息 -->