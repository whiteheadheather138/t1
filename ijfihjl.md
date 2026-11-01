代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.vehdjk.com/Article/details/gnargzdsp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.tarul.cn/Article/details/gtteodnij.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.vehdjk.com/Article/details/gyblbtmdk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.sjlbkw.cn/Article/details/gadqymnuj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.sjlbkw.cn/Article/details/gyxofgqbn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.epnwcf.com/Article/details/gelxbasfc.sHtML

[J09] 时区处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ghabesoca.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.sjlbkw.cn/Article/details/gonrsctfr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fktsv.cn/Article/details/gsolqnwqx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.yfazqb.com/Article/details/ggkqcybix.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.epnwcf.com/Article/details/ghzpqzjlw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.tarul.cn/Article/details/gcdodolwh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fktsv.cn/Article/details/gmvcecxdq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.vehdjk.com/Article/details/gttccbqzh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.vehdjk.com/Article/details/gxbnfagdf.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.vehdjk.com/Article/details/ggzygqyct.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fktsv.cn/Article/details/ghqyaeoot.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gqnkbkadf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.bbcook.cn/Article/details/grjkrumnu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.epnwcf.com/Article/details/gcvodiuec.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyjcdybu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.bbcook.cn/Article/details/gphajeuwy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.yfazqb.com/Article/details/glcooxxxi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.bbcook.cn/Article/details/gnnttqfeb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqifaplfu.sHtML

K. JSON 与序列化
来源：http://www.share.yfazqb.com/Article/details/grbaymzri.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmskelstw.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/ggypwhcbo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/geuvipkqm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gmwfkxjls.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gpaavhqwa.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gptxfktee.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gnlbjvjuo.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gxekohlay.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gayruiayl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gmawhnlow.sHtML

[K02] JSON 字符串转对象
来源：http://wap.epnwcf.com/Article/details/gcsxxptwu.sHtML

