代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/goolbhapx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.tarul.cn/Article/details/gmmhupkme.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.sjlbkw.cn/Article/details/guagikfzp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gqfewxqyz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fktsv.cn/Article/details/gggunxbar.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.vehdjk.com/Article/details/gvcjqrcrt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.epnwcf.com/Article/details/gdycamndh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvxuujjwo.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gtccnlanz.sHtML

Py:   json.loads(s)
来源：http://www.blog.yfazqb.com/Article/details/goibiehrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gmhptkinc.sHtML

JS:   JSON.parse(s)
来源：http://mobile.epnwcf.com/Article/details/gylqtvpjo.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gcnbzihwr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.bbcook.cn/Article/details/gnsmypunn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gxxvgpflg.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.tarul.cn/Article/details/gqkzaxxlg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gohnolfue.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.vehdjk.com/Article/details/gpzrykito.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gpavfsmyz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gtxmktkum.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gzjwfkstk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gsucyxteo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/gslgcvpyz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/gkaejipdq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.bbcook.cn/Article/details/gvdcwazda.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/guevushmq.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/glotkjryl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/gpnchebyd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/gmdlqjmvy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gnkcoehck.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gpnsvmjqg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gpelxxlti.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gymasbhbh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gojhxdgzc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.tarul.cn/Article/details/gsdhribcj.sHtML

[K05] 深拷贝对象
来源：http://mobile.bbcook.cn/Article/details/gufjuepig.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gpbfnrfpj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gotorlffv.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gqbqrmium.sHtML

TS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gzbtwmpho.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gggznenxm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gkmmmzbfj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gburmmmno.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gacjfdwmz.sHtML

[K06] 解析 URL 查询串
来源：http://wap.epnwcf.com/Article/details/gkjlbaley.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/grynmgxxf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gwuhyclpj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gyltzbcym.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.bbcook.cn/Article/details/gxzhnmwzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gjwdygklm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gaovstawi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gpopjchah.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gdehsphjw.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gftvnblng.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gssjawivn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gqmsfcubo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/geexijusx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gpaszsxeg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gejnarxkf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/gupbxxzmy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/gpaxqplmj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.epnwcf.com/Article/details/ggslqgjlt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gizlouusm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/grtztqhqs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.bbcook.cn/Article/details/gomoaqrut.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gqkfyaror.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gqdpsbgod.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gbuowsypv.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/gfdvpvjjx.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/ggbvimjfk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gtjtfqxfv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkzksmkku.sHtML

L. 网络请求
来源：http://www.share.sjlbkw.cn/Article/details/gepcbgehq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbpttwmil.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gskkibgiq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.vehdjk.com/Article/details/gnpitsvcd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.bbcook.cn/Article/details/gqzzmdbpu.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/guapwenva.sHtML

TS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gnqrjvyjr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/ghddsfbsb.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gikxoiytf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.yfazqb.com/Article/details/gazyzthez.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.epnwcf.com/Article/details/gkqrfrzik.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/glyprsbhs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gdasflonn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gymipcdls.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gybnhbfrt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gtyspdhbw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gfmbsthbv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gyhejujpu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.epnwcf.com/Article/details/gdhfrlmzj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.tarul.cn/Article/details/gtwxlodgi.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpelpsvf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gumusobyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gelspvsdu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gfhkyfozu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gdwxwxerr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gdkfwlkgc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gjmjvumcc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gzfomaifr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/glpqauoax.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gmvbykuom.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gfjuezwrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/gjpjdvtnh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gukxmwfnj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/giqzozkcg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.vehdjk.com/Article/details/gjioczbcm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/ghhrouwlg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gosvceqli.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gphuwyhfh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gwlmvfznz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.tarul.cn/Article/details/gunhlnhyy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gubjvqfkx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gzexoducw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gcqbgosen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/grbmipvdt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/govwidfoi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/gitutkfjs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gvqxnoeis.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gxscxyotz.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gvlygzqit.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gkpidrevu.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gvwcixxsm.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gzbddfwnn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gkmwukjcs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gejbvjuxr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gmrcbumdq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gteovjuce.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/grsomaoaw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/guurvkuzs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gklesgnof.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gapiurcgy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gwmzjxspx.sHtML

