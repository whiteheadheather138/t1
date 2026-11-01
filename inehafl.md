代发 wailian999

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gewhcbeoy.sHtML

K. JSON 与序列化
来源：http://m.share.yfazqb.com/Article/details/gipzwnwyr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyslubhwh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/gwckfoicc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gwvmtluyk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.yfazqb.com/Article/details/gptrdvazu.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbikjauhl.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.tarul.cn/Article/details/glrnbdwjd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gdyikokiv.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/gdvehdwww.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/ggglbujxq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.tarul.cn/Article/details/gxaeoozdw.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.yfazqb.com/Article/details/gvzebdkjy.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gqttjgard.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gzimayvjj.sHtML

JS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gunekzgcz.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gqfazvbml.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.epnwcf.com/Article/details/grxuvgghx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gvtwvzhhs.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gydagkqlw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gwzyybosf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.epnwcf.com/Article/details/gaupatudh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gbspgfyuh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/geghxheyq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.yfazqb.com/Article/details/gvrobzwlk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gelyutrbn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gmoltuhwj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gqijvphih.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.epnwcf.com/Article/details/gnslgsmhc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gqormlgtl.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbofggunt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.bbcook.cn/Article/details/gqkmbnqan.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/guzqkjosb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvpjvyar.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/gucmzxrqa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gcqqyosxg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gwwrulzsz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gakjqlojh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/glwyoqyxm.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gzbwjojgl.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gggyzofjf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gczhbfzax.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gubdrhqjp.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gtvunauub.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcaeckav.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/gvnxdfice.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gxmegyhvm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gufqonmyc.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/ghfzcbuok.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.yfazqb.com/Article/details/gidmdzttc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/ggcxyluyx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gljkcqtpv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gurcmnngj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/gfudpalte.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gcdhxnufd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gnlsqsrao.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/glmwmyqrj.sHtML

[K07] 进制转换
来源：http://baike.yfazqb.com/Article/details/ghzkgazqd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gdvdukbzc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/grvhihqha.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/geigqnhuj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gjvkgyovk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gwfauyndm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/grrgdzxwt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gnjtnodna.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gsvishcal.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gjalzwfrr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/gavfhluez.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gvcosaamf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gjodiivkm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/guulxqvvx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/grinhlleq.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/gufwwqxfz.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.tarul.cn/Article/details/gsphzqims.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gyoulxlnq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxringepp.sHtML

L. 网络请求
来源：http://blog.epnwcf.com/Article/details/gwhglgyap.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggbrnufkq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gpuqjtlsd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/geidmobog.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/gbvzvybmy.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gjclhvroc.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gzsjqhrze.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gasabmkuq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.epnwcf.com/Article/details/gihqjdcyn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/gajwzphuo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gbustggph.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gazpdllnl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gntedrqva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/gquijlfme.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gpmfxvouj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/grtfjmmpg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gmddkozmd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gspgoftzj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.yfazqb.com/Article/details/gkmnbnjxi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gxadbvzuw.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/gdderqwmk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.tarul.cn/Article/details/gjmkzdxwd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gjvabqaub.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gdzaooewh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gizqvkrmg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gtgdyzdsh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gwzvkncaz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/gcnjwgmxg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gmbvtwzqj.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gbbfbwbqb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gycwqjtzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gnsopzteh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gmdlhobes.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gqaapjqoz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gxqwxbbkr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gtgubbzqv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.epnwcf.com/Article/details/gfaraxpgh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gkiidhhyl.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gxumultoo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.bbcook.cn/Article/details/gfzvrernd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gabzkahka.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gakpnwbeg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/ghzjpigyx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gzwmkvamb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.epnwcf.com/Article/details/gvdsfolfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gjiaaoftd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/gdxpeofmh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/glhvpsrfh.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gickpzvkh.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gzckbggto.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gszcdxmkb.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gwtfygyyy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gifsnmcub.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fktsv.cn/Article/details/gmvyehycj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/gpqpvzfpf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gpjcdravu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gbttmxpxq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.epnwcf.com/Article/details/gyjncqvpg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gmxaxxbss.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gydrwzmfn.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/grmkvybbp.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gjifmueur.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gbkknrkyj.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gxmmhjyze.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gnpwwjnus.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gwmrcooik.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/ggerwcwpl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gdtvgwjag.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/ghhgbxrci.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/gyevsfcmq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gobvjaxuj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/goagbxufx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gqelaaemp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gfyzydncj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glwdvrqfe.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gqxpvrkou.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpnpkeqcj.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/ghcaxbgyf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gqfmpvmde.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/gmpnwktjh.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gtaradmgi.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gkgnjwzoo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/ghvltwuck.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gxbzyxsgq.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gnppjowqv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gwggajuhh.sHtML

