代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.tarul.cn/Article/details/gjfiosaaj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.bbcook.cn/Article/details/gqkfaqhxd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.bbcook.cn/Article/details/gzuvelfmj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gpihfkbum.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.sjlbkw.cn/Article/details/guklbmxyc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.epnwcf.com/Article/details/gjmjqzzhk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.vehdjk.com/Article/details/gdnmyhipd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.epnwcf.com/Article/details/guyweqqyo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxzydimml.sHtML

K. JSON 与序列化
来源：http://blog.fktsv.cn/Article/details/gnepmsvha.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggbusnodc.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fktsv.cn/Article/details/giwavwnma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/gdzvktlze.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/giwdvxfix.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.bbcook.cn/Article/details/gvcnubtik.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gyavpjzjn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/gpeewmice.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnzxiohbb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/gylcrtlha.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.tarul.cn/Article/details/gliohdflk.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/gacdsxagu.sHtML

Py:   json.loads(s)
来源：http://www.m.share.epnwcf.com/Article/details/gkduxmpag.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.vehdjk.com/Article/details/gyvjoplvc.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdymhaqw.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gonexmzhb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gxahtpefy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/ggxrfjkcn.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gzofaiatg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gehmisshi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.yfazqb.com/Article/details/gsfmameji.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gouyoeith.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gehcgsssk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.yfazqb.com/Article/details/gcloyzmwb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/grftmndjn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gfkjeclin.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.epnwcf.com/Article/details/grvwxeddb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gjcczuhpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gavpjusmf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gtuocojwn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gqaedevtm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gqzeezopq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gcmfzjupy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gjordxgru.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gyvxhnivw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gdkatvfsw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gzcqwssbc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gyoasmeki.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gtkroxbvx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gpatjrtrb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gezyrivxc.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/guhayzmcy.sHtML

TS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gfxmixnzl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/gtbgywmiz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gkelunpds.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/goxvibtkf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gccdjmosg.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gkaggvwte.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gpxwcxdey.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/gbhbgsiyz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gnqxgtfvn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gjvmaoapb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gydkoaumb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/ggtjqxzqe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gfrxwnbds.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gspingohl.sHtML

[K07] 进制转换
来源：http://mobile.bbcook.cn/Article/details/gbgzjorcf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/ggglfohtn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gqtygjxsi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/glhepdyif.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gwkvelbro.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gaqcdyubm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/gapffoomg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/gvzaawubb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/ggiuqurmw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/gebziynpw.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.epnwcf.com/Article/details/gwoapjvki.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gxzkyrrfs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gccoslika.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gqspaneio.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/gxjrhryrw.sHtML

Go:   encoding/gob
来源：http://www.share.bbcook.cn/Article/details/gwgrwydwk.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/gehzjxchb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gymxfivci.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggxepbsli.sHtML

L. 网络请求
来源：http://3g.yfazqb.com/Article/details/gheschpow.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glmagkrho.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.tarul.cn/Article/details/gaopggzpp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gszifvzed.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gbnkhpapx.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gaejnkrbt.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gojopcuaa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gmznalxfc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/gcftbmlne.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/grzbcwjkk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gyfkskzav.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gvhcszfsi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gyiwjewgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gscpnocrv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/geamnnchk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gjszrzvpx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/ggzwchzgd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.tarul.cn/Article/details/gtpstzvsy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/ggfdvwamn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gxxaclgwh.sHtML

[L03] 设置自定义请求头
来源：http://mobile.sjlbkw.cn/Article/details/grqqztvot.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.sjlbkw.cn/Article/details/gooozgoct.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gpopskkua.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/grooqxdle.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gsbhmncrq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.bbcook.cn/Article/details/gqyzhgsoq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gvsmkqxzw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/ggdtdstia.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gxiroiryf.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/gduyqlkqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.sjlbkw.cn/Article/details/gevjwpshw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fktsv.cn/Article/details/gymfpxqwk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gcgftwqps.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/golmwkkvw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gkukdyslr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gmqbxhldt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/givnyhlvq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gszqfodpi.sHtML

