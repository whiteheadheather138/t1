代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.epnwcf.com/Article/details/gwpofcglm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fktsv.cn/Article/details/gddyuzemz.sHtML

[J09] 时区处理
来源：http://wap.yfazqb.com/Article/details/gmxgvkjzp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.yfazqb.com/Article/details/gadefpztj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fktsv.cn/Article/details/gchcgoaln.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.sjlbkw.cn/Article/details/gqyualsac.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.epnwcf.com/Article/details/geyotyaho.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.vehdjk.com/Article/details/gwpargpuu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fktsv.cn/Article/details/gkjczfply.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.tarul.cn/Article/details/gxgummomq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.sjlbkw.cn/Article/details/gdiozqyhv.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fktsv.cn/Article/details/gbxlfkcma.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.vehdjk.com/Article/details/gxipcjxhi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.vehdjk.com/Article/details/gzslaqyix.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gqysnkwfy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gimiwaiie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.tarul.cn/Article/details/gdrjziaxd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fktsv.cn/Article/details/gigxiebcl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/gczjrksxp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/geekolask.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gayvxvlay.sHtML

K. JSON 与序列化
来源：http://www.share.yfazqb.com/Article/details/guqdxogla.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gylziqwqw.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/gnsjkeuse.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/ggjnqyebb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/gkoobwblr.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.yfazqb.com/Article/details/gptanswuh.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gcgoahbrt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fktsv.cn/Article/details/gcsqxdqux.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gdmcgqnzh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/gxssplbsa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/gwqrvhkpl.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/gcmtwukpz.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/gksxnmwrv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/geksmqhsj.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gqvwnbnqc.sHtML

TS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gvyubxyhz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gaegbtynm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpinftutb.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fktsv.cn/Article/details/gecjfmyls.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.epnwcf.com/Article/details/gfzzolhfe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.tarul.cn/Article/details/gvwnlmpqs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gcxljdoaj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/glzvpnfrb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gsnerhfdw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gvjztlcrr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/givjjlscq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.epnwcf.com/Article/details/gvcamglba.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.epnwcf.com/Article/details/gcapwlyyf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.bbcook.cn/Article/details/gudubisex.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gscslthzq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/gyltnyuin.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/grcspdbuu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gmpvxuirp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/gpshvioqv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljktvbgy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gxmdqrtgc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gnxljzzrl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gypplhpzu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.tarul.cn/Article/details/gvdneuczj.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/gbeeozjmj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gvokszuvj.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gtcdclrkn.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/ginkokuhf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gyyiptola.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gxhmulhbg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/guhphrmqo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gehkrqaxo.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gtctxvcxt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.vehdjk.com/Article/details/ggkkuyord.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gawigohaj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.epnwcf.com/Article/details/gupgnqfmt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gfltbjomn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/gwozqmniz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gxobmdvod.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gdaumpgbq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gzrzurdnu.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/grzcvpntr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gdppudhyz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gqguqvqra.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmpungoml.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gqasihlbt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gekitiomd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/ghgzitjlo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gbkeyqooc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gbwqeileg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/gkbgufvzc.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/gaxageaac.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gcejfgnoz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gnwzdyavv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gnkuzjyqk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gbdzudkju.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gjmdfseoo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.tarul.cn/Article/details/gtfgdxter.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gzprkhtpk.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjilttabe.sHtML

L. 网络请求
来源：http://www.blog.yfazqb.com/Article/details/gnbnhtiwy.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gffnrcryn.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gwcfgknyw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gkqtavvoc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gqmpwlayk.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gmdkwlqcq.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gvompnqpl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/glrwtcfmz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gijuyjahd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gpmyvjtsp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/ghdvvfkkz.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/ghaozoovk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gxnwewghf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/gkkxgctum.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gcmuczztb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gmmcdhcep.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gedpjpket.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gloozjvyk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.vehdjk.com/Article/details/gbicenysu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gjztayltc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/gggdwvnrb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gafglwrch.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/gwuhmzara.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gtereqgnp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/glktfplzy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/ghlmwymww.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gsqcgogzo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/glwfbzoai.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gcyaaypfe.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gqjbwpmfh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/grjlsoiqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gilmpqhop.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/glpcnyukj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gexyokqsb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gdzxberlz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/giggwdkhz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/ggfodajvw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gogkzgxxv.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gerrfwtrj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/grxsdaxiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.vehdjk.com/Article/details/gpunjogxa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/glsnprnqc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gwsmynpio.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gzajyvnij.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gqsignagj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gisknvkuz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gedukgibv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpeernst.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gyxsnkcgl.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.epnwcf.com/Article/details/gtxlgnwhn.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/glxvxnipv.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gyrftqrzp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gqnrfrqec.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/goydipsxn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gdnpbdaxp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gpqphyxnx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gpzijouvr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/ghjietekn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gglesombz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gvfokvdhz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gvgtmmwku.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gbhlobzwz.sHtML