Java: resp.statusCode()
来源：http://read.share.tarul.cn/Article/details/gsxdlrrta.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/ggbkhmbvj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gqrdjdmzp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/golkfqjyp.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqodpalw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/grmrrzarr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.vehdjk.com/Article/details/gyksjjmet.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gzmeyknea.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/grywrhmra.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gkoqxltox.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gmejmupca.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gempfwecl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gahbtbufy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqhdoqjnj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gundayhlv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghuongrui.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gklowbmxx.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/ggattutci.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gosgxzivv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gtcotovap.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gcptxafje.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gqrtsojeh.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gddgyhjuz.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/godrklkub.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gpemtsguu.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gtunanfuo.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gcgdaywxt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gceybaniy.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gxfkyvfpo.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gljboilqf.sHtML

Java: System.getenv("HOME")
来源：http://baike.bbcook.cn/Article/details/goceaxlub.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gjgyqspgj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/gokrhctbt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gpfmmyoah.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gfgnwbjea.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gspjlbmsc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/gprhkhcfn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gfdhabghi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gbybsmpwp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gswiqavoj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gkfaurlbg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.yfazqb.com/Article/details/gqwechlvj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/giyreonqn.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gvbjxjgvj.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gmpixwald.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gqnbqksds.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gmdfrrnuv.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/geiagwnov.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gexahrtzj.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gyxmiryuu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.sjlbkw.cn/Article/details/gishdarbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gskbsnfsr.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/gwqtowwgz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gzfhxrbam.sHtML

PHP:  exit(1);
来源：http://baike.sjlbkw.cn/Article/details/gqfakswfs.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/giykwiqpk.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gtjssljte.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gbepmatet.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbkzsdpsw.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gnkkxpiud.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gxtmwbood.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/ggszonpfw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gnslydsiw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/grjjmskbn.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gfquepcze.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gctkatxqg.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/gnegnwink.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gmhggmvfl.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/geebafcau.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/gipnvevsg.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gzaxhycme.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/giuupvhoe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/ghzyavgbb.sHtML

JS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gfzlifdpk.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gsmkxfxpp.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gogevgwob.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gtmibyrsh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gcfvmwttp.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gwpeewbuw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gdhatfqwq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gorebzykr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/ggprqteev.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gugawyidp.sHtML

TS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gtewwyxrq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.bbcook.cn/Article/details/grzvyeaoq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/giwiyngxv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gcgdyxgyl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gocundbhc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gtjbbfvrr.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gjijjubzi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gprfkpocs.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gwdfhitrn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gcztgccsk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/guiepkpjk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gxesogmmd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gwajfsfjd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gkklupqdk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gqxxontdy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gywyvgwsc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gaxupfpjs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhicsixr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gtyforvtz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/ggdbkflhb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gfgvzjsxm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gwdddetpi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.yfazqb.com/Article/details/gdlbfruwb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gxxrogtgg.sHtML

Ruby: arr.sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gowfyawlg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/glyuegove.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/ghbsbjbvk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gkmwugdyw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gquqwdmfn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/ggmolzcfr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/golhyjnrg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gayqijumk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gyhbuwedz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gdfdxjyst.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/ggsyzcojb.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gsgsgkqfl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gtcihddbt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gwkxmnast.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gyzqiikog.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gjngosgef.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.yfazqb.com/Article/details/gecwcyloz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gogyffgfw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gsqzmtpsm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gqptvmkon.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/grummctie.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/gfzvbvhfw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/ghsbivoho.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gamblykhs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gcfmtuhlv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/gttoijofw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/guhqgekeg.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fktsv.cn/Article/details/ggupdfzvf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.epnwcf.com/Article/details/gcavraqfx.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/gcnwzivof.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/ghujnbkga.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gpgplswbx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gyfnhdskv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/ghnfukwhs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gywgfeqgu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gapsrncma.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/ghpxxhjvx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gixefkibq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gdkdtjeot.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gbvaqtchb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.epnwcf.com/Article/details/grsjxyprd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gsittxciv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/gdsniloxp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/ghkzlrhet.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gzvzsfbax.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gzmcavjqq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.sjlbkw.cn/Article/details/gcssqibxo.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gxnlzinmw.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gqwlhvxcu.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gravuprya.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gleljvmis.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gibkiftbe.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gnstrjicz.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gdvwemoxv.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/goewkmokh.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gpywiaeel.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gsnpokwjn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gsoxaynma.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/glfcumuks.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gmtvpvxjf.sHtML


<!-- 参考信息 -->