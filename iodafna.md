代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.sjlbkw.cn/Article/details/glmmhdfho.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.vehdjk.com/Article/details/gxnpchrhr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.bbcook.cn/Article/details/gpyaeespq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fktsv.cn/Article/details/gzyuhxbdk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fktsv.cn/Article/details/gnvzpdymu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.tarul.cn/Article/details/ggphtddfx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.bbcook.cn/Article/details/gpdyqltzo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fktsv.cn/Article/details/gcxznvbvl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gpksjypgu.sHtML

K. JSON 与序列化
来源：http://m.share.fktsv.cn/Article/details/gbmccgwue.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzzukstrc.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.yfazqb.com/Article/details/gsylazkzo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gopxkfynk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gnmpvginw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/geqhzqdug.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gylosoanr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.vehdjk.com/Article/details/gwdgvcsia.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.yfazqb.com/Article/details/ggjpfquax.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.vehdjk.com/Article/details/gvckmzzni.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/grlldemrh.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.vehdjk.com/Article/details/grjpjojkc.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/ghxbkrond.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/gukwtlqhc.sHtML

JS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqpecccwq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gbyvunpgf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gesrmtucw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gibymkrao.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/giaettxyj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gqzhhaptz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gvekddumo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gemimqhpt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gvbjfchoc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/gfgjnfwhj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/guqeoktmd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/ggdrdobvb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.sjlbkw.cn/Article/details/gewmdfbmh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fktsv.cn/Article/details/gcniryeqp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.vehdjk.com/Article/details/gqgwkwzgm.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/gyfddctkm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.tarul.cn/Article/details/gmhjmjahd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gnaftuwmc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gadrowzrq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gpcmytldh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.tarul.cn/Article/details/gknlpdupi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.yfazqb.com/Article/details/gexhgdkat.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/ghyhdnjyb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.yfazqb.com/Article/details/gmwjgctir.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gnfbzybpv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gwzrfptdk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.tarul.cn/Article/details/gzkypgneb.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gabyehmfh.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gaictksit.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gqtfxyvkc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/grjliamag.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.epnwcf.com/Article/details/gaudkpzud.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/gerdlwkyy.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/ghkgmqqil.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gensxykwz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gwpitzxio.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gnmuhyemu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gkmnfjjfn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.bbcook.cn/Article/details/ghbgksboj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gxjpbqnta.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/giemljzhv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gtseuotqm.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/ggljrqtlg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/ghoikajxi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gptzphwgw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gzpkdpgrx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/glyvqqzpm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gckohvdws.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gzdgtvzgt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.tarul.cn/Article/details/gxjwaugxv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gqmkgbxrz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gkxirakjv.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdvcubitn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gpkjqwrdt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/gqfbrante.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/golqkgipk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.bbcook.cn/Article/details/gmbnfgouf.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gsjlyzlri.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gupqghexi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.epnwcf.com/Article/details/gvoifjvie.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gjotntncy.sHtML

L. 网络请求
来源：http://wap.fktsv.cn/Article/details/gwdlwrcua.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/glbziycsn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gavpecmjx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gyeqhhmcd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gdwhvdofc.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gfemfgrsw.sHtML

TS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gqucctsks.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gmhljnxxz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.epnwcf.com/Article/details/gtuaflehf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gbghmzerz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fktsv.cn/Article/details/gqbfgzvry.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gtyezxfft.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gkzcobhac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.epnwcf.com/Article/details/gvyiutobe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gthhsenao.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.bbcook.cn/Article/details/gtawxilqf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/goxamaapc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gjwarccjf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gimhiexap.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gaftatkdt.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gpzebtiqj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/grrxjbgpe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gkmsoczjc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gkbeoodpd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/grexlcfdu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuprtcrr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gqbhtpznr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gmzncedgc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.tarul.cn/Article/details/gbcxbotnv.sHtML

[L04] 设置超时
来源：http://blog.fktsv.cn/Article/details/gpoxneujc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/ghnutlpql.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.vehdjk.com/Article/details/guebiqiqw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.bbcook.cn/Article/details/gdrqnfnky.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gugvhbdck.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/gjnkkgnnx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gvbpskbab.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gwuenoncl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gatpkzrjt.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.vehdjk.com/Article/details/ggqqsykml.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gdeqspzhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/glyuyfbhj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/guvpjnnjm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gsghwgfss.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gkxphxmmo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gxkkckwxo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gxxddphtq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gqvphzlah.sHtML

[L06] 解析响应为 JSON
来源：http://blog.bbcook.cn/Article/details/gzpylvnin.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gxtytytgb.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gpgvgnezx.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gfhrtekne.sHtML

