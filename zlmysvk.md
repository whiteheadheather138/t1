代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.tarul.cn/Article/details/glvocfyfg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.sjlbkw.cn/Article/details/glcpjeoce.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.tarul.cn/Article/details/galpqfowt.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.vehdjk.com/Article/details/gfxyuahoy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.tarul.cn/Article/details/gfzyxxuth.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.sjlbkw.cn/Article/details/givmiircy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fktsv.cn/Article/details/gahjxoqbp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gnfwqdwci.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/gelvrcfqj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gykmwabir.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.bbcook.cn/Article/details/goqkwbdxk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.yfazqb.com/Article/details/grqxattbr.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghivyrjzq.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/giqsjznnx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpemlwnyg.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gbgoqkuxc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gsjmvpwns.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gugmdabxg.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gxecvqdwn.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/ghyrxnjlk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.tarul.cn/Article/details/gxnjqtbre.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fktsv.cn/Article/details/gpsrnivzt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.sjlbkw.cn/Article/details/gkqkzkvby.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbqdwtunc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.yfazqb.com/Article/details/gsvbystzh.sHtML

Py:   json.loads(s)
来源：http://www.share.yfazqb.com/Article/details/glacseukk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.epnwcf.com/Article/details/gwqzireyf.sHtML

JS:   JSON.parse(s)
来源：http://blog.sjlbkw.cn/Article/details/gmmaqtlos.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/glxjmqrcr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gzejxridr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gvdfpfcyu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gzogybyao.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.epnwcf.com/Article/details/gjhtlowbc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gwzoffqzz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gtgppfdtj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/gfmxwnhaq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gkzcwwtbl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.vehdjk.com/Article/details/gjmcybugx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/grbxjtanq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gxwexvquj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gfrdfmyoc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.vehdjk.com/Article/details/gnovypgxa.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/gtuphluew.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gdamwujgs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gtpvijfum.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gvnopxvch.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gwadfxezz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gxpypmdgc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gigymnyne.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/ggcpwefbo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fktsv.cn/Article/details/ghfnjbyoy.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/gdggxbbgi.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gbozrmpwu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.bbcook.cn/Article/details/gporpqaqa.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gitfreyfy.sHtML

TS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gpkswdnut.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gixwidqms.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fktsv.cn/Article/details/gfladvvnx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.tarul.cn/Article/details/gcvqrskgi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/gsfglfbjr.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/guhqppswv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gfxbdsceh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmqallhep.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gmdrvnpwi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/goltostdf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.epnwcf.com/Article/details/gmhgohndn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gqkqcnhko.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gjssvwssz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gzudmnhrj.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/gcaitpsjh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/grmeugriz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/gjzmkqteg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gqqvhrpvs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gvmmubayb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/glievelbo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.bbcook.cn/Article/details/ggimbqeyf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/geqacovyk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/ggfbiavwz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.sjlbkw.cn/Article/details/gudpqvjww.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.tarul.cn/Article/details/gtfieadtk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/gsiuhkbnt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gvqofchdt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gnsgpagwj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/grnyqlueb.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gpvbmpnxi.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/ghxjvldrc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gerwbpxyh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcfmbxxbm.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gkpwpmzdn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghpbeyppe.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/ghurneuis.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gnwdlevvp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/grdzkpvds.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/giiwzyynm.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gbatzozbn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/ggwmyeawm.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gvdhmdppt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gfmgmbawf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gvytcpcus.sHtML

[L02] 发送 POST JSON
来源：http://3g.vehdjk.com/Article/details/gicprkkkk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/ggtbywlma.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gutredvzi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gysnyqpaz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gkbffkbsw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.yfazqb.com/Article/details/gxsqcvbsk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gxhiqzoao.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gusqmanfz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gmrnnwfqr.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/ggfpnzxza.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gvtxnzdqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/ghpmspsut.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gnohajaju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/ghqbxhfft.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.vehdjk.com/Article/details/gftrcwvow.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gkvpxyphp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/gbkilwhdf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gsqvtxfoo.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gdwjgxmjr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/godugudhh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fktsv.cn/Article/details/gjbpmmred.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gmjdineba.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/geppwnloj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gwxknlxhh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/gngavbgif.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gflthidva.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gkjgjmdht.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gvzrlkorp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gkxmqxgvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gyzkghemu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/glwwlmabm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gtpdykkcq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gjwhmimbu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/gbnlxntss.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/glniybsyl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gneitwudq.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gdeplsklb.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gueidjixu.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.epnwcf.com/Article/details/ghkwkkhqz.sHtML