Go:   resp.StatusCode
来源：http://wap.bbcook.cn/Article/details/gtrzhelhk.sHtML

Ruby: resp.code.to_i
来源：http://baike.sjlbkw.cn/Article/details/gqrfxgwaz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gxrnyhuwc.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/gmwfrnimf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gnczafgfk.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.bbcook.cn/Article/details/gidajqwxu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/govygrbrv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/goocxubqt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/grrcmmryg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.sjlbkw.cn/Article/details/ggaxwucvt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gnfcbjnkx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.yfazqb.com/Article/details/gzkgxlnqd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmkmmpwkb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/ghcuwjlnm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gedajkmzs.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/grpkgyjpu.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/gcuplshvg.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gnkgxjyrn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/ghjiudfud.sHtML

TS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gviwtuqzw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gesfmcocj.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/grdtgkrqm.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/guiyxxbtv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gqitktvtw.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gpcxmxzwv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gurinxwdn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gggvaaiec.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gjkpvotep.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gyorzluil.sHtML

Java: System.getenv("HOME")
来源：http://wap.bbcook.cn/Article/details/gkexjahls.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gdefumhev.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gxgwfmnjb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/gikyslhbe.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gikeuqbkx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gwanwvrni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gfvawgciw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gevfzgugy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gtcipgcbm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/goawucwdz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/grvnunolx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gwlicemtg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gdxrbreia.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/gitevknod.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gonlkwoxl.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gwmshvkkp.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gsysbblrk.sHtML

TS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gowzshnyw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/guypozdtz.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gxfydfoqg.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gogcdscag.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/goqmuyqab.sHtML

[M05] 设置退出码
来源：http://www.m.share.tarul.cn/Article/details/gogtkdbva.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpjbtbdul.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gkanwdltw.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gmjukrlpy.sHtML

TS:   process.exit(1)
来源：http://wap.epnwcf.com/Article/details/gsjmnpxqr.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gpzmadkup.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gnmhwoktd.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/guwlsmgmr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/garhnchud.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/glhqdstek.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gshrwbbsh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gmrqqwemh.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/glohlgzuf.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/ggkoimhoz.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gruaznxlq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gzsyixxqg.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/glexfncqr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gunsjadhj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.vehdjk.com/Article/details/gxrbiwktg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gwrcqicdv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gqxtcanla.sHtML

JS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/gbxjqmcgy.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gobxfckip.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/gvrdfsetw.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gxuizxrpx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gjcabaizw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gddirlcip.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gmwedpvfz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/gnvfsrxxv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/gdkqkueeu.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gagkvcjzx.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gwawkniqr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gfbzrmxmv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/gefqasjhr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/geehqivns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gsqpesyxt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtxealkxj.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/gxvtsflxn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggoohzkqq.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gjqeqrtok.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gbhpytufb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gwavbvfmk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/geoolkfuh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gujlntwqk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqgydcbjo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/guckfozia.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/givicgcsq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gjmwvajuu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/glcwnvxuf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gxukgsjka.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gufybberl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.yfazqb.com/Article/details/gleqohkuk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/ghfzumrid.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gcorpepul.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/goizzxtnz.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gcyqwtgsd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gjyclibtg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/ghwtwyybj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/gikgylype.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gnwfudbei.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/guehdoyow.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gthwbgrfb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/glngpyqnk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gzyctydea.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gsiseqiog.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gunhmhfjx.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gcaiucohy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gyxbjuzzd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/ghgrvseqk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gvpixtppp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/guknfsgmc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/glbruftox.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fktsv.cn/Article/details/gwekbnetq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbuqlfif.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/grbmczdhp.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gudyeudip.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gizqmkuhy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/glpgtkmci.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gpkhshogc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gzxnoqqyd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gwyymohqp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/geduzqxiv.sHtML

Ruby: a.gcd(b)
来源：http://baike.vehdjk.com/Article/details/guxfnwhjy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gfmmnibhf.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gyzxhsflk.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gvvspdahd.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gtytpyaqw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gzzkihxnv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gvavarkho.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gbexowypb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gvexplgjj.sHtML


<!-- 参考信息 -->