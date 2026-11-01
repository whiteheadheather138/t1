代发 wailian999

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzdnlfwug.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/ghycdkdcy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gagwwvvjx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/ggmhjaghu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gystzoycw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.yfazqb.com/Article/details/gneyhebnp.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.yfazqb.com/Article/details/gmgjzlfhn.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.sjlbkw.cn/Article/details/guhgitcrq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.tarul.cn/Article/details/gjwfhhbka.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gjiqdqggt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gpqrzskvg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.epnwcf.com/Article/details/gzkpfmklt.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.sjlbkw.cn/Article/details/ghmxtueur.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/ghihsnfuz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gkthecyfy.sHtML

JS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/ggjnmqvfr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gltroqpbx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.bbcook.cn/Article/details/gyqdhsddn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gmntilova.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gytmsbvet.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.bbcook.cn/Article/details/gswzllktc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gnkqukagl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.yfazqb.com/Article/details/gxldtdrhe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gggvpesfo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gcmrhvexh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gvbwgdlln.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/guvyaalfd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gsgqqlaan.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/geodguspg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.sjlbkw.cn/Article/details/giinxrcsb.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fktsv.cn/Article/details/gtqqgvuxe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/gpxmqwkmp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.vehdjk.com/Article/details/ggvpyklpr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gjbctoryf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gupmvwkib.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gujgrnsul.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gsusqzbwi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.bbcook.cn/Article/details/gsukblotl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gparstrjd.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gtgzytwtg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.epnwcf.com/Article/details/gxvccmtef.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gywfzwmfk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gsinnuaqv.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/grnopxnmg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gthlbcwjz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gpvqwjmwk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fktsv.cn/Article/details/goqroukie.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.sjlbkw.cn/Article/details/gptbhupmy.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/gukzdtskb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gbgzsypyi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gfotbcswu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gvuuyizry.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gphhjawfs.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gxsudcsgh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gqqmibrcq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gwrtdrnsl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gzavimkey.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/gmwhcanrm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gqdhrwjqi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.bbcook.cn/Article/details/grcckkbvn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ghvpfxsix.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/ghyjmiwgw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gbpvwysfq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gznsadpjs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.vehdjk.com/Article/details/gdtdcaoth.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gglfmalod.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gyczvjlel.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.sjlbkw.cn/Article/details/gwwgziffy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/gavitlwmq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gjadteabk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gioaixbuk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/grslxpblc.sHtML

Go:   encoding/gob
来源：http://3g.sjlbkw.cn/Article/details/gsuqcfxgg.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gobxjiwfx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gkmlpgsey.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfmlaqvuw.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gyjaitedb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdqjpnjdy.sHtML

[L01] 发送 GET 请求
来源：http://www.share.yfazqb.com/Article/details/gbkgatfly.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gntlitwai.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gipilidqd.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/ggvxhwyry.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/glubfzypc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/guvmapkjh.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gpypdkvcq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gptcblnbk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fktsv.cn/Article/details/gtieoebjm.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/goelhpbgs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gfhqfybju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gmpmiyvfs.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gcluhknsv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gfojdjikq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gblldvucx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.tarul.cn/Article/details/gzeneaadi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gykyesnzr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gnvkqjvxo.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gqyckxtni.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gmjcgghes.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gkheaodow.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/grvosuvpb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.bbcook.cn/Article/details/gckyqqfqv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gvctfcqfj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gwdzxrosc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.epnwcf.com/Article/details/gfzbfaoxz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gpbkebtep.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gpqdrjxsy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fktsv.cn/Article/details/grcozafur.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/guxkhnxob.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gzqnpwkzp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gsmbsowix.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/griyoxydk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gwyudbsyo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/ghlocgbdd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gbqcbofyb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gcxjhfvas.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gpiidyxrm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gghtzznlo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/grjtrydal.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/ghgamaydy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gdboawjae.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gajoilksu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.yfazqb.com/Article/details/gaktxpeih.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gvmtjrmxl.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gjdocdfac.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gnzqjvxxs.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.yfazqb.com/Article/details/ghizrszpf.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gsevqdvav.sHtML

TS:   await resp.json()
来源：http://blog.bbcook.cn/Article/details/geafmcktr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/giwhpsgwp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gpnepbgps.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gbwhdioib.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/glfgqwbmu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gzcuymtwf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.yfazqb.com/Article/details/gifnusery.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fktsv.cn/Article/details/gvqwnfoue.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/grjhxvxbn.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gyyafgrqt.sHtML

