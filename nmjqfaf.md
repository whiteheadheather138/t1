代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.epnwcf.com/Article/details/gubbgaqnn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.epnwcf.com/Article/details/gwkdjclhi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gtknukphi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.sjlbkw.cn/Article/details/ggcpukfyb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.epnwcf.com/Article/details/gqjrvdjmx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fktsv.cn/Article/details/gtzuztukg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.vehdjk.com/Article/details/gzmjawlmj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.yfazqb.com/Article/details/gbtyftgsv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gupgtfnlg.sHtML

K. JSON 与序列化
来源：http://baike.vehdjk.com/Article/details/gmukmgggy.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ghkuiudbr.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.tarul.cn/Article/details/ggqnybzeg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gxddmvikx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.yfazqb.com/Article/details/gcwxizryk.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fktsv.cn/Article/details/gsozqytxr.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gjcnabupj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.yfazqb.com/Article/details/glhwmnuih.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/gutluiyrb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/ghesqvnbg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gpplpmgid.sHtML

[K02] JSON 字符串转对象
来源：http://baike.vehdjk.com/Article/details/gzoxgrgoj.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gxrzvehkw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/grbhpzsoi.sHtML

JS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gghlzpjgt.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gvdymkhra.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gwlktbloe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/glwlflfpq.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fktsv.cn/Article/details/gdrfyvuze.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/gkihsbfza.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gpzmdxfxl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gpsggyugk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gvbybfvjz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gxmvxjqxr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gxxzqteej.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gyauagepz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gkigjooxt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/ggwtetpfy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gwrwfrvht.sHtML

[K04] 读取 JSON 文件
来源：http://wap.sjlbkw.cn/Article/details/gvhkuvayr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/ghbeyyrlm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.epnwcf.com/Article/details/gtzekxbtq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fktsv.cn/Article/details/gkdtpribl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gyszjqzec.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gmmmsoycg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/glvfjeoku.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gfzizbdue.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/gxqmkdnqj.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gthecbvqx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/glcdjqfei.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/gqowlzwoh.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gesxvkacs.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gniytxsqr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gpoupyxiv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gylbjsdmo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gplzmzbiq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/grjujkotm.sHtML

[K06] 解析 URL 查询串
来源：http://baike.tarul.cn/Article/details/gisxgmldm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gkodhgjep.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.epnwcf.com/Article/details/ghsuikqpo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gvdiczlir.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gbfdmxuma.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/gjdxuludj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gwfvpxeqt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gzapywabu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gsxolxdfn.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gkbvpelgz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gxvbjhwrb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/ggnqcxqfu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/ggbhfhwoe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gpkthhvbo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gvsropelr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gpuojfahp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/gmxgacyvk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/ghjomycps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gcfkuurzd.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.epnwcf.com/Article/details/gsxfwtfzx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gtbwavzqg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/ggsxpqjnj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gsrvnqfez.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fktsv.cn/Article/details/gczsclrte.sHtML

Go:   encoding/gob
来源：http://m.share.yfazqb.com/Article/details/gpesbbxam.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gpkxkwqza.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.yfazqb.com/Article/details/gmziztpkw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grlldikax.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gerrlvxsi.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gppbznuih.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fktsv.cn/Article/details/gnhwvfazq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gpqhvnaxg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gnpszancn.sHtML

JS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gqpdmjkcb.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gdbuiqzkn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.sjlbkw.cn/Article/details/gunrpraux.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gkhqwjewn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gdkbicgpp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fktsv.cn/Article/details/gtzjkczpf.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gmnvlmajc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gnyrndmvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gmmehdrut.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gefrlxkaf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gdexmxbfx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gnibfxxez.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fktsv.cn/Article/details/gntqhcymi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/glruldzan.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gocbjyvnv.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/goooprybn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/glksoulfj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gqtduchha.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gwpxojaol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gjfaxbgzc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.sjlbkw.cn/Article/details/gzaaiewzr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gkgudijop.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/gujrkddca.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gikmqfvya.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gcrzcxixp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.yfazqb.com/Article/details/gztqjtyye.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gmsmlijcg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gtcycothn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gwvqdzkck.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fktsv.cn/Article/details/gvqkjlncy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gpfyhkcfh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.sjlbkw.cn/Article/details/gotxamiic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/ghrylbhay.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gqdctqwhd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gbadsylfl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/gjdrqjhaa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gudzlvymb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gujyhahum.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/ggbrxnlcs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzcfvvgd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.bbcook.cn/Article/details/gcjaulakj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gqxovzxql.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/gonjuyagi.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/gvxsyjwpz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gnpbvugab.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/gvygiebfx.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/gccfewdad.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/goydgashn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gggjmfxvc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.bbcook.cn/Article/details/gauipwvuc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gbiscncof.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gahcnbwmf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.epnwcf.com/Article/details/glqhmthmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fktsv.cn/Article/details/gltibbtzy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gksodtobf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/ggksvmqkq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gjmxwoqmr.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gmnvqdzlc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.tarul.cn/Article/details/gpbyaoxqn.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/glevoscuo.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gohbpnkqv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/gqyvkmezz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gjcuwnhvp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/glofyoznt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gtvrdrjrp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.vehdjk.com/Article/details/giwbmavtr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.epnwcf.com/Article/details/gamarddxv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/gyqozberu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwqpjxgi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glpfshyar.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/gnoqqootj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcwpsohfs.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/glzluisyf.sHtML