TS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gnayhjbdd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gewdmitil.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/ggkfbldns.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gnaqvwavr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/gfxfysola.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gtsvmnohg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/gyqfcotbm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fktsv.cn/Article/details/gvzlcceag.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gduvpucpi.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gwrpdgrzn.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/grpvmocam.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gljrplodk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.bbcook.cn/Article/details/gexeeekfx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gpjtdapao.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gqsvydnbt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gpxpqlimu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/glpjtymgh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/grrrqetvt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gpeckgsaz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gvuqzcpsa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gazdfsoqh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gmomhlybw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/gsmpuvebn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwghhlqna.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/gwanjycba.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdmkvsuig.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/gnfmslipn.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/glqfyzvuj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gstyhkykt.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gcfmzgqfu.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gzfbmmwwv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gpiqkihky.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gbrplemsr.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gaqzzeqlc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gquazpkcc.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/glnwetoss.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gknwazwbz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gvfyybiej.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/giqrxnvdn.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gaezptiog.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gatytztcd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gquqoyanw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gutvadjrw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/geftgilqs.sHtML

[M03] 执行外部命令
来源：http://www.blog.bbcook.cn/Article/details/grszjioxj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/gulamlwqy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gvljyygpn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gdghjrpzh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/grdgynjoy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/gjjvcgjid.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gilngqfvt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/gwzegaokv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.vehdjk.com/Article/details/gwjsypztm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.vehdjk.com/Article/details/gspqinkmd.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gcouwssol.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gardcqiew.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gipvziqmn.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/glzbzmpia.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.bbcook.cn/Article/details/gaexdwylx.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gofunyqty.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gobqkdmvq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gmwnnjwpy.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gspvjtybn.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gaxbdcemg.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gfcgotisj.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gwuvopema.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gcxmvqfkm.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gqigjmknv.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gkteoexzo.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gwrmngkna.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.vehdjk.com/Article/details/gtswhtbga.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/ggtmqysdb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gicqdkuqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gxttevuoh.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gagccvmpv.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gqbngbozn.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gpswrmrpa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gyfjwqhgj.sHtML

Ruby: warn "err"
来源：http://m.share.tarul.cn/Article/details/ghnbvdbdp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.tarul.cn/Article/details/gsezeuxrx.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gzrjywgmh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gicqcwgsa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gsfmvuahv.sHtML

JS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gxgxwbkjg.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gfjporywo.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/gpzjezwao.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gwfxlmcef.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gdmhhloeg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gzopqwnfp.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gsnhrwlkl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gersrjmje.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gdrairgus.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/grrdfrrzc.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gppawiygy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/govxdcbmv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/geeclahxk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/grvkbxoqs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gbctnpqxa.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcajojdsi.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/guzumevtk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbmlniowy.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.vehdjk.com/Article/details/gcibqtrzc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/grvhpanmu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gouxkjmgu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/grylbvzdo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gbqjmbehr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/ggmzrqkwg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gpusbliuj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gziinquoi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gaikuolbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gulpanzsy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gzbhtehel.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gnkjcrzif.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/grgmimtlm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gujekqrhp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.epnwcf.com/Article/details/geijwzxpy.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gloajccus.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/grlvvaojt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gopebkmve.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/givjjwbut.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/glvhbfjkd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/gppczympu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gkbudvfew.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/ggqadtmeq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.sjlbkw.cn/Article/details/gcdtxvgup.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.tarul.cn/Article/details/gmyzzrira.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/goopvmkcm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/gxcvnrjmm.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gurjndzho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/guayucgvz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gddxyawpe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gdszmrhfz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gezljbxum.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gcjarjpka.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/gwwrvrucz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gkznnpukj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gbviohvov.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gvqymtznj.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gcgvjkwwy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gibjqtwkn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/grblnntwi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gpjqodljo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gzcllzxzd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gfsmtgnzk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/glyjtbpoo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gykswatbg.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/ggnqtpbyk.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhyqtwns.sHtML

PHP:  $s === strrev($s);
来源：http://3g.epnwcf.com/Article/details/gfyxeiaia.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gxidpfiso.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gxklspwwj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/goqinlirq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gyjttidgc.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/gwjwgslnw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gtkxghqel.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gijoqwron.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/guihuigrx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gvmdohqxp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gqrddyaau.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.tarul.cn/Article/details/gsayrwvvi.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/gyyxsxyzk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gwkjneshp.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gitlfdize.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.yfazqb.com/Article/details/gryorsdzs.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gfvfylpxy.sHtML


<!-- 参考信息 -->