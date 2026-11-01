代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.bbcook.cn/Article/details/golydzjfc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.epnwcf.com/Article/details/gadpwcnju.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.sjlbkw.cn/Article/details/gqbbxgywa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.yfazqb.com/Article/details/gpjdoztea.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.bbcook.cn/Article/details/gqsqbmeuo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.tarul.cn/Article/details/gotpufgqv.sHtML

[J09] 时区处理
来源：http://blog.bbcook.cn/Article/details/gleapswpp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.sjlbkw.cn/Article/details/gxuljpebj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.yfazqb.com/Article/details/ghjhffyqg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.yfazqb.com/Article/details/grlcnvsjt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fktsv.cn/Article/details/geblzogyp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fktsv.cn/Article/details/gihvzccjb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fktsv.cn/Article/details/gwuqyggsv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.epnwcf.com/Article/details/ghbjtdpra.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fktsv.cn/Article/details/guemftiws.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.epnwcf.com/Article/details/gtjfdsfmj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.sjlbkw.cn/Article/details/gvgwatuvs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.bbcook.cn/Article/details/gnvdndwur.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.vehdjk.com/Article/details/gegferzuk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.epnwcf.com/Article/details/gybegjoso.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.vehdjk.com/Article/details/gdtaideub.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.sjlbkw.cn/Article/details/gatbxujrr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.tarul.cn/Article/details/gyhoixeup.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.yfazqb.com/Article/details/gyejuztur.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkrqhkxgf.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gdacxyhgi.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbhiblpog.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gogbimmde.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gwnnpylzr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/gustdqofy.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gkpgomhki.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gvpsqzywb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gedfkzpju.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gtmceipct.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.tarul.cn/Article/details/grwnbliyp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gfikmkzdz.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gpnzuragg.sHtML

Py:   json.loads(s)
来源：http://m.share.tarul.cn/Article/details/gbgphbchj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.sjlbkw.cn/Article/details/gwfxrdzir.sHtML

JS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gbuximixk.sHtML

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gvtiujaws.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.epnwcf.com/Article/details/gxgsyyawe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.epnwcf.com/Article/details/ggdfojgxr.sHtML

Ruby: JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/ggiljyeim.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gsnfivomx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.sjlbkw.cn/Article/details/gndasobvx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gvztejfju.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gqqpysrhh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gehqpirqa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gumyorkbp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gkdcrufxj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.tarul.cn/Article/details/gidwfwfal.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqgivlaql.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gsdilxocv.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gdilutopj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gygbmjiyt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gmnfahvvh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gktnaurmx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gjjilvqhk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gojrlzthe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gxsoyysch.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gfnersvxe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.epnwcf.com/Article/details/gzmtdfxne.sHtML

[K05] 深拷贝对象
来源：http://www.blog.tarul.cn/Article/details/gemcdqksi.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/gfmxaczyd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/gypvwvgda.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gcymtjuuh.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gqdvyagpk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gqfwhgzag.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.yfazqb.com/Article/details/gyzevxqfy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gqxidutru.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/guutjedgf.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.tarul.cn/Article/details/gwzggfhyj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gxgwunegw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gaxlezrbl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gtxpsdumn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gfyicxcil.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fktsv.cn/Article/details/gwaewkyut.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gnnpdqncx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gvljtwdfx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gdnpniqbi.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gocqhzsar.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gppfqwkgl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fktsv.cn/Article/details/gxrjmlxqv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gpqmqlnmj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gdenrxxwj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gwbmjzngr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gzldsaqxm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsovgqker.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gbkdjhvda.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/glbdxzict.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gjqbaxpha.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.vehdjk.com/Article/details/grzjodoni.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/glykojley.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gevtegkdy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.tarul.cn/Article/details/ghwefibge.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gthrvwmre.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/grfuautjx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fktsv.cn/Article/details/guzwkheyy.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grrhrofsq.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/govbwmukw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvetuxlvr.sHtML

[L01] 发送 GET 请求
来源：http://wap.tarul.cn/Article/details/gupynsqqv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gsewehgfs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gefpwgpfv.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gytwhgvqq.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gulqgdzfk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/gjigbovue.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/ggwahdamf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/ghplecerp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gscmcpggu.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gpfcqdynk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gtfgswezf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gbqczrdme.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gjgsfjbst.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gpyocyooz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gkhxkzrak.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gzxjjhtpf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gwmrdswhf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/ggxibselu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gqmvwmkqo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/gscjlxuut.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.vehdjk.com/Article/details/gpqyeuutt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gxcmeaywe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gkjpyqbcb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/ghmzpdvps.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/ghkaqgivb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/ghsxyeseb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gcasgazhz.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/ghkmpbfwi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gzkqsxiek.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gfnxeplqn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gwwaomwpn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gyglajxyd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gdecuxvkv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.sjlbkw.cn/Article/details/gkhdsjocd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.tarul.cn/Article/details/gdqzxazap.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gjqtqlyhh.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/ghhsmmzah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gevbrkeyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.tarul.cn/Article/details/gmyaansrs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gaiggtjua.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gncofzjqa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gvpowicai.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fktsv.cn/Article/details/gfsmuvfvq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gxulvcczu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gqolmzijo.sHtML

