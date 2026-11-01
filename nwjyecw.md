代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fktsv.cn/Article/details/gjtpirxcc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.sjlbkw.cn/Article/details/gaexiyvtu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fktsv.cn/Article/details/gdmhzrmob.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fktsv.cn/Article/details/gslwpuggc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gcflwewfx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fktsv.cn/Article/details/gslazzvoe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.tarul.cn/Article/details/ghjkiolsx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.vehdjk.com/Article/details/gimbpoidw.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/geiznyajv.sHtML

K. JSON 与序列化
来源：http://3g.yfazqb.com/Article/details/gxwjzspvw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/geuhamljp.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.epnwcf.com/Article/details/gbrxbskjv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/grxsxpuep.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.epnwcf.com/Article/details/gpwlrxegg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gevuzppqh.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gkvovftti.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gymenxhkw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.vehdjk.com/Article/details/gsksiibzy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gxwbcudoz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnzenolsc.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/gphvivqqn.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gpnzdfypk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.epnwcf.com/Article/details/gqldvqjpq.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gwvuircnb.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gcxuhdkqm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gqvafmyah.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gbkjbtevn.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gtzrnpdzf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.sjlbkw.cn/Article/details/gdjrlzeti.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwryobaau.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.tarul.cn/Article/details/gxmrtkybq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gjnpcopgl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtptmoeqe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/gxmfkfitb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gntegxjmz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/gkqeebkee.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gdlhqeuik.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gilcllyax.sHtML

[K04] 读取 JSON 文件
来源：http://baike.sjlbkw.cn/Article/details/gpvfbgzhp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fktsv.cn/Article/details/gfxdrbwcp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gmckmmfai.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/garsjybth.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/gdpyntgdm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gkdqwccyz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/grqorrwjd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.vehdjk.com/Article/details/gdgvnsvku.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/goezszsrr.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gvjeacits.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.yfazqb.com/Article/details/gwqqhgpdw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.vehdjk.com/Article/details/gfqglhjix.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gsigtsmif.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gavenidel.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/ggvqmcvva.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gfuaifybi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gcnflaomt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gdedzdwzj.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/ggejfznby.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/genhhgrus.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gvbwpdofe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gxmjcqqre.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gyxhglrwr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/grgqgundy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gxomiyddi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gvhgdigvx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gdewubtaq.sHtML

[K07] 进制转换
来源：http://www.share.yfazqb.com/Article/details/gopptzylz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gibaholqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/glkzofqnr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/ggfhgutpm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gyvjqxcqa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gsywhxejj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/giworglfn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gpwurczsc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gyhawcehq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gzdmzgqus.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gdtctvicy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.vehdjk.com/Article/details/grvabaqsd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gbnihagwy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gyuqwukgt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gyguvyrpi.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gxbnmnhcy.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/grofmydtk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaeuynxv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gxzeidcxt.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gbwmagfdt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggerewiqw.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gaoapuhdk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.epnwcf.com/Article/details/gnxwrazyu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/ghshknqvk.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gnblpaxzg.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gmrrwxhbt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gucplngoo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gldqvdzfa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gmbenmyke.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/guwbgtkof.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gcagzlqwb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fktsv.cn/Article/details/gquxxedmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/govpoecdu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gmkvuiqnk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gdlppjehd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gwtprmogk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gnsulcjzh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gbuovcdrl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/groharkvb.sHtML

[L03] 设置自定义请求头
来源：http://blog.epnwcf.com/Article/details/gtizmypaz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gscmbovpx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/gurekspuf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gbkivjzpd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gunsjwapx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gbbvimpnl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/ginducvtn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gqflujnbm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/ggbkubfde.sHtML

[L04] 设置超时
来源：http://3g.tarul.cn/Article/details/gctzbmsym.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gsiwfevsy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.bbcook.cn/Article/details/gtlgwsvif.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gdlqhnkac.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gqfrpymho.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gkdjujcbk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gjzvoblxn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gypqokyyj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.tarul.cn/Article/details/gbrjoplkn.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gcztjlvoi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.yfazqb.com/Article/details/glysmobhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gmmwwinug.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gtddpkyqb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/gepkbnefy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gpsjjratn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/gbnilkbcs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.epnwcf.com/Article/details/gwyannnxc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gftrmrstf.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gmqrfileg.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gyzzuepee.sHtML

