代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.sjlbkw.cn/Article/details/gjwhwyrpp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.bbcook.cn/Article/details/gbcyjcrwy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.bbcook.cn/Article/details/gibjeyhmp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.bbcook.cn/Article/details/gnttwjtbz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fktsv.cn/Article/details/gorwqmjah.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.epnwcf.com/Article/details/gcwasnzvs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.epnwcf.com/Article/details/gebowccqk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gmvnaugyc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.vehdjk.com/Article/details/gbnkgotyu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.sjlbkw.cn/Article/details/gfsjaxjsr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.epnwcf.com/Article/details/gxbxeekre.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.epnwcf.com/Article/details/gtvvcdubl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsrjihkck.sHtML

K. JSON 与序列化
来源：http://www.m.share.fktsv.cn/Article/details/gndsccvob.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glsvyhfir.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/gekmnmfey.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gpgnwgddw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gbkyxevmc.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gcftorxns.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.bbcook.cn/Article/details/gixtuzrvp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.sjlbkw.cn/Article/details/gssfdayqf.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvpjrmneh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.bbcook.cn/Article/details/gcioacbei.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.yfazqb.com/Article/details/gfiruwnkw.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/grxuyhbia.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gbppmmcuc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gzhwnuhbw.sHtML

JS:   JSON.parse(s)
来源：http://read.share.vehdjk.com/Article/details/gojzmgxfw.sHtML

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gbkpxspbc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/grfgojywt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gauaafnkt.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfiaguxre.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/glrgjkofa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gxihnokti.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/gttcszpwd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gpcootcrp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gnnyhxcyx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gcgdekwij.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gwdtqcexl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/gvpgijxfv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gyfutgxvz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/gybnrrpmz.sHtML

[K04] 读取 JSON 文件
来源：http://3g.sjlbkw.cn/Article/details/gcxbgvwmv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.yfazqb.com/Article/details/gowsaydzx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gsbmtwgqt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.tarul.cn/Article/details/gvmvegrje.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gesybyoto.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gjcromige.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/glgvhsnnj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gdpnsdnbo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/gpyqojowd.sHtML

[K05] 深拷贝对象
来源：http://3g.fktsv.cn/Article/details/gxfgnjncc.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gqgincnjy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gcxrkfiaq.sHtML

JS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gcmyeypcp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gqiopekdl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/glkvrxwxk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.tarul.cn/Article/details/grlfymdjj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/gwzfzmgej.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gxdrueqmk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gwvobxlqy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gbglfjejc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.tarul.cn/Article/details/ggnvcryqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gasvxbmrn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gpbxemslf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gcvjdqnyb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/glymwzgnp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/goehdckgl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gfolssgch.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/ggfkzmfbr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gqdvasltc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/gynlunrtu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gynbgniff.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gdenfzjlo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gfidhtxkk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/ggcfifdnh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.vehdjk.com/Article/details/gakawhplv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gubwwjeva.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/gnxnkvldf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gejrtvnta.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fktsv.cn/Article/details/gtrdpigqe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/geexsmwig.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gwnfqwahg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/grnoazasl.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gzpazavhd.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gljjwkiza.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gvouskjvt.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grvmsqirr.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/gaqsmordv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnpldnmku.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gwuatfjfu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gqjeevcqv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/grgosgytg.sHtML

JS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gojkldphc.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gcopougyt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.vehdjk.com/Article/details/goyesxpoz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gdvwscdjx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.bbcook.cn/Article/details/gozjokdhe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/grmywikkq.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/gqsghgvec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.epnwcf.com/Article/details/gxuzfxnbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gqfalsvtj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.tarul.cn/Article/details/gxioqaqiv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gktucfwck.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/gksgjtwge.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fktsv.cn/Article/details/ghyaylqvd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gwuspxlpj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gonrogeev.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gixzlzgol.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gyvgnooks.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.sjlbkw.cn/Article/details/gooclxzpy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gnkkfjnxq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gnrzeizdz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gqxfbqwsx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/guzypwaft.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gpofvecho.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gchoswrya.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gbtokphmu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.epnwcf.com/Article/details/ghwrsyhgz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.vehdjk.com/Article/details/gqyiomcho.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gjprsqvza.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gjjbncydj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gnngqpyau.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gefvtqnim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gxmxqpymf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.epnwcf.com/Article/details/gjaghpzar.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/guamzwjfm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/gsvcnotmo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gucpkjpwk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gztfyrqmv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gxpnswvyr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/giczjblvp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/ghzdnmimw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gibbcnzua.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbucdqaav.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.vehdjk.com/Article/details/gpokmpmhx.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gxdkuzdrq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/greftwlpk.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gnaijnxkt.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/giwjxcart.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gundipyif.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gjzflhizw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gmsrnodhn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/gbhnqkrra.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gragwlopb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/gwvtvemmq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gnetxqpfv.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gjhgjdkoc.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gqfojpqsy.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gepwttqsf.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/ghebrmxie.sHtML