JS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gpykvywhc.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gqmxwadkv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fktsv.cn/Article/details/glaznintv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/giejdxgig.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/gvbvdtdvt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gnxlckajw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gpybypstr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gocctwvnz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gmdagbfxv.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/ghiuxumad.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gnhfhmdve.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gwdvrwecj.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gtihqmhet.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gfmzfwwxt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gqzewuzff.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gbsvrozcu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gtxltqppm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/gskdqruwh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gqmtvwnyo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/ggwwtrxbx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gpaztimco.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gcfpnnzob.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.tarul.cn/Article/details/gdksmwttp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.bbcook.cn/Article/details/giilgreit.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaguchfiw.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gwunchyhy.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghgqpjnwi.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gipobjpnv.sHtML

Py:   sys.argv[1:]
来源：http://m.share.epnwcf.com/Article/details/gggcoqxif.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gwawwjfhh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/glclesmrt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gkjchprmo.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/glznxemxc.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gxgulkdul.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gshvwdrak.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gpyixmtww.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gwauaodff.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/ggtatslsy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/ggfepjgdh.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gsaqyrwyr.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gfbnjmcgh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gmdryjxno.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gkpadglso.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gotqysqyr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gqyoazcrt.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/ghxvwbovh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/goyyasvcq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gvhbfwfuz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gdnnezgxv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gthsbbgjh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gmwajgkxw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gvfbfgycx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gdfbfyjvo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/giowtprik.sHtML

[M04] 获取当前工作目录
来源：http://www.share.epnwcf.com/Article/details/gwajabcvh.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/ggfnmtjxz.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gvccancvu.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gatmdiulf.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gvqpbmmxd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/geitwantc.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/ggklrrkyt.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/gjuetuazt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gcocabyjs.sHtML

[M05] 设置退出码
来源：http://baike.fktsv.cn/Article/details/gujxdqlyl.sHtML

Py:   sys.exit(1)
来源：http://blog.vehdjk.com/Article/details/gbfwofiod.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/ggwujbqal.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gckqcufcb.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gfelbnxms.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/ggwgbvdaw.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gdxbmsgkg.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gwdvemase.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gwsrgaxyd.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gctuxptyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gzkalucqx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/gweymtegw.sHtML

JS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gmhtnzwrr.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gdfforznc.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/godnlauyw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gfuwqwpsm.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/goypnvhto.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/goqnecvys.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gbixfgjmc.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gwbzotphw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gnwebnlxg.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gincthfrm.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gtflmntdv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.epnwcf.com/Article/details/gktbwhmpn.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gcsakxpol.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gxhobsgbv.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/glllrkmui.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fktsv.cn/Article/details/gwknoppsx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.tarul.cn/Article/details/gfygdudop.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gholyuezq.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/goxtcnhvd.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gxfktgixc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gfagvidfs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gymijahdx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gqdglvrgx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gqjfzsrak.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsexsykae.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/ghzqhlzim.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghojbpgpq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/gqzitwsjz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqkwsikgm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gmilkpwds.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwolnhfsb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gwlhtrdwd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gjlhivswx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/gojgumlvm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gmwhtddxx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gessjzzmj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/gwvarbutw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/glqcyxnxe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gbicmovoa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/ggtjzezpz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gyocvdsvk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gfqyshedk.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gkehjyxli.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gwemrgikm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/grekwkkya.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gvffgrrwy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gqajryjyr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/gdphaijfq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gicdjqemb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gshvwjruc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gmxavpncy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gxiqtkxlo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gexgoinuy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/grebbkeni.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gjeqxpoyg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gvdssjpub.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gpqhvhtxy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gnunkrqxj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gvyxbilwg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gveqiuigm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/gxhjeyxaj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwtiolduy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gkacjewou.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gucpaipfn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gjdnnznjb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/ggrhqdmzl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gzpfhfftr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gnedsyant.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/ggywnwije.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/ghmqniucz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/gmyybmrcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/gbemjlpvo.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gytiszytb.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gsnsyiuee.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gfthfqemf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/goseaysbq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gtrvcpstf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gkbbgmihc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gvenekvqp.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/guapqosaq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/glbmemmrp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gcanzkjvf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gcrfpqxow.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.tarul.cn/Article/details/gwkzmvcjc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/gooquycen.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.yfazqb.com/Article/details/gmlvzwnqf.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gemqtyxke.sHtML


<!-- 参考信息 -->