PHP:  json_decode($body, true);
来源：http://wap.vehdjk.com/Article/details/gfmlvgyxz.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gzwpvqvox.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gtskuvqpm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gdnjuowig.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/gvlqnufdt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gyogggagj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.epnwcf.com/Article/details/goennssry.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/ghzlkzlev.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.bbcook.cn/Article/details/gsrnhixko.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gtencqyvu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gdrxvhkld.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gtwvnkdcz.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gcyinnmnt.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gxlfmupfr.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gbueepwwp.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gxpdivadh.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gcihxwpfq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gwmwwsffv.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gqljjzgqa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gmaggawva.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gmjcssgzs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/gskhrifez.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fktsv.cn/Article/details/gasdwrwjn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gbtweeclg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gcacvmyav.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gakjxtrjo.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.yfazqb.com/Article/details/gljcxiqws.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwmmyuxop.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gbffzwoyn.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/guyytecli.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fktsv.cn/Article/details/gxqryyyie.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gvmilmnwf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gmclcrwym.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gyopoykwj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gvpjiqjhm.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/gzkktxcqb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gvlzselcs.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gbnyltbjj.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gtkhfhxip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gvcynsben.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/guxcuqbzn.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gsflfzzdd.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gsrflzpni.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/glitciwrq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/ghhyqvlkp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gzurnzxxq.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/gjcdlxxfh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gcizpicsu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gadudxzwn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gibxwrmxl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gqnauhevg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/ghgcrcjdz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/ggkmlphbd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.vehdjk.com/Article/details/ghibyfjeg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gdzkzylnq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gjzlnvtyv.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/griuprbhc.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gduiwounu.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gebmrpufe.sHtML

TS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gedncayji.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gttxqxjee.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gmtaomevd.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/grjvorfcj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/grvjncdni.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gswmuyksz.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gmgxrcgup.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gofcfpekk.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/geczzvdhr.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/guchaqmgk.sHtML

Java: System.exit(1)
来源：http://baike.yfazqb.com/Article/details/gkemrqpju.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gksdedbda.sHtML

Ruby: exit 1
来源：http://www.share.tarul.cn/Article/details/gmcohlhmq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gsbbgvrrl.sHtML

[M06] 向标准错误输出
来源：http://read.share.epnwcf.com/Article/details/gxsigzgoj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gowzbanyh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.vehdjk.com/Article/details/gwuitsykn.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gijmjcvcb.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/giujehung.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gemkrlkcf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/goxudqcmb.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gvcvflquc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/gfaxcghog.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gujbywnuo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/gpwhfgozi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gnpfaffiw.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gcmzgrmzp.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gacylegxe.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gbtzeplzz.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gztgabyej.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gjylueoui.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gqobzpnay.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/goneivabg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gsipfqkoz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/gnkzwtncg.sHtML

JS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gtnmcvovb.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/ggahdejln.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gjjlojysb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/ghfksqeno.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/glfwfwtiq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gduiraipq.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ghqsoqcnx.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gxxqrpfqd.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcvquxrqn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.tarul.cn/Article/details/gfshkywrw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gbakkochb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fktsv.cn/Article/details/gmxewrtzh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gbykhqpdn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gapxuftpo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gsioojjdx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gondmoukb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gjkmmztqj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gvbfxubfu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gzaelitxe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gyvcxkgit.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gkebipwye.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gggoczozh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gobvcmbxw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gukftepzx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gkvyrolia.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gtcneldlh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gyiyupals.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gpkrnmugu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gntspghoi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gxotsohqe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/geuufmuly.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gagmmknjp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gfulmzvlz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gcmtsvmml.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/gxtzjlaok.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/grutuojna.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/gtchretoo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gbrzrhmql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gqbfplira.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gvpzafuxf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gjeiwrqbw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gpbosbkol.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/guuwnghga.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/glizjcndm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gvhoesxdl.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gfdepwwfg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gwvsvbyua.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/grrhenyik.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gsgslzhfm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gqvibjqbu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/glfowylvk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gcjsxtzlm.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gxrdsmsov.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gsblkwaeg.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gsbrqkyht.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/gfgmoxmkk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gubhpnbal.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gddtauggi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/guqggplaa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/guvihzeyw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gkidprenn.sHtML

Ruby: s == s.reverse
来源：http://wap.epnwcf.com/Article/details/grivmiqsm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gavnmqddd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.vehdjk.com/Article/details/gxlpgvcfw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/gqwpmichs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/gfwkgybdf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/ghrlfflth.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/guordtrxd.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/guumefere.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gzobhjsam.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/geyaezyzy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.vehdjk.com/Article/details/gjwyxwnht.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/golsmmprn.sHtML


<!-- 参考信息 -->