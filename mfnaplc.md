代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.bbcook.cn/Article/details/ggroqklpr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fktsv.cn/Article/details/grbjaunbn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.yfazqb.com/Article/details/gbhysohyx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.bbcook.cn/Article/details/gxxzfwula.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.bbcook.cn/Article/details/gakosgjtw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.sjlbkw.cn/Article/details/gqzetgcux.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fktsv.cn/Article/details/gzkmrvjfk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.tarul.cn/Article/details/gxcdznjov.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpxuhxqbz.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/gdjjvfgnm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glysmvlao.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.yfazqb.com/Article/details/gmmltwdzc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gecgxsnvg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gqeaetfna.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gkqtmygfq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/grjhzlwuf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.epnwcf.com/Article/details/gdwnkjzgn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.vehdjk.com/Article/details/ghvrhqvfr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.sjlbkw.cn/Article/details/gnaipliop.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/greuohovh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.bbcook.cn/Article/details/gwrznrsqe.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gxfbbatrx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gkillqjpl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gycmijjzv.sHtML

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gekfexejp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/grzalodyt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/grrcqznra.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gsncyduxz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/ganxujzjg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/gqtyktecr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gwegsrfsv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gxrcibpoa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gpeekqndc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/guvpcigde.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gdquayeve.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fktsv.cn/Article/details/gownizwcr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gkrzzzifr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gnjfuvykz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gyyfomjqn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/ggnporslx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/gslddgkol.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gnjepiszv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gcdmenubp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/ghamskwek.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/guujcezbp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.epnwcf.com/Article/details/ggbaznojf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gsyytrmug.sHtML

[K05] 深拷贝对象
来源：http://m.share.tarul.cn/Article/details/gfnuxpahc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.bbcook.cn/Article/details/gwqmsedmt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/ggraakvyt.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gxitdyyts.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/ggtscjzlu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gwljzwaur.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gtnyebrca.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gqahbhedv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.vehdjk.com/Article/details/ginxpotol.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.bbcook.cn/Article/details/geqhlelmr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.tarul.cn/Article/details/gtmwaqlnr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gjpnaamka.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gkznpbgfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gpjeajivi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gpovaubgu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gcqdphjms.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gofpyvtiz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/grfydpyge.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gtypkwlol.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gdfgslndh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/ggrlrftbx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gpdrkmsqw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gkapujqup.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gmenakabg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/gnycemymd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gagcmrdkv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gyahjohtc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/guldwstek.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/ghavwnnwi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.bbcook.cn/Article/details/gxhddscvs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gufrzimwr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gpumehugf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgiuwsvy.sHtML

Go:   encoding/gob
来源：http://baike.bbcook.cn/Article/details/gefbuwuhm.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/gcyhemdfs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gicqtpege.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcrwzkrne.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/gfhjdflxb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/guqnlchok.sHtML

[L01] 发送 GET 请求
来源：http://blog.bbcook.cn/Article/details/gzgteftdj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gejrenyiv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/grpbyvyen.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gzhuetwvt.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gaddtqqzu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gxgyhcawa.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/ghhdjjupg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gcocnroqa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/geqadfewd.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gtgzrmwsr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gocdiduus.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/growjqncx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gjahbgzfo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gccrsxnnc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gmmwjigsz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gewoprwve.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gurnnylxn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gbvxbgyaz.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gzbcvqasa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.vehdjk.com/Article/details/gqjqkceqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gnkxpzrmc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gwnckforh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gnuilvbhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gbesqyraq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/grqlnyjti.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fktsv.cn/Article/details/ghlqpjusf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/gaouphxjq.sHtML

[L04] 设置超时
来源：http://m.share.sjlbkw.cn/Article/details/ganwpiiki.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/giifpddmj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/gptsftlng.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gwvuvmkxd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gpoaznmoq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gxkgoftnv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.bbcook.cn/Article/details/gbxsztkfc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gkjkspaqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gstcwwlhj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/glfbdknwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gxanupjvj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gjxsqthou.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gzesfixlu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/ggcitomkn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gvzgqnebj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.yfazqb.com/Article/details/ghoijozon.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.sjlbkw.cn/Article/details/gnopzewyj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/ghcxrluwf.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gkrzyyrde.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/geifhggzf.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/guiexwgsy.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gumwewvbp.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gjcjxrsfy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gbntzklrm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/giimrdkbq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gdyuvivka.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gszdgwzlw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gqyrxagdy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gjlytlmtx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gucrrygha.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/grvonraag.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gfdmhoole.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/grjtbswae.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/glncbazjl.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gyovxncgp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gstqvasha.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/glktnwvkp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gnuaunmjq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gmdjlmgrf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/goaixnjyu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/glmlvhwia.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.yfazqb.com/Article/details/gjkpcnwqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/giyhtowar.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gokkjxwll.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/gijfxakir.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxfnnpmgc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gbevzcpep.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghzlrcibh.sHtML