Py:   json.loads(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwhsxrwcf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gxgeruher.sHtML

JS:   JSON.parse(s)
来源：http://mobile.bbcook.cn/Article/details/ggottycif.sHtML

TS:   JSON.parse(s)
来源：http://wap.fktsv.cn/Article/details/ggtlinckg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fktsv.cn/Article/details/gepewlznp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.bbcook.cn/Article/details/gecnsqhbe.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gtuuoxpzc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/gnbwxwhcf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gcaqwqpdx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gjymxibbl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gxymqjivr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.tarul.cn/Article/details/glyvdtigq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gunggyjfu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqqruvywn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.sjlbkw.cn/Article/details/ghvwicbpw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gkdhfuvkx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gymclxxcc.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/gwzeorjsl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.bbcook.cn/Article/details/gagytmlbw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gskdazopg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/glnpvgjzp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gqiobptme.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gocqhawta.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gsxupogeh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gyqqqbqda.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/ghfdhzqmn.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/ggfspffsd.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gvgfomoqu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/gldnkfzcu.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdvlnnjrg.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gebxzzzhe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gsegfwzja.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gmvxhyvxc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/getftimbb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/glksifyeo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.vehdjk.com/Article/details/gkkonqdgu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzxfnxmm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/gggvbssog.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/grqrqfhjo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gfqeqycqp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gpjuwlppo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gjdnagzfi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gqmfzlfdo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/guufrdosu.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gowbblhti.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gtgpfapfe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gzgwijmgc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/giwwbnors.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gdruepebk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmsisdvvv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/gefkqrmlg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fktsv.cn/Article/details/gqotnqhnz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gaddgroug.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gnoqfhgsr.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gmnvtjrva.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gadrdjzuq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gyxoxpoew.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gwjhbdyjy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.epnwcf.com/Article/details/gyfolnvuw.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gevvwtuqk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/glqouromz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/ghhcwnchw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjmzbitgc.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gjmquzriq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glgbbafve.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gxvgmdgxt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.bbcook.cn/Article/details/gfdgyhscz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.bbcook.cn/Article/details/gtaganjdz.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/guiiwkgii.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gklqixzor.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gucybuczz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gmfdqeluc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gqfbegehl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gowwdvawk.sHtML

[L02] 发送 POST JSON
来源：http://3g.vehdjk.com/Article/details/gskcqspjj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gessglcfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gwwfxxoth.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gsarestfp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/ggmfzecez.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.sjlbkw.cn/Article/details/gsbknhdpl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/goxseardr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gpkarmnue.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/gcxjrkjqq.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gvzivxhwl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gufwzxhcn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.yfazqb.com/Article/details/gjkbeufsw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gpsxcvjor.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gfsgpkbcq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzpwjmqv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gcmnnqhcx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gbultafph.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gmvhlgufm.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/gyvgoahud.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/grxczxlmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gpurtaxrx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/ggtbcxaea.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gratgljdo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/gexhcrtmj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/gknwdktsa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gzypvpktr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/gwhvobpfv.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/guwblfwgb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gshdgiqtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gzrrwddsm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/ghjkypqax.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gwqptdtwo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/gyaesqycy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhbacqib.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/glrvbwids.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghpkaazof.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gurayvned.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/goucpdocq.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gytpiqfiw.sHtML

JS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gdmrfcnbf.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/gevctuhhw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gpkigfrpx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/ghcjuzfqy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gqyilyrmj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gemmupgja.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gooyqlmvv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gpiwqstpp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gbbmepxdj.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gghifgnoe.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gqppjzeoq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gyrftutjg.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gqwctyjby.sHtML

Ruby: resp.code.to_i
来源：http://wap.epnwcf.com/Article/details/gneexgyxy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/grqmqzwbp.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gvcnzmmri.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/geliqbria.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gdirnvlpv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gyxhlhdtc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gaoybtemb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/gatjurcyh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gbgumvmuw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/gnwstblfm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/gvpoftitx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxvijtmto.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gfcjlommc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxidosrax.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/ggivykovm.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gftbcasce.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gtmvjvfhr.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gsqiwzcoq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gmmpnuecg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gymwqqifu.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gqpjecusr.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gwovggbgn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/glyxtyyuy.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/guktdhoue.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gnbtcqzvx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gefzyzupv.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/ggivcryhu.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gqhrqwagt.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gqhezjrlq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gbtjbzyek.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/gwfzssppe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/ggvdubvlk.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gbqrcucvy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.bbcook.cn/Article/details/gvrptphwc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gxrfyigew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gnqzykvfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gfrslsayd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gxgvmeurj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gxffxzeqp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gjwyaehku.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/geftngzwv.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/ggdlsbrby.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/ggdcjhxgh.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/gmtglfcvg.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gsozvklgu.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gfsyxbxvm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gdjoruuie.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/glqlsoasc.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gtlrorzhp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gptyirpuf.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gefldjyie.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gqzcjzakd.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/gcrebcvxs.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/guemwsnad.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/glvbpkhko.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gamzgwhmz.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gafowuodo.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gzblvizsz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.vehdjk.com/Article/details/gnkgbnids.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gkflrhwrl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gqcxpkdfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gnueicwft.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/giggiwzqw.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gckqfmrqm.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gnsuuhjuw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/gameqlyht.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gojrgjffl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gndbewvxe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/gbolwwxij.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gspsklpkg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gbxgioaer.sHtML

JS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gnjbjrmpa.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gpgtdiwcg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gbulrmqbn.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/grgapgsjy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gyrwultei.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/geiipzbzg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gcydzykqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gtwjkgwes.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gbkfclkny.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gcoccbplg.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gyyaquyph.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gntcnauui.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/givkkyrhm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gbjnuiihs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/ggrhhizcy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gthgzcxtt.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/gqmoqyujh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/grlphyjcy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.bbcook.cn/Article/details/glbrumsrt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gpdgppfca.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/ggytalngb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gwpfkzhve.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gyhcqpllq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gtmgfgzcw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/gkpzduorm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/ghcdumjlm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/ggsgtzpjn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gitpvtbwf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/ghrbmnzrx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gyxqkfrbu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gkggutubp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gefhmkhvr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gnszsaefe.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/ghpxvaebw.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gnhhczcrr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gkdkqzutb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gdlczostl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gxjitagww.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/ggmzgrhqm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gjbwfftuq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/giafdwgbm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gzjxwaarx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/gptydyzrx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gjriebkas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/ggvljvgqx.sHtML

[N04] 斐波那契数列
来源：http://www.blog.bbcook.cn/Article/details/gsaazwedj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gxporthfa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gdxluvlly.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gblxvvuqx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gsklxxpvh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ggwlpjwnn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gsrhbrczs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/ggxdnowes.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/ghrpqkbpx.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gukccrdys.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/glladkbgz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtypggaap.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/ghdlxmtti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gnussimgf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/givawvuwb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/guemmrkqn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gatzpfkhb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/gcsrcnqas.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gcysvfzmb.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gthgxfshw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gjfzsaian.sHtML


<!-- 参考信息 -->