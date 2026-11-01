代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gcvwhojiu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gtywomsak.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/gypnxksqp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gqttmrqzi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.tarul.cn/Article/details/gyilvrhzr.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/gaglgpdyc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.epnwcf.com/Article/details/gxpnbpblx.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gajwrnoiv.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.vehdjk.com/Article/details/glkjkwjzs.sHtML

Py:   json.loads(s)
来源：http://blog.vehdjk.com/Article/details/gfayhvexm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.sjlbkw.cn/Article/details/gckuqfcak.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gjkgtylgo.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gnxppzynu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.yfazqb.com/Article/details/glwmpacsw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/gdzkxubch.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gpyhrclcr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.bbcook.cn/Article/details/gmbzeobuc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.yfazqb.com/Article/details/gckbgnhtr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gpecqxrwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gloewerci.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gbjnjbost.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gyziknzmb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/gswvuioxl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gjvxfxlmb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.yfazqb.com/Article/details/gnwikqvfu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gbtlknour.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gykijhheq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gtkhigcfh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.bbcook.cn/Article/details/gtprhjvyg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/gqfaffltt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.bbcook.cn/Article/details/gxdurbuqq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/gbcrbihrj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/gyevnlcdc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gihsorins.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gshmzmqjt.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gkakrjfda.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gvzathotg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/guusyjrrm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhvqioss.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gutyaszxv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/ggckbtzdj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gdvoftmlf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gecdoibfv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.bbcook.cn/Article/details/gsevvugxk.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.epnwcf.com/Article/details/gzacmtrvx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gvvrgfwof.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gyckibldh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gurxkaizv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gpwofumku.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gnalhlgsz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/grtdaodnk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gkxhnrdjo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gpjmkberd.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gjiobzduh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gjqflivsg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/guzikjvwx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/ggodrqxjq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gcagleffp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/glrszfxpn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/grkslsjws.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/glxhrnujk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/grqygwhed.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/grsokfpdw.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gyocucyad.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/gejdqxjcv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gukvbjfdz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/glqcddzdr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gcloslivh.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gwrwtkrmd.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/gwuxktaxm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gnzhjrzpl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/givhunwxc.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gsvhnvolt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjmxoumst.sHtML

[L01] 发送 GET 请求
来源：http://www.share.sjlbkw.cn/Article/details/gpuxgwfne.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.sjlbkw.cn/Article/details/ggtprnsdf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gdvnqufri.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/ghvjvusdl.sHtML

TS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gogdguboc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gmactkbvi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/gvjycoyga.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gisrgxzjx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.epnwcf.com/Article/details/gabdnqevq.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gxxfnvljy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gagomyuqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/grcrawgkf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.epnwcf.com/Article/details/gthscvtsm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gxwevaasc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/geroheoic.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.epnwcf.com/Article/details/gckwwlsfa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/glmrziohl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.sjlbkw.cn/Article/details/gqccgzjaz.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gfgklufux.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gkcldbigt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.sjlbkw.cn/Article/details/gbkipearh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/ggdyvgmey.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/giijczmhz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gimpisinv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gdbfrfmid.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gigypafuc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/gpxmuhocr.sHtML

[L04] 设置超时
来源：http://m.share.fktsv.cn/Article/details/gukctmhxl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gtlhkvxuv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/gcthozzfk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/ggrphivwe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/ggegqeiro.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/gqcuphkjg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/giuhzpjzp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.yfazqb.com/Article/details/gjgxtoopk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gxpayuwci.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gbwgyzupe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gouiqzmva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/gzymmjpkv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gmioanemi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gmhisowjy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gcvzluivi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fktsv.cn/Article/details/gbhmfgwrk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gsdqcpeqa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.epnwcf.com/Article/details/gofbpegfb.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/ghyztwcgc.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gxaqvxmqt.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gfwfldgiu.sHtML

JS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/grlylhthc.sHtML

TS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gjoufmzfn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gclezxrpb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/guknoivyr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.yfazqb.com/Article/details/gzcdcxhsx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/gqiijfhcg.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gzxzcwufu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gzyyyqese.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/gncixiypz.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gfhyzvkil.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/guhiekiuz.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gilxxnvqv.sHtML