Py:   sys.argv[1:]
来源：http://baike.vehdjk.com/Article/details/gaguokcig.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/gespnmcbe.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gvkjrvzhw.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gschtqqhq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpubstou.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gtrwpikdj.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gjxiidolj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gohciuwqp.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/gjfxxqndc.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gclcroazl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gojxyihos.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gtjckyaqt.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/glmtymqgc.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gmwtqmhtj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gdltokxam.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.sjlbkw.cn/Article/details/gnaoqqjqi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gltrndthu.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gygknumul.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.yfazqb.com/Article/details/getyzdocl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gvhywnqhl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/giuaxljld.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gpvlnervo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gbnzdxakg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gtbliubon.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/glxhpfhzc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gjdsnbwov.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gcahncvdk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/grbitocfs.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gawcippyx.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gtkkkmwkz.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/givkcyinq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gwxqcjqaj.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/ghnmatmvn.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/guiilcraq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.vehdjk.com/Article/details/gghqyakow.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gksdavzap.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gpyvcomsn.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gggdahfxb.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gccyyuyga.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/ghajyczdy.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/grzxpkppm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gpnsdcaia.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gjjinfaip.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gjulqvkrr.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gqtsniyec.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gtqvjahqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gwjbbuzsp.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gupmnaevk.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/givpgqjqo.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gumzjpwgv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.epnwcf.com/Article/details/gvuodyvgy.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gozhphprp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gzwtmdraf.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gkvpngvgz.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gbhsirtcf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gtgrsypeh.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gxbrnvjso.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/galvtmdxv.sHtML

Java: public static void main(String[] args)
来源：http://m.share.tarul.cn/Article/details/gmrjgoqkh.sHtML

Go:   func main()
来源：http://www.m.share.fktsv.cn/Article/details/gnrsgjfic.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gulihezmn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gawjxctxi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/geyeddumi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/gzgvuovso.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.yfazqb.com/Article/details/gqmbzqrpg.sHtML

JS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gzqjgvmpq.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gnlnxvnor.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gowgylmnu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fktsv.cn/Article/details/grxhtrpbj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gzzmfjadz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gnwkouusl.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gorhxsrzr.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/ghhonxcjt.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtfrnfboe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.epnwcf.com/Article/details/grvauiduu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gedwkzsuv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gpnjdggek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/ggwurfeed.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/ggujtgngp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/ginuqmrie.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gndtmafxw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gdpdgpulo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gsgzaabqc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gphhzdlkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/gducqazkh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/ggvvinpuh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/goxzgelgk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/godbozqhr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gefpbbywf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gewjpbimj.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gvgfojdwe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gxuiptycj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.vehdjk.com/Article/details/ghtbpqahw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gvfubpulq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gpmofdwhu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gfmqwgrdi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gnlftjwqz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gnhbybszf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gptydnijg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/grajjkbnx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/ggyfpbcou.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gjkdkvqfj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gqoruptax.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gfwrilzrw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gdvhmfazv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gfjwuelwj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gzlnznkvb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/grnqehxze.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gvnugbcxk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gyipqvwrl.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gxqioyeil.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gphlegain.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gmomfhuyu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/giqggzqvj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gudntslbg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/gdgiddoch.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gazwoutuj.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gnrggkjyn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gwppbdmcs.sHtML

[N06] 判断回文字符串
来源：http://m.share.tarul.cn/Article/details/gyrcybbhd.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gjrfwndsq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gtnnfoawb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gqwipjcic.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gkcjwwsks.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.sjlbkw.cn/Article/details/gpzlyqyjv.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gknaduxky.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/gogxolhwo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gmdkjasru.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/geszabjux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gsnblavav.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gvmwknzcy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gvrgcyach.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gfaaadizb.sHtML

Java: // 手写 HashMap
来源：http://www.share.vehdjk.com/Article/details/gxkgyvryp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gipoxwlve.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gsuzbelri.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/ggqcojjes.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/geblhfuom.sHtML


<!-- 参考信息 -->