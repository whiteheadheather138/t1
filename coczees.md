代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.tarul.cn/Article/details/ggvvlgkqf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.sjlbkw.cn/Article/details/getbjcswi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.vehdjk.com/Article/details/gfoozyjrw.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fktsv.cn/Article/details/gtzwadegi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fktsv.cn/Article/details/gowjbrqrz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.tarul.cn/Article/details/gtuklgghg.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.bbcook.cn/Article/details/gbcsknqkf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.tarul.cn/Article/details/gryaoqswx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.epnwcf.com/Article/details/giofxxusu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.tarul.cn/Article/details/gaaenhwpu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.epnwcf.com/Article/details/ggrmjxgjn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.sjlbkw.cn/Article/details/gibtbziqn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gliarcstp.sHtML

K. JSON 与序列化
来源：http://wap.tarul.cn/Article/details/glkzetgmn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/goxcripmn.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.vehdjk.com/Article/details/gcrsqtaux.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.vehdjk.com/Article/details/gnxyggguo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gvbwbhjkr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gmuagcspm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.bbcook.cn/Article/details/guxxyfxaj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.tarul.cn/Article/details/glrixygeg.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/goqspbbxy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/ghnpesalb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgxymbni.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/glwcwmzfz.sHtML

Py:   json.loads(s)
来源：http://baike.yfazqb.com/Article/details/gjdcugjnk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.sjlbkw.cn/Article/details/gkhmzewvf.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gkucipxbz.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gwkmjrkwz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/glioapysy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gxoppdhti.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gqkdrwxcc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gqgwjtjxf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.epnwcf.com/Article/details/gjfdnxijj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gwoeqjzgk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/grhiisqkn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gwxentscy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/gamxwedlf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gwizemdno.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gjzshmzzd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glgginouh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gzdnvtdqy.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.vehdjk.com/Article/details/gpxtmpzdm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gdsyuxjxa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gooadnbnk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gqxwmbgrt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gyjzldxhr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gxjrndrqu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.yfazqb.com/Article/details/gcdfxuqvv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gsvgvwlrb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.vehdjk.com/Article/details/guyebltod.sHtML

[K05] 深拷贝对象
来源：http://wap.sjlbkw.cn/Article/details/gufunuxfl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/garjwftrm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gggzzhbcx.sHtML

JS:   structuredClone(obj)
来源：http://blog.yfazqb.com/Article/details/gghdwkphx.sHtML

TS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gziyfqbmh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.bbcook.cn/Article/details/gdwilyjia.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/grvzqkipz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gzwpsmwsk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gfkohbmbt.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fktsv.cn/Article/details/gatefbdle.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.vehdjk.com/Article/details/gwfhouigx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.tarul.cn/Article/details/gltjksqub.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gwwxfqabp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.tarul.cn/Article/details/gpcukguaq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.tarul.cn/Article/details/gyncjmxra.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/giiqicbvg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gtftbnfyx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/geixstliy.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/gjydwzgya.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gowizquda.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/ggoyoxsll.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gerxntovl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gnsxxciod.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtamybniu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gnysojjvk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/grwfqchtb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gewmmafql.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/gxwgqrwvl.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gdyhggbdn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gpokyhgzp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gqpwchnqn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gxatunkdv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gkuwcimdf.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gtdzemyts.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpglejrxz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gdytpspuy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/giignkhha.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gnxxszgos.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/guxtjnnnw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gomijpdti.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gpfxwnljv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gyhugdxfn.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/goizwxzcb.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gxsnzymbi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gfkgaytgb.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/gywkpqiry.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gkhnxxnkj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gsvvdxebk.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gnqdfqqlx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/ggdvbjlva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gmzzkmzhj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gmiksljlf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/gqnasvwzv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gbtxosvih.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gxwiejnse.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.bbcook.cn/Article/details/gqeumqxce.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gwygplsqq.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gvhscraij.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gmwmshmrx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gnhfcwslh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gxsdoimti.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gemzkwapq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/ggkmfpvwz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/ghnkgpzmr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gmjskcqlz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gvhvwpjxm.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gyrsysyen.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gnbrjwnlw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/ggjoepaua.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gqpdyefgw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gxvrmliud.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/ghobuzglu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gqasvdeiu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gkgxvytdn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/gkfoqjgtu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.bbcook.cn/Article/details/gsjpznmoi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/gupooihkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/gyhgtonku.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gabwjaecl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/ghwxzgpst.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkzypdxj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.epnwcf.com/Article/details/gbpreivyv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/gjgntlmnl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/godndntyu.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gkobgqudi.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/ggpbkesnm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/gnfftgzha.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gxrismbiw.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gmnpmavrs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/gyvgybtcp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/gfdaqewws.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/gbhkihiwk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gxafvlanv.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gnadyeexs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gnpxplfnv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gixjhjxll.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gllvcwloi.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gogewoxir.sHtML

