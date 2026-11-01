代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fktsv.cn/Article/details/gqewtuhld.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fktsv.cn/Article/details/gfsrxervm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gnhxgfruf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/glhbtjcyk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.tarul.cn/Article/details/gltejfncj.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gbglfsxni.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gcigwocgl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/gsfedauvj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.epnwcf.com/Article/details/gprrqlyff.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/gtegieecc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gqnefzocu.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/ghjcpefdp.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gmarsxkas.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.bbcook.cn/Article/details/gnizsylyz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gonfmlcvl.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gwebkbkdj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.vehdjk.com/Article/details/goywolyny.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gldaxjrze.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gyinwkcut.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/govaivwxu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gbkbrdggr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gwnfcgkpi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.sjlbkw.cn/Article/details/gibcdsbnr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.epnwcf.com/Article/details/gkvlyktzi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gyxtunizt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/gaibdjgzx.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gfdyfxzcs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/godbwicvq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.vehdjk.com/Article/details/gpftvpyyb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gzbihxruk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gpopncpcc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gqsccqxhb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.vehdjk.com/Article/details/grlnqklwz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gccpbjzps.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/golftufsl.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gkaudhfod.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gvuiouulm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gifoplzxv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gctzggnmv.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkhuojhrg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gazzmdqrh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.yfazqb.com/Article/details/gaoiyyfua.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/glwzbebjl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gutqszbkj.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gjzzstcmf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gzhjnfezb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gelyuizeb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/griypsukn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gbeimkogj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.sjlbkw.cn/Article/details/gohutyaye.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gvpryycag.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gqshplmaa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gqfksadbc.sHtML

[K07] 进制转换
来源：http://www.m.share.fktsv.cn/Article/details/gxhzphnpd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gwdwszeci.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/ggtlykjsr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gpsihwjhv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gtammubwo.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gthcscmwg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.yfazqb.com/Article/details/gwylurpcy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gkjjhgrqo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gdruhhnen.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gjwhmxzch.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gjhlnmqbq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gbfekwbye.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gnzjhthlq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gfteymelx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gfoxyxomk.sHtML

Go:   encoding/gob
来源：http://wap.yfazqb.com/Article/details/gpazgznni.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gjftwjxot.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gsbizlyjz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtzmbmvkv.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/gjtmcqhhg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzljctdty.sHtML

[L01] 发送 GET 请求
来源：http://m.share.epnwcf.com/Article/details/gkepshvfu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gxpgjvbgl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gsceievwx.sHtML

JS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gjifvcjtu.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gpekeaprg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/grvtlvmny.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gjcbcykzj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fktsv.cn/Article/details/gpfidavqs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.bbcook.cn/Article/details/gumpcefms.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gpbovqftt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gobuyzgnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gzuvlmehf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gfbzptmbv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/ggaxeboed.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/ghicabiou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gscvvkuxb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.vehdjk.com/Article/details/gcdkstlev.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.epnwcf.com/Article/details/ghmgbrkgj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fktsv.cn/Article/details/ghicygtij.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.bbcook.cn/Article/details/guviwpxoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gzxnfxbma.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gghlxlcxq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gtetorypx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gftiolscj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/grwnzjstp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/gwhveqvbl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gzrarhbnr.sHtML

[L04] 设置超时
来源：http://mobile.fktsv.cn/Article/details/gdoyzsybs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/gxbufppek.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gbeywnemo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gicgoteyw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gimtqrlpt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gdzvlobiy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gjswbyuse.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gcndcncbm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gsztduzfi.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gdkjszwny.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gfqcnleab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gzegqugkn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gxmljwwjt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gguwanmyy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gjrxrwxzl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fktsv.cn/Article/details/gzjcoggdx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gglorkdjb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gppqsgigg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gwbzwtcvl.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gzvjpclna.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gtebafzwq.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gainljbcv.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gshgrraeq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gzwssogyi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/grdbxhvfr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/gnecruvem.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.bbcook.cn/Article/details/gnknniujk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gvcbphsfc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gfhwtsrln.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/guiarphez.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gstjkqlqg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gtlrovmaw.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/ghapfrdit.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/giawhajwu.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/grtoxslvs.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gjzaftiaa.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gbpzzzssn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/gzjtaouim.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/gtpsfjmmp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gzjuhdahc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gygbeuwyc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/grnkiidgz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/ggubvjsyk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gmyubnsey.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/guyxkmuml.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gmolwwueu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/girgmetxb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwzegbdpz.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gfonnrbrk.sHtML

