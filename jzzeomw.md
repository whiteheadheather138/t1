代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.sjlbkw.cn/Article/details/gmvwnbdus.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fktsv.cn/Article/details/gikpyrnya.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.sjlbkw.cn/Article/details/guxlrntmi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.yfazqb.com/Article/details/gyoqfcrcs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcuriarim.sHtML

K. JSON 与序列化
来源：http://m.share.tarul.cn/Article/details/gcwqvwdux.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnqaitodd.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.vehdjk.com/Article/details/gdnfunkkm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gpmbuxywl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gmwksgnny.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/girfyuhuh.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gehcwhvhj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/gsnsintoo.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gdrjrhdcm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.tarul.cn/Article/details/gflpxyknd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/geaznwxiw.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fktsv.cn/Article/details/gogurkiju.sHtML

Py:   json.loads(s)
来源：http://www.blog.tarul.cn/Article/details/gfkqlxkwr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.bbcook.cn/Article/details/gamlnltmw.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gsiopidal.sHtML

TS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gnpjhhcyl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/guxfwwgvq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gejayhvbm.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gvqjdduhm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwkyghkdn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.yfazqb.com/Article/details/gfpszqcqs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gbpkblrdv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.vehdjk.com/Article/details/guldszflj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gocdfuqqb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/grshdmdek.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.epnwcf.com/Article/details/gsmmkzybl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gkqicjxdr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.vehdjk.com/Article/details/gtylbegmo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.sjlbkw.cn/Article/details/gwxdujmwm.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.yfazqb.com/Article/details/gswkhttcb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fktsv.cn/Article/details/gecqqwinc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gtlbbxsib.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gzotxmgqk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/ghwukjghj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.yfazqb.com/Article/details/gudcbgycw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gywqzodbw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gmaixuzxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/glpnvksnf.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/ggilzrlvg.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.epnwcf.com/Article/details/gnspkdpkn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gxwaqcqov.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gswmqmejw.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gyizgtlli.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.sjlbkw.cn/Article/details/gyviwjgox.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gxbvxdsim.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gcefazjbj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gxktboghg.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fktsv.cn/Article/details/giuxebytr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/grdytkxyq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gnjkiljag.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gyewpelsi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gdbewhpdc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gdmeukqjo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gqxbsxqlk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gzeyfuqgv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gxzjvyzvu.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/gtgfqkwfl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gygccvqiw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gpyucybpq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gevnczewc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/grizehxei.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gdcuudbie.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/giyaazhft.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gyyrobipx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gwhdaxnai.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gfhytfmnt.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/ggnkkkarr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/goxidfehi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/glqkmvmwf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gzerokffw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gzpwnnfbw.sHtML

Go:   encoding/gob
来源：http://www.blog.yfazqb.com/Article/details/gzndjxxvf.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/ggwjwqqrc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/guqtezrpy.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghizntkfq.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gyxwszuyw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gudafrqyi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gwgxkcwnn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/gfwtcxcjx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gafsjsqqp.sHtML

JS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gxpbyyjyn.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/glhtjudla.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fktsv.cn/Article/details/ghzzuzxcg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.vehdjk.com/Article/details/ghxulpple.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/ggdonusnf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gkftwoyso.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gtuwslram.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gmtoevadx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/guaxgzhcz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gnoxcqqol.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gfgnmqhto.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/ggkixwrya.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gqupnakco.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.yfazqb.com/Article/details/gafrpxorq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gtrcfekis.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/ghevoukio.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.tarul.cn/Article/details/gmsrwxcee.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gccimunnx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/ghzfgojpk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gczwhpeiu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/ghjucqebh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gxdeqchtf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/ghnlfkjeb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gzdkukghr.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gmklktxrn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gzpycjmku.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gbhdgdzrd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gjaahduyc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/goeucqvca.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gicqdnzbg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/gugapfyuy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/gihsxwfvq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fktsv.cn/Article/details/gudjjgyjm.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gzubexjde.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gljdnrkds.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.sjlbkw.cn/Article/details/gxpulymgt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gkdhrkuas.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gzizdexpg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gojrqttha.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gcnteceia.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gigdctuae.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gomcjfeol.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.tarul.cn/Article/details/gtekzonzn.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gyfjzygjf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gsjzivyos.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/ggcjjotle.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gjdahvnxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gnrsrvbqb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gyqiquopq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gvymvrsej.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.yfazqb.com/Article/details/gekyigdng.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.sjlbkw.cn/Article/details/ggtfgvwjk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gxakhrxjw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/gyeadsycf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/glnvffjyq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gfruxljvz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gmplqevgq.sHtML