Ruby: resp.code.to_i
来源：http://baike.bbcook.cn/Article/details/gtyeodwle.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/grefwwpvh.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/gceftbdil.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/greouwoev.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gplhikczh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gblpsdtzo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/ghbnilquw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gtwevolww.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gcffnszsq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gkoelwctc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gaxnigtqf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghwpctelj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gnesddakb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxifqgmfy.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gxevgdnfv.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gksjgwlba.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/glyosakxv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gawanbqgb.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/glghoevdw.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gyamtrmgx.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gcoahrjfg.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/guctgeudf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/ggzupzbhx.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gajzhnugi.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/ghwdphmxr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/garaobdpt.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gahhmvjfx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gtmcfhnjn.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gkbsxbenv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gsybkarsm.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/glgesynvh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/gxcnruhvw.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gbtcqhmgs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/grcmkvwlm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/giomiuwlj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gudmsbkxr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gwkaspzfd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.bbcook.cn/Article/details/gggbdudjc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/gitpfynwr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/gfritifvf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.epnwcf.com/Article/details/gyvpytyqg.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/gigzywqmq.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gsjwepzvb.sHtML

PHP:  getcwd();
来源：http://www.blog.yfazqb.com/Article/details/gefdpesvr.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gevcavkjg.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gviolikaa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gatyzdlcv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gxfhqjuum.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gyqbtxlou.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/gakekdanj.sHtML

[M05] 设置退出码
来源：http://m.share.yfazqb.com/Article/details/gyifuprrn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gcghmhteb.sHtML

PHP:  exit(1);
来源：http://mobile.bbcook.cn/Article/details/gkkuctoic.sHtML

JS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/guenjemyk.sHtML

TS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gyojfuqve.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gvccqipch.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gdeccarzv.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gljjouqte.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gpviimema.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/grrnijdkm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gapmsnxtp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gwibkihae.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gvlrhuwxt.sHtML

TS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gmviirsvg.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gslpkvahn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.vehdjk.com/Article/details/gyfnipyvu.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gjbqnqunw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gejoevqqj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gjifjfock.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gigwvkheb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/ghllnzitv.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/gqomshopm.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/glmzxsqgb.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gguaoaoud.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gbubvggsb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/ggmzqmgei.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gqdbqcbtg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gfsldgkbm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gqztwurwn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gxaqxggur.sHtML

JS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gpgdkdhri.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gdlqadbax.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/ggkcsffuc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/grlepztvg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/glodwfbhk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gxjnomplz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxbjytqpp.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gssqzpypp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gifjtayjr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/ghdaxkdnj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gkcdeqvjp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fktsv.cn/Article/details/gtcrgdsxp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gyjughvdp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gafqajgxs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/ggcfeeluu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gilluqhdx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gofufhwic.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gcdzebjaj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gzbqaeksk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/giiwhrwpw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gaifyfplj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gdueukdqk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/grwjptife.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gtmtkumrf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/ghubyxcpm.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gcbyzqjbo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gtcxcpagu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gsyznftmu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gkllpgbrb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gzofccpdj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gtffsfcjb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gvehuignn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/gtzmdhllg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gpcgnbviy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/ggryaluhi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gmamjplmy.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gqgjaqkgb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gopidwiaa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gvzyhheef.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gkdgufqvd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gsklahwmi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gcqzclbmy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gndvywycx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gevpxldoe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gsxrounvf.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gsgftwcds.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/ghuhymdjs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gijgrwohw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gtjrpdwic.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gdbzktbqs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gnzglmjaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/ggglygncd.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/geavqwyvv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gsftbhcgk.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gcpjxnpld.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gogrlmxkt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gccbnrpha.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gkydkguwg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gjlzmusxk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gflzntczq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.epnwcf.com/Article/details/glgyobbvz.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/girgmhprz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gbrdhccnx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gwnzadlxh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gyftyhyzu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gpfhnsxps.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/ggqcfulrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gyxlbdlce.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gttiuhsug.sHtML


<!-- 参考信息 -->