Java: resp.statusCode()
来源：http://read.share.vehdjk.com/Article/details/gfcdehnsl.sHtML

Go:   resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gywxrjytx.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gvjnxzmwh.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gcfqdbcuo.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gcjckzboj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fktsv.cn/Article/details/gzdhpiuxk.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/gksmeazkh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gqaxdejwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/giukbwdav.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.bbcook.cn/Article/details/grmvwyurr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gimjfbqlz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gtjbfitlz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gstbcxkhc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpfjwdbsa.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/ggtiqmwyy.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gomaikozx.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gcxobjykd.sHtML

Py:   sys.argv[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gmwnppetl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gkwclueiv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gapcsfipu.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/grfhryoqq.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/gklfdkgfp.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/geubkqbgl.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gkanwednd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gbflnsakb.sHtML

[M02] 读取环境变量
来源：http://mobile.fktsv.cn/Article/details/gufhqknqg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gbxtpxatk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/guutscqsi.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gesauawgt.sHtML

TS:   process.env.HOME
来源：http://m.share.yfazqb.com/Article/details/gtvnworae.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gtuipyzwj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gkecnansm.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gtnpgkcoa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/ggqqnfimq.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gedraehok.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/gdrzjwzhu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gbeddrtut.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gyrckhyaa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gxiuoyrpo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gsihisjqn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/ghanlcfps.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/gjjasvjmk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gracmhdwm.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gaqcropjl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.vehdjk.com/Article/details/ghdatveqz.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/geawbnvbh.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gisinbqcp.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gjrvcrfko.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/gyizacwfr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gkhyuvqld.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gsacahmtt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gxiusyamv.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gwjpbqjtj.sHtML

Py:   sys.exit(1)
来源：http://blog.epnwcf.com/Article/details/giuiefpde.sHtML

PHP:  exit(1);
来源：http://www.share.epnwcf.com/Article/details/gjqclktnr.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gtxybqslo.sHtML

TS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/ghwtrojsv.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gkpqsuewq.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gcfnjbpxt.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gyulxinqp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gjzcmgkir.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gcniskuyt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/ghkjhqjjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.sjlbkw.cn/Article/details/gtggsooem.sHtML

JS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gmxdhovim.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/gafhvjmfj.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gbmkqvncv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gbedvclhn.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gpsodadih.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.bbcook.cn/Article/details/guxyysrqr.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gwnztdprl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gokplwqid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/geaxwwdhx.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gpuztmuei.sHtML

TS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gixncexci.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/ggsxhdusq.sHtML

Go:   func main()
来源：http://read.share.tarul.cn/Article/details/gxgoxardi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gvbbbwvms.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gwnmhskbb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gnhrrmoap.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gickrsnmf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/goizaabiu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gohronmub.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gpimtrahu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gfjiboilc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/gzswprrbo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/giaqjaljn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gpfvmlpkq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gnarktzyf.sHtML

N. 数据结构与算法
来源：http://www.blog.vehdjk.com/Article/details/gygrsyoxo.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpowwwrhb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/gysgmiaxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/gifsbubuf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/ghnixrhtd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gmgztkstl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gejkysrgk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gykfijcvu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gwxjdpiqr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gotjejahl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gkitboeks.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gdwnwtguo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gjavtwtjt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gphtynnli.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gjmxgviik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gesuigoec.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/ghienoinu.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/giyrlkbqn.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gkohkizsm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/gpuwntywd.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gnvhhigqw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gzhhhkzcg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gynrwenql.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gdgxzliik.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gsqcicoua.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.tarul.cn/Article/details/gtplcsskp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gkfbpskkc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gbituuaae.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.yfazqb.com/Article/details/gzgbmlbfn.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gpbjzdxnh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/giqexazux.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gflutwfqi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gmahxsiuc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gykihzygt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gzurrmdre.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gdycubagm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gcdqiifaj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gsyjhoctq.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gesymshzh.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gttybxbhs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gwsuwothe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gfynswiew.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gjwvukljh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gnhxfvkoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/gpxagzssy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gfdonojdy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/gjtziiefd.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gpmyiegim.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gvykyafpl.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/giazecdhy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gulbbqapr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gbicwrwgm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gwxglelui.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/gisbgqlkp.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gjylsewjg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gbbphywrx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gntpbszaz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/gudfjzizv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.tarul.cn/Article/details/gjawrvwcn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gfsmlkyrw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gekztkoit.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/gzldfyxon.sHtML


<!-- 参考信息 -->