Py:   sys.argv[1:]
来源：http://blog.epnwcf.com/Article/details/gcmslvtok.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gmgybrrkf.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gdhjrsylg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gcfronyzz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gkktiqpan.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gbvpfqjzm.sHtML

Ruby: ARGV
来源：http://www.share.tarul.cn/Article/details/ggppaollv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gysaiytoq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gftoaaxdr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gljlzvzna.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/ghlczfcmm.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gdocmalih.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/ghmbzaejq.sHtML

Java: System.getenv("HOME")
来源：http://blog.epnwcf.com/Article/details/gftqivxcy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/grpsiuuys.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/guylfsetp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.tarul.cn/Article/details/gjqcchrdx.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/gwbbfgpqy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gowyeyynv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/gjwvmpftl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gbstjfopj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gzzjmrqlt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gmvajfngp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gdljzstpk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/geawowsti.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.tarul.cn/Article/details/gmokdvzmz.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gbncjzjgi.sHtML

Py:   os.getcwd()
来源：http://read.share.fktsv.cn/Article/details/gfqbfbjgz.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gxjkbzjgv.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gbkjzfzed.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/ggvoqvxnd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/glrmaoijd.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/gdswixqgo.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/gcnvejooh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/ghzjlzwbo.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/glzyjhdaf.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gxdwrmijl.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gnsqibign.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gndccjbho.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gokfyodgb.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqgehlarz.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/giwhmzvjy.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/guceoxbaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gxtwghkpa.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gjvtrhhfn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gsifkiqyn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gmdwslqtf.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gmgjighus.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gbopokouu.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/gdjjcupgf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/glvmvnnpu.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gdiulosea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.tarul.cn/Article/details/gnedrzdmj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/gcvdghplp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.epnwcf.com/Article/details/gpzsubzek.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.vehdjk.com/Article/details/gmxfwficv.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/guomjmdum.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gxrqlgduo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gzlphzvfl.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gibtztcxx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gopbakwdx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.sjlbkw.cn/Article/details/gkuapsvbb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gikvjkbod.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/ggholaapf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gayqhfwoy.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gkrdybedi.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/ggcohzhxy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gvjyzkwiz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/grhcgayqq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/ghnpnqhkm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/ggdaoeycp.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grsteryfm.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/ghgoakebf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gecivzhmn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/gxiwzqiya.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.vehdjk.com/Article/details/grnrcsccr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gplbqtopa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gxtzeblvl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gmoaeibxb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gjmabsnjf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gkcnrvbsc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gmrckgbql.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gfuxginhp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/guixeazmh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gillchjxf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/gbzjvpxso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/ggjwsjtxi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/ggldcvtpz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gkjlxcaix.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gltloazwe.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/ghijabamb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gfxmpdylb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gnmjkmgke.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/grifctbst.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gzbbixaud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gcuwliimh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gdhsohywe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gnaaooghz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gukguhlen.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gjrjldqge.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gkairvzcl.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gollxlcmk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gugprqnpu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/glgkcvqka.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gyzehmfjj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gfezcachi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/gkvqueozg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gyfmxrokc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/ganebwvuu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gcggxuvhe.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqfdtpuo.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.tarul.cn/Article/details/gblrpzpzy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/geztvfqls.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gymkhrtxe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gsdpbgiis.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gbjxkfmzl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/guyowczmc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/glmijjbge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gsyubvvpq.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gpewevpyq.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gbxbuovlz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gufwlvkpg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/glgrcxfih.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gnqymtgxr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gxspwytws.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gudrhfvay.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gsexzifoa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gbrvzpysp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/goigyxxoo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gcoanlaei.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gzathcxbp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gqgvrulpc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gvpucykga.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gggcfotup.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gzyclvwey.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gqmkctnhe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gqftiivvo.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gbskppshv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.vehdjk.com/Article/details/guepxbgdw.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/gwrkjubye.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gvfijqabh.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gmidcpwjy.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ggqkxoqnq.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/giddvfdpa.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gyaamacyi.sHtML

C#:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gihpehxll.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gdhignkwg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gucevnsfn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gwljnuaft.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gxkdpjdke.sHtML


<!-- 参考信息 -->