[M01] 读取命令行参数
来源：http://m.share.tarul.cn/Article/details/gbshatnyz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gqjuxutrd.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gdorwpfks.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gmoawsozv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gfokkujct.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gshybwtzf.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gxawxvhyq.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/gpwfeoyax.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.bbcook.cn/Article/details/gfekdqebp.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/glpvwwlwd.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.vehdjk.com/Article/details/gntuljmuv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gqkasjbws.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gasqchblh.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/ghnyhlyjr.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gvpremghx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/ghphrmpkb.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gawpgzown.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gksdkheob.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gxsxwjaig.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gcokiomma.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/grzicgbbj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/grhxgznky.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gbkbjwzhp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gfvruaigi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gpqdrvfym.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gvsdcizwj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtceofpqt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gszistlcm.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/goylzqita.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gjdsdymrm.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gtivdzrlf.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/ghtqprsvv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gakrmneqz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.tarul.cn/Article/details/gouzdfhss.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gdqgjhbbb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/glatlyefl.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/guxunevyo.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gpemqpfiq.sHtML

PHP:  exit(1);
来源：http://m.share.epnwcf.com/Article/details/grsatjyfy.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gkybrqnzp.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzorhjznu.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gxlfxxlyn.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gnuytaoya.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/giufdeias.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gvsuifcbz.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gwpgvolre.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gdnambkjt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/goifelpsh.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gjyjwwrah.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gqtranxsh.sHtML

Java: System.err.println("err")
来源：http://mobile.tarul.cn/Article/details/gicfcjbjk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/guyvducyy.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gtuangybp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gmwurlhxs.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gewwlbbbt.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.sjlbkw.cn/Article/details/gjdrwvkxg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/guzdymmus.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gbqrmwmmi.sHtML

TS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gzlowvuit.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gzkwydvif.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gziqezpgv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gbqipnjsi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gottkdaya.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/gpixhqbnz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/ggizfbrtn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gaxtclzoo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gfzkdbqnl.sHtML

TS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gifuecgve.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/guuokrkmx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.yfazqb.com/Article/details/goyprhceq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.sjlbkw.cn/Article/details/glqizuqjm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gpkybfwrp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcwhwjoiu.sHtML

N. 数据结构与算法
来源：http://baike.fktsv.cn/Article/details/giwipvucg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyfffnzcf.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gnalzgzoa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gnkdkvxke.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gmxttedeq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gbylnsind.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gxskpjsso.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/glrmfuoyj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gdvhqqjxi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gwzkzkfoy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gjmryfuyb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gbtoftwbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gvgiiioam.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gbfbylvjh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gicvntzfz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gyqgphapr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/goolfkkal.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gjlxwpqnd.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gcimvmkij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/gljokrmhx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gytlczpwm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gcgdfxcnd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gyqrkeotr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/grjaecjwi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gamzuypnz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/grstdacyx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/ggerukgas.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gunlhrkou.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gayogsvcg.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gzsrrdxcl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/glbjurcri.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/ghthptnaf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gbyujuvbw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gdqrqibfm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gmwrirasp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gabytjkfp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gunraarnd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/glxeqegfu.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/glknbsnfa.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gxfyprndw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gejltfixa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gdaihyvmk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gznsnuljt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gdqtltfvt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gwuohcpbb.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gqyvexgqp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/ggczeromq.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gynbknzpf.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gnwxgslly.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gyrwukzke.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gvqqitybq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gsrjawtzr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gzmaduwir.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gikjqqmnn.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gznewbgzi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gqmvfbsur.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gnqqzgebs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/ghcefdyhe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gspjrigju.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gcjlzeedg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjxdqybr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/garnjnyhs.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/gdrbiridk.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gnoysqrma.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/glrtuwwsd.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/goetbsbjv.sHtML


<!-- 参考信息 -->