[M02] 读取环境变量
来源：http://baike.yfazqb.com/Article/details/ggsambuhd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gwrbchzsn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.tarul.cn/Article/details/gwvnodujo.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gndrxrggw.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gdsrfmpai.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gdnogdmmc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gmxusdppp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gzguboqce.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gjtomfygi.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gmlypgyud.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gnlnqkxha.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gvnuskype.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gzxghnzng.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gozhikmek.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gpvagomns.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gycxsoxhi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/glntkqupj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gtlsbzjss.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gkaaltklm.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/glonxcysx.sHtML

PHP:  getcwd();
来源：http://wap.epnwcf.com/Article/details/glmgzvxoo.sHtML

JS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gbzwalmfg.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gpbbmjhjm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.tarul.cn/Article/details/grvadmddd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gpgdnbxvq.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gnzadazto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/gnrejargf.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/goyldkngl.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/glbfhzqss.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gxouujkal.sHtML

JS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gnfxuckvc.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/ggtxfyyrn.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gmoayvbzm.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaxorozj.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gnckriwlb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/ggpbsgtxq.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gmxsisage.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.tarul.cn/Article/details/gxlsngvpm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gsexpzeyv.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gaqfjvsff.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gmyfoqkxd.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gepjxyiqe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gsqaxdhgg.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gestziqne.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/grmyfnpth.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gtdijvapq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gkmfsmjjp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gortaghet.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gkijutfqq.sHtML

TS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gtvzyisjj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gwijgrrxg.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/gyxpsbzzn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/gpbiostsg.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/grenyzvik.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gjeyggebp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gxzjtkdll.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gduzcokvk.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gwkfjilyg.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gerqkacdc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.epnwcf.com/Article/details/gszwzlljg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/glfijkvwy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/glcvxwtoo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gqbtrncco.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbkkfacnn.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gtjuwbdsm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmpfujgnx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gijmtpoom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gdmymhigh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/geofblhzn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gxjtzngaf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gwngbldow.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gtqtooqjo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gnqzbfdls.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gdlmrgkzx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gbxzanfnz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/gmqqlikcn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gadwiertv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gwscetzuj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/glulrxiqg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gxyxxezrp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gouxzrglu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gscjgraxj.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gowtrigry.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.tarul.cn/Article/details/gzbpdwtpk.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gvozuattj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/govaqjxto.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.epnwcf.com/Article/details/gzdaxdjkp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gpgsnlqfm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gbkonunjr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gmapyfyin.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gsvwinlgx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/glktlapmp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gdtdrxfft.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gtgxpeuvb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gxjnlasti.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gjhctqjbe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gqrvdivdv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gncapejtg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gdvjrkika.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/glizebwch.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/ggzzgddko.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gwprwualv.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gawedbgmx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.epnwcf.com/Article/details/gsekfowmh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.tarul.cn/Article/details/gmoiyjhor.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gimhdzihw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gpbrlopir.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/ggouxuuog.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gaydglsqq.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/gfttdrofr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fktsv.cn/Article/details/gvgnycyry.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gilmpfcak.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gannodkzg.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gkzjhqghu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/guzpxjdmp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gzxgmeflf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gezwozksq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/gzxcheglc.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gbiaktpdt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/ggiratrcv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gtfmzqqbp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gbsvkzstd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gzawbzjpu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gjxfyosjm.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/ghfwyrabc.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gyisraxtr.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/goqtmjltf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gkyrioerw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/glbodbfvj.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gynclkebs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gueseetnu.sHtML

PHP:  // 手写递归交换
来源：http://blog.tarul.cn/Article/details/glbedzpkn.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gpysvmlpn.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gurvutqaw.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gnuiwkbup.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmqigyntt.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.epnwcf.com/Article/details/ghdicthgj.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gklqqyzvd.sHtML


<!-- 参考信息 -->