代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gnftziczm.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gqscqlbki.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.bbcook.cn/Article/details/gkbxembkm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/glyynpmzu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/gccrbhqtl.sHtML

Py:   json.loads(s)
来源：http://www.share.fktsv.cn/Article/details/gmnfuzqby.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.sjlbkw.cn/Article/details/gqjtlomcf.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/giullosto.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gmrprilfd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.epnwcf.com/Article/details/gbbjdwxst.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwmncvxi.sHtML

Ruby: JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gjqgxlryb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.sjlbkw.cn/Article/details/gkenebqfz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gmepyymdr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gnxmyqeqf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gphhligln.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gjxfglejt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gewdxmilr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gbyotmwkf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.vehdjk.com/Article/details/gjuaakeyx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/goqxhkhvx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.yfazqb.com/Article/details/guwvlzjxv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gyoefkldz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.bbcook.cn/Article/details/gatypucdu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/grljapsra.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gtmhzbilr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gyopxruoc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gtbuecnwg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gpbdxhocd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gcbsblqos.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/geopmgtta.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gdqpdqoln.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gnbxzjshj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gfyxadeyu.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/ggzcvfhpt.sHtML

TS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gmkkdnutm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/ghtxjstnt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/giyrdsjpq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gzbuwtmbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gxpaqlfws.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gpoktgtkw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/gamjjxlzo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.vehdjk.com/Article/details/gglyaonff.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gerzqyhpj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.bbcook.cn/Article/details/gubeoshdo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.bbcook.cn/Article/details/gdmyxnkiu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gcjupagpi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gcjvlctoc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/ghdjppysn.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gmpcehmnw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/ggateykvy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/ggorpdbpv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gvibdlorp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gfenpomlz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gzcsiavql.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gztsnflcy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/gquguihjm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/grqnhzsqc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gxcmafpnb.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/goblmburn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.vehdjk.com/Article/details/gcyidbnto.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gnzriujab.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gknuypynl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.tarul.cn/Article/details/gyehyoksw.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/goiwhxfpq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/glgizcurf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gwjphjleb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcaurvsky.sHtML

L. 网络请求
来源：http://wap.bbcook.cn/Article/details/gxgqudtoo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggbtwgyqk.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gaqgozavw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gkaveyxmr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gfaohggsz.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gomdtupqf.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gxwuxjidz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gbkeiwiui.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/ghdtwmoan.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gtssvipiq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gsvuhziof.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gmejbjzzw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gesvmcyfu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gwfayhtwh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/ghygyfxob.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gxcfdnnvf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gutjvfcoo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.tarul.cn/Article/details/gsucizdrh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gyvpkcfou.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gmbickiiq.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/gunamzbhg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/ggfjfxgkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gdmgwbdnw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gsjrgaaqh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gevaykzqa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.bbcook.cn/Article/details/gedyweqpd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gzgzntwat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gbacrpjol.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gdwxthfqh.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/gatdagwhz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gebwudpkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gogoulunx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gbmessrsq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gdhowvccs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gavwwiemq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gixvkwzdi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gapodexal.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gzdkrpebr.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gnmgetead.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gfnuubfea.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gyllidlpy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gtangtwmn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gkafhapac.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gmgmmespp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/ghbfbbhxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/gedwmsdwh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/ggbfbnsei.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gyslamrfe.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gtawlhlzu.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.epnwcf.com/Article/details/gxhdxgzri.sHtML

JS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gjihclfwe.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gcouosnqe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/glymwggsg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gywuphdyh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gupkclbib.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gueqqbfzg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gnpqectbe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gvdjjjbhy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gqfjupjli.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gcjbvjlyv.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gmdmukegv.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gvgeqtnwv.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/gujqhqrdc.sHtML

Ruby: resp.code.to_i
来源：http://wap.fktsv.cn/Article/details/ghdbllaja.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/gtrswtpap.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gzphnomnt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gownwaxzj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.sjlbkw.cn/Article/details/gxnxkmxob.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/ggzyfnxqz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gkckqgfja.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/gjnunzbwd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/gsehqnspl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gqrjvqqdf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.vehdjk.com/Article/details/gaknehodi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtrtkjtqq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gaxrdyyfp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggpgdjpeo.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/ggdsgzfff.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gszrtzhac.sHtML