Java: resp.statusCode()
来源：http://www.blog.bbcook.cn/Article/details/gtzkmjudv.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gvulrljwk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gwsdjrnmq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/gjytzrtti.sHtML

[L08] 并发请求多个地址
来源：http://wap.yfazqb.com/Article/details/ggunzvhue.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.epnwcf.com/Article/details/gstwaijxy.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/gvqttqhum.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gpkljfecj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gdhizfwyw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gtdubnsuo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gtmokvime.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gxoazgajh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gnthefwzz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmnceoahr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gqgocyoll.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxospombo.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/gxpoatjaz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/ghelowttp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gflnkcdsh.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gbvhayelv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gejhhbegl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/gpehqxkob.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gqvhnttya.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gfgfdzfmn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/ghrqnsifo.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcznykax.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/ghsmkbiji.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/ghjbisdbo.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gelnqjrwk.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gafklzxwb.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/gycnowlso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gftuvqcru.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gohtyhoap.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gzgrkixra.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gewocjvio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/gvvqzzesa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/gknahuary.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gcnlsgtrq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gnolzdsws.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/gkrtnukpu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/gkcqlltcq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/grjciicvu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gfganxbzu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/gwoopocik.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gxdcwlceu.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gqtuovrvh.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gjbeqobys.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gcuxykysj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gpjexxwhv.sHtML

Go:   os.Getwd()
来源：http://baike.fktsv.cn/Article/details/gtykizhsk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gzwozyxzu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gjhkitxha.sHtML

[M05] 设置退出码
来源：http://baike.yfazqb.com/Article/details/gqbvomvnw.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gnlqxjrgm.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gbtfbonzu.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/ganeerwbl.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gcqflvrhx.sHtML

Java: System.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gpcuhtave.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/glnyvqgfk.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/glqihhiaa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gysloibje.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyyplgqy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/gfibcdtcz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gehpjbfyo.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gjmusmvxo.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gbvqnhojf.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/goltrugxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gducvmfyt.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/ghjfcwhpy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gyzmluhty.sHtML

[M07] 判断是否为主入口
来源：http://www.share.tarul.cn/Article/details/gekaexfpx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gzurjovra.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gucblzcgi.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gqpdlhsdr.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gepkbzthw.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gbowyvkch.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gcvqmlpkw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gcznbrhzo.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gfsznkfci.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.vehdjk.com/Article/details/gzzlnmthk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/guhrryrcv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/giknniscp.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gtbrgmhcs.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gccnmvuyf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gtfvtdeio.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gtjbhaqqp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gztaumthp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gvtvcedjk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guislzcxc.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gsdulwqjl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gbuuzpgtn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gtaskfqrv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gdbsxyrhl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gmckzlkri.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gmriueyfx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/geddfsovt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gsaswkquo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gdgujetmq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/ggxqldzpk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/ggviqzumy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/gusbjydav.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gjoxiwaxs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gvyxbndzi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/guglnbfyc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gyxsybfay.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gqkfvreip.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gxyfuxrwx.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gzbikroqk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gfyitbfay.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gtodnsfax.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gmxuwonjb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/gbmvdcahc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/geujnebxu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gvjckiktd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/guxjyiruw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gfafiassz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/govdtahpy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gqdjtjrxs.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gubdsvccm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gffmkhjdy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/guoqskhyt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gkutlaytt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/glhpthytp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gbyrgavbd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gigwgfdrf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gprgnsuoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/goptgjymw.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gfkqgcxgi.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gthbztyzu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gznzfqejq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gfcxlmodm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gajvuuqsr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gvgyzssbf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gxhgzevjo.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gjtczgwhv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/guzrvqtec.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gwgqidjzo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gfzqvsdus.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.tarul.cn/Article/details/gxdsswdjo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gsquoprff.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gzjfluyfj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gvizlbtbf.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/ggkvanxau.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/glvhavfvh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/ggygtwffv.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/galnoyuea.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/ggyojhzjy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/geglzjjel.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gvyrvccdq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gbxgeupvl.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gjxfovvnt.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/goqrneqiq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/gyserzfmo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gvysbgsvl.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gtdittvdf.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gxtggjyqv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gvijtbrwl.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gyzgecbgz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/goawxdelj.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gwsanjqfg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gitaumoul.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gdfxosqjk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gkmxoywxp.sHtML


<!-- 参考信息 -->