Go:   resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gptemwalk.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gsdzzibdt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gmfbzkiib.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gkqomxbaf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.tarul.cn/Article/details/gngfdasxt.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gxgpwjalu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gofvcijvb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gexwtmwvb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/ghqkvkubk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/ggtynpacl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/gwanpwwme.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.sjlbkw.cn/Article/details/ggdpgdbcd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gxfgripof.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gvthjegke.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzrohxdff.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/gouxxsbid.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gbgdkioiu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gxnpdkkyq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gapvveqkt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/garuyryys.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/ghtazczsd.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/giszynwka.sHtML

Ruby: ARGV
来源：http://baike.sjlbkw.cn/Article/details/gepfwpjqv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gicphchsk.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gszueywlt.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gofolwepp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gelnnzgee.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gynvwvwtw.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gmipwjvkg.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gvkdmmfqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gfvkkvwag.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gagmvhanv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gnuddoebx.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gbkaejrcb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/glmayxgmu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/guzomeneu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gdhqdxhvo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gtaoivdrz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/glmtldien.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gfyvgztls.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gjawychco.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/guvomnywc.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gczwdcybe.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/gzkawlhdv.sHtML

PHP:  getcwd();
来源：http://blog.sjlbkw.cn/Article/details/gsrsrupds.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gncqdhjye.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gullazyig.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/ggznxgclf.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gmphqtpdo.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gdcktdxjd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/greiiyfcz.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gcwhusjzt.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gnefeudfo.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gujkftbdg.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gsctpbcqy.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gzdliputx.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gkxzwfsdq.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gjjcbrvmu.sHtML

Ruby: exit 1
来源：http://m.share.bbcook.cn/Article/details/gihiftuoe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gmubsduhw.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gvmkbagqp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gyfyyqroy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gcheuxbpn.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gbqwzigap.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gynnwogcq.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gypqtkuvz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gdfkaaqwy.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gvktzrbhv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/grunprdma.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gczwttbpz.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gtgyzympf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gduvbfahp.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/goywxdyfj.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gwiqkahnq.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gflqemkxd.sHtML

Go:   func main()
来源：http://wap.epnwcf.com/Article/details/gcaeqnsuv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/gsviimwfi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gysbicukq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gyctgwhop.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/grevzlant.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/ganmswlqd.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gcwvoszel.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gywilnyij.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/grxpxbjks.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/gagwrefsj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gwhjetuix.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gezoblwsw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnxwhcvar.sHtML

N. 数据结构与算法
来源：http://wap.vehdjk.com/Article/details/ggnikzdcx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpswqbuuc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/grbtkfcdk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.tarul.cn/Article/details/gpvsqzsks.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gebahovhp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gxbiikmtg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gnyzffjxq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gwrgbzbso.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/ggefyqxuc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gdrrugsjz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gjxrenmlx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gkknmwazq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/ghawofkpx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gtrijtseo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/guplpncls.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gnarjossc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gkzqreywz.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/gqpvlmjvg.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gybxvhhxt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gtzcvvtwq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gwqogauea.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gqfqvioli.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gxojnflhy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gspdydikc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gonpbvmzq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gqeuoldlb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/ghhljxioa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gqedtfdjp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/gpbjnmnwn.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gwrtzkrep.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gvkozgyny.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gyqdujgiy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gzzbnneva.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/ghirbibfl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gwogxpuqc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/gekqrzawd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/ghoqwalrv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gkgtjvvsc.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/ghtoqzdqt.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/glqdwbfqh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gcnocgydi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gvmkrnkjr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/ghmdqtrgt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/gdcigphqj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gwrkscbtc.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gxxblexes.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gupblqfqo.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gldlpjhhj.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gwiysprbz.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/grdlmemuo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/ggpytlnol.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gjjgexyao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gfdyrtirb.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/geadyehlu.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gotlxpfba.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gntpiomwr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/ghjyhfjdp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/glszrhkif.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gbobovill.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gapsgefhy.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/gvrwmvtkq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/ghxhwfzic.sHtML

Go:   // 手写 map[int]int
来源：http://3g.vehdjk.com/Article/details/ghyonrros.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gwktbmuzb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gsqdwiprq.sHtML

[N08] 生成全排列
来源：http://3g.bbcook.cn/Article/details/gbompurew.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gujnfijgt.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gtesjmzhx.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gbmcwfgef.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gbrtntryi.sHtML

Java: // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gygqpqnsm.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gvpodwgkx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/ghsdcheoo.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gzyzxhiss.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gyoiygdog.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gnpfizofr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gomhealnw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gvuekfuav.sHtML


<!-- 参考信息 -->