PHP:  $argv;  $argc;
来源：http://3g.tarul.cn/Article/details/gxyarupjb.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/ghwdlifkg.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gktmdfypm.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gakxmckxh.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gcwbobgwu.sHtML

Ruby: ARGV
来源：http://blog.epnwcf.com/Article/details/ggimopxyk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gglbzsmbz.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gibbtvzky.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gucwqhaiz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.vehdjk.com/Article/details/gyvqeqaeu.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gzpxkjyti.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gsculvxjo.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gdllqwlpb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gvuwnqneo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gzlvfsqzv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gprvkgojh.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gpedxvphr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/grderjnmg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gizuatmha.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gfgofvkdb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gvspxxsku.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gdsllmhdm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gaxmluoxj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gufvrflfy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/ghguvtevu.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gupvyduzt.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/gegweyebs.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gusfvjzbx.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gprunltwm.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gjyzpypos.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gybmdahcj.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/ghuygysiv.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gxnrzjtba.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/ghfhvmuxs.sHtML

[M05] 设置退出码
来源：http://baike.sjlbkw.cn/Article/details/gcdzqvbxf.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gbtcxzlib.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gevfhvcis.sHtML

JS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gmnolmqry.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/goofdczon.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gdmoiluke.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gqwtxcfnk.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gtvkcghrr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/gearksqdc.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/ghxkqjztw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.epnwcf.com/Article/details/gixfnoeci.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/ginhdmhhk.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gjhwwqysh.sHtML

TS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gslwcjyns.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gjyjagiqc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/gjcpyaefi.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gxauprvps.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gbvwffxhr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.epnwcf.com/Article/details/gzaqhfccg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gnqlagtge.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/gytejgvpf.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gtwhjfmbd.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gvgxiraxo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gjgsuxshq.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gekvzaqpe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/guxoferwe.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gobvfqlgg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/gvkcqkdhf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.tarul.cn/Article/details/gjozkqfur.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/gqnakaguh.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gtwzxsapv.sHtML

TS:   process.platform;  process.version
来源：http://3g.fktsv.cn/Article/details/gwwqbshfl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.sjlbkw.cn/Article/details/gnllrsqxo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gnfalpobm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gwdqfprmw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gdlhvepjn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gikitrhzp.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/glznlubhx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glkwpnvwe.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gyhpgrouz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gegccvgjz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gnuhqbfsc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gozeiwhty.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gniseuoka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqdkxbqb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gplfgckwx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gtlazfooe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gcspfsjqs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gzmfhjpuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gmouwibyv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gsufnygyg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/guuvksaer.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gidqeigxv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gwenbjwrb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gantslnhe.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gsrpwqdwk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gigfomfzc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gubbgzdud.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gghsrlwrz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gifxrllip.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gtopzhkye.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gajffxqxw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.epnwcf.com/Article/details/gzuouvsjw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gqageptds.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/ggmfqbyon.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/gqxaoocki.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gndyrmyjh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gmyruzwoc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/guzkgvcsp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gikzyzvno.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gfpeopjvq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/gkdeypmtx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/goazwgqco.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gzlimgdqd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gyziahskg.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gjhqgxsoo.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gjsbtfusq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gpyhhgvet.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gxghevrqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmherwlrx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/ginugctol.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/gcjqxfnie.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gccttgqoq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gktrblftv.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gunhzdmde.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gzueylqah.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gxbvhkyed.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ggcgehpii.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gpzbnkjct.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gndluvzvs.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gdnczojlp.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/ggooyjduf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/goiadkahk.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gcqamewao.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gvzfulvcj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gfqimvdus.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/grxkdbtmu.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/goxmvfoql.sHtML

Java: // 手写 HashMap
来源：http://mobile.epnwcf.com/Article/details/gztfprkjl.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gjwlthisw.sHtML

Ruby: // 手写 Hash
来源：http://wap.yfazqb.com/Article/details/gshxnrtic.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.tarul.cn/Article/details/gawzmxvup.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/giukkphqy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gguihsorn.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gdpjrdikt.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gcnzudyfq.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gtumxcpnz.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gutkjguok.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gdnscofvh.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gmdyuwkia.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gmejdntee.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gwtsjyijg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fktsv.cn/Article/details/gatiioutb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/glddkcoam.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gunyrfxlg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gkjmsgaoz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gbiyinqeo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.bbcook.cn/Article/details/gagtrdkdj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gktmhjtmi.sHtML


<!-- 参考信息 -->