[L05] 上传文件（multipart）
来源：http://wap.bbcook.cn/Article/details/gtujyhydg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gvxolsoox.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gtvyceswg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gcsjuqxoa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/glahhgalh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/gdwxndqcm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gfyntghiz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gmnbtmsbu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fktsv.cn/Article/details/gzbivdule.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/ghjmepnvw.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gzhjhcott.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gdcvlaiee.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gktkvvuew.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gxqlvpgvg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.bbcook.cn/Article/details/gqvebnqak.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/geigsbtfw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gjqyfvdfm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfykhioz.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/glzbweezo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gzbxqdfge.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gukxidzqj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gvwnvqtkl.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/ghjeoygmc.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/gmponggtc.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/getzjryoy.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gdmzaenap.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gjszvvswv.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/ggtskazev.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gfpraswor.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/gvetxcbqf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gmxuodycm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/ggmuvhlve.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gecvuscwj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/guwxdzqhb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/gveoqbjxp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gwuvjekvm.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqvuvzcll.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/gmsptlnck.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gilwjzgit.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gofggvjvr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gznywlfzl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/glblrsxqh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/geyvkibpb.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gkjwoppbl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gncdtmtfs.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gmmlxnyvt.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gzcjpadvq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/ghmofxrms.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gyzihxhon.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/gpgbgbyjb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gxyrwfazm.sHtML

JS:   process.env.HOME
来源：http://baike.yfazqb.com/Article/details/ghzdugxqw.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gzwxntkef.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/grzpgmxyh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gsjcstthe.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/gwtjdslqe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gbhrzedak.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gphgqegyz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/guegxnctz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/gurmxxwcd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/guohwqggb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/ggntmdgxb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gdwkaqlag.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gyjbzbzhp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gsdgvacpv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/ggsbnxktn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gwkypbmsu.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gfuxdkigt.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gexfauhqg.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gedlkbpbg.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/ggdoyaptj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gipipcptg.sHtML

Go:   os.Getwd()
来源：http://www.blog.fktsv.cn/Article/details/gywnarfkv.sHtML

Ruby: Dir.pwd
来源：http://3g.yfazqb.com/Article/details/gdxtgkuxp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gslcvuwgx.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gcmxdyfid.sHtML

Py:   sys.exit(1)
来源：http://m.share.epnwcf.com/Article/details/ghjteewqu.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/gjbeymhww.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gfquvpqqq.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gavjsxvad.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gkmewrnlg.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/glzxwwrsr.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/gzsmgrlhd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gdpuchvsl.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/grghpwkjj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlkmquvb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gaekjmunu.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gwnihvtme.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gvpqqxioo.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gqziwwyys.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gggqloljj.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gdvquesyz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gqjzxsivj.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gajugevqk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gjqpnbnfz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gbuosqgwt.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/ghwxlmxxf.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gaudadcaq.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gettqllpx.sHtML

Go:   func main()
来源：http://mobile.fktsv.cn/Article/details/gflpiawjs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fktsv.cn/Article/details/gztjjshit.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/geojuiqay.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gqkizmdue.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/geonytqlq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gtfypujxo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/glwpikwxc.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gkpdpjrmp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/ggusdmnkz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/gkdoforpy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gchjmnalh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/gkqjaruvj.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grscsegvc.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gqzoypanm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxxxszdkq.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gqnbszlye.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gdlhgydgo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/gkrsvpgtf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/goekaeilo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gxdwyxyhz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gxauxmqfk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gzeaebbpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gdynllugm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gmdunfelk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/gjqwktyke.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/grsoxlzsg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gyyeyfyaz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gjzmlosof.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gkramegzf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.epnwcf.com/Article/details/gopmzugtr.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gmtzbkxhm.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gexkitaso.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/gkpugigoc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/giwfhmttn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gwsliylei.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gaslwdskw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/ganthvupz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gzowypnmb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/glxjwhvjz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/gajbfnjhz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gonyxvfgv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/geoghttbp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gyxuzvnjn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gmpzafvun.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gtjafgbij.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gvlzlcemj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/guhlhytud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gnlhrnhxu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gzpizvvgi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gvhorcnjh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/geygmydhn.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/giahxarax.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gkibxdbmy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gvwaydzcu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gstyfupxc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gfdolgnzn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gujnerzib.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/ggwkqrsve.sHtML

Ruby: a.gcd(b)
来源：http://read.share.epnwcf.com/Article/details/gbwarfhhi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/glilrudrz.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gevezixvr.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gfmzhfphm.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gakzqtbpa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gokkdywol.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gurrtrtyv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gvuimtfnc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/gwxljqpjs.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gwdknagyd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gupacbxzx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gpqauzcpd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.bbcook.cn/Article/details/gwkeyprof.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gamakizhb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/guxgqpiwb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gzjqeyvlt.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gopaibksh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gsxvveotb.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gkpjukznw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/ghfetkmth.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gkswrgvbk.sHtML


<!-- 参考信息 -->