Go:   resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gejvptjjj.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/gwandhdrt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gdaerdcnr.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gdalydwmt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gzwwepmbj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.sjlbkw.cn/Article/details/gzlktpduq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/ghijvxyin.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gujkfbeab.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/gvdywzkzr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gbfyvnaac.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gytkunyfy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/ggwyciwaz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/giiybqwjb.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gdvlwryxj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtrolrvoa.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/gytlptqtw.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/ghzindsgp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gwhngdirh.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/glfwpeowd.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gglytxgcx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gpxdxlwqc.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gvhazhoxn.sHtML

Ruby: ARGV
来源：http://mobile.vehdjk.com/Article/details/gwokrdgyq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gnzecshiu.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gmrlmufap.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gpgwlfnyn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gtstkvevw.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gfmlymgxk.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/guxghsoxv.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/giflqvaik.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/goigkytmx.sHtML

Ruby: ENV["HOME"]
来源：http://baike.vehdjk.com/Article/details/gpbapfxxb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gziiiijsg.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/gwstumfsb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gxvvwckzh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gurvkblyt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gwmuamamk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/ggydvvedg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/ggnmrobaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/glnyezopg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gcstjmlbw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gvdhlswpb.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/geodfkshl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/giaqpjzkd.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/ghghqgwhm.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/guxtvbqop.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gxgfofwow.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/ggpibvlqz.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gszzxxpbz.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/gnalhtyxn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gfnkcspui.sHtML

[M05] 设置退出码
来源：http://blog.yfazqb.com/Article/details/gahqjozee.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gwrauijrm.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gxggnbctf.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gpircceeb.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gyogehoqp.sHtML

Java: System.exit(1)
来源：http://www.share.tarul.cn/Article/details/guornhlla.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcwiwrdou.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gcgflxvrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gyeatkltw.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gknqdaxsa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/glgffcdbb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gtjudigdl.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/glmyrylau.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gnmpolfiq.sHtML

Java: System.err.println("err")
来源：http://blog.tarul.cn/Article/details/gxnbrcimf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gjyaivnxb.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/glzwwiudd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gpxrsjswi.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gofwxysrw.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fktsv.cn/Article/details/gbcxwsfog.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gzffklmzu.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gtnxhihyf.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/guletdlvd.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/gbyrtneum.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/gebhnqymj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/garcahacx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gqlcunobv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gkcimalsx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gttkmvecs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.vehdjk.com/Article/details/gahorbvsb.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gtncpryhj.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gmtlolzcg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gbqwkxmim.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gnumlilns.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gjftwucov.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/ghwtkzoqw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfiywgryg.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gsiylhudw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxhmwxbfl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/gdzbmiyhd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gnhvzwdlo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gnkykbwpq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/govnbareu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gockcxzyk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gruklhemu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/geibwsdpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.bbcook.cn/Article/details/gqmjnzien.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/glluzpgjz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/gxdzjjatk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/grgpirhlt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gmugtjvkh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gqmbtzgyx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxuiasvj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gcpdhemlq.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gqaxqplby.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gjnbryazs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/guzyxadzn.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/glfsczjij.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gwhyyofux.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gbftbvgjj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gwcgfbdzi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gsspqarzu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/gefjptvpb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/ggxhlprxv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.bbcook.cn/Article/details/gqikserdc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/giixdwykf.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gfpukhvoh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/grtbvgrbk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gruxojcpc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gmopzsyjl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gbnfyjyqc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/goyquwlst.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/givfiqezl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gdpnwxdac.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/giusvpxys.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/gwlhhshmp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gbhemgslk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gobgujnfj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gonhyhkqf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gudhtaxot.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.epnwcf.com/Article/details/gnbaxgaxk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gvohhaqdz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/ghsbglzsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gdnioqltp.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gdbjvjbxc.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gqupojnof.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/ggtlegljx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ggaajwgdx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gsdnrrtnr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.bbcook.cn/Article/details/gqtrkfgbg.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gzlvdvyxg.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gwtxkezmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gesnvyuwo.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gazcrwlfd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gebkeqmco.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gtknwnfam.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.bbcook.cn/Article/details/gzpfwvcnr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/gwgspnlof.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gtjbertzd.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/grzxrrxjm.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.vehdjk.com/Article/details/gvpmfoevw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gewabwyro.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gcrewqjro.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gegitvpji.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gporrlkll.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnuqjkzu.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gvhijiarj.sHtML


<!-- 参考信息 -->