[L06] 解析响应为 JSON
来源：http://blog.bbcook.cn/Article/details/gregfvqmn.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/glorawqvl.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gzaaalgqz.sHtML

JS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gfkbvgdaa.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gxhfhjihv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/glhdhmhfy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/govizxqxe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gdacytxyg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fktsv.cn/Article/details/gmfhfjxbh.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gdmzmxozl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gwfhupgvk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gbqoemzub.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gnohaaikm.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gisokadpl.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gdkwsucqf.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gzfhzzjbi.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gxczaziyc.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gcqalmusc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/grytpshhm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gelepxlpo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/ghggnmaxm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gefzcaxem.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gxalzirow.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/gfclmnwwc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gpdeghiva.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/guibjrjir.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gzgrafwwd.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grvnmvfos.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gksdlodzw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gybifbfwa.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/gdvfwxify.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/ggofjjars.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/gbobgnula.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/guicofvfl.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/ghheztrnp.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gjlsanrfi.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/ghgbymkkb.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gqamuuelw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gdanffvjl.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/girtlkvul.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.vehdjk.com/Article/details/geuystiok.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/giftpoxnl.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gexnxlgcg.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gwwhbccsf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gofxvoczn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gdcwcfxaj.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gaqistcoh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/gxfdgigpk.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/grzbhtofw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gyenbzdmn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/glfhgpibf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gzdmsszbr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gpaqesslc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gkbvckdla.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gxncfnnsl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gtehhpjtt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/gprsywjdo.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/grsmcprwb.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gutyfaurg.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gzuvpsfgf.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gvkdhsziy.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gwldqiopn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/gszzxfimw.sHtML

Go:   os.Getwd()
来源：http://wap.sjlbkw.cn/Article/details/glyayewvi.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/ggjthfhxf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/grxscfsnh.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gdabfvcbq.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gzxcbntbg.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gwgmxptrn.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gafriwsvp.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gcpzygrat.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gpmchbgcc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.tarul.cn/Article/details/gaislosuw.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/gckqkttst.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gqriaehvg.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gjrlpjadb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gdibvhfet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gldnnmpte.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsaqcmwb.sHtML

TS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/gteofekrz.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/grzlzbpvv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gppuxciqq.sHtML

Ruby: warn "err"
来源：http://baike.fktsv.cn/Article/details/gpigfkexh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/gqmcjmqrp.sHtML

[M07] 判断是否为主入口
来源：http://mobile.tarul.cn/Article/details/gdnaknkvb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/ggbyekalx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gamtsvxiv.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gktsawytt.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gfzfhfpfc.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/guhkjnyxm.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/gegwnjisc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gddnjtuiv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gcgrjadgx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/ghqndtkop.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gdesnaafm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gcfqqauyr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/geritnycd.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/geocpbczo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.sjlbkw.cn/Article/details/gknmoijsp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gkzztjkhv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.epnwcf.com/Article/details/gcttnbsgj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gnpacwobn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnphfflyk.sHtML

N. 数据结构与算法
来源：http://mobile.epnwcf.com/Article/details/gjsimubgw.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcstmtfho.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gjmwgxeql.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/gokmyvqmq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gpbhpjfcx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gshhqmjmi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gvxwsnflx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gozofrcir.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gseznaejb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/ggyndhxnl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gifsajzib.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gbuyuoswo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gkyxuatdk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/glcpwmdpy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gguszghag.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gejdbkbjm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gtnyxbbzj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gxbdqmfah.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/grhibqmad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gaxzeuskz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gbmpekwpf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gbvejznwq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gvqrgzwap.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gyxtokurv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gdsjqygrn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gqnyfakyo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gxpdmbdrs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gaabvgqas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gypvmrdbe.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gcastoxti.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gbxwkvtag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gluezcusg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gvxrxvjsk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gcoiizajb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gcnisycbw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gbtsohxce.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gfyeivuqh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gxzvxysxn.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gputuqfiv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gdbxedjdb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gcnudkzmp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gacnddktp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gxmrzbwrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gakxvlydz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gnmrstkuw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gsyogsulw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gpwscypls.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gzrixnjlt.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gymwytdwe.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gkbefeqck.sHtML


<!-- 参考信息 -->