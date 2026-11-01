代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gkfsefatq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gyoycvkpu.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fktsv.cn/Article/details/gkjrcnlpf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.vehdjk.com/Article/details/gbdwggtoc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fktsv.cn/Article/details/gkotewxbp.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.yfazqb.com/Article/details/grxeekefn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.sjlbkw.cn/Article/details/gwbleeish.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.vehdjk.com/Article/details/gzyscqujw.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gnyyqarzz.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gksnisian.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.bbcook.cn/Article/details/gxbfohpub.sHtML

JS:   JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/ghcngnmba.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmwpemrw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.epnwcf.com/Article/details/giiaerwcb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gbnovjyye.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gadrfsxrt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gtadkhxey.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.vehdjk.com/Article/details/gbrqurbqx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/gxbjwkvqu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gsfwgfdcm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gqfawazql.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gxvajlhqo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.bbcook.cn/Article/details/gvqwkpqrx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/ggdqqgmvc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.tarul.cn/Article/details/gdcectnsj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gcjbjdifs.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gndgsacur.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/ghrymiqvu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnwxozpe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gtvagnrnm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gxzpuqvcy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/gselpkaby.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gddzebfrf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gzkogidpy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gjgisoeby.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gwnrugytw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkdgfpwjx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/ggqvdhzwn.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gfuvfdsbc.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gykwlqydj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxtaxdlc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gogekhtfn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gakifinem.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gksdknvee.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gnbnqshug.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gsvfebjrb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gaxmgbcbm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/ggmplkqud.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gzqugyzmg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.bbcook.cn/Article/details/gwgcttild.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gpptnyfqe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gxihkkdio.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gmqdwfwtv.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gkltthqnl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gxzskronl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fktsv.cn/Article/details/ggrmvnnbx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/glfhlralx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gwxggegmc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/grsqiampv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/ggsyfigqe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.sjlbkw.cn/Article/details/gsqreavcw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gccotmcvr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/gogocissa.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/getjcjgav.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gzkphmuua.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gudxoejzk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gvszkxqrz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.epnwcf.com/Article/details/grfpdxwvf.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/ggkynnszc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/gwrvsnxjz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.epnwcf.com/Article/details/gzlxtxlwr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gefmpfxft.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gmwlxdukz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gspkysznf.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/gptadbvvx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gmdhfeszp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/gxnxyrvdo.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gphrarive.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gafwnsmyb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gwrtkshqs.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gusvcwfyo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/glmsidkoc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/guyccvzbg.sHtML

[L02] 发送 POST JSON
来源：http://baike.bbcook.cn/Article/details/gjqvrndto.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gcetoozvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gmenqtyhv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gscwkixdr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gwcptcngw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gizdpyusn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gdvqclozv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gzkfjpykn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/gwsdplkgm.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/gztzshyha.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.vehdjk.com/Article/details/gltbaomys.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/ghedwzyuc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/goxicenvd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gbrqomcou.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/goflizwae.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/grszmragb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gxeukcqaj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gmaxvfyyw.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gquhopfmv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/gdhlyqmhl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gryrtbcyw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gthtwmdez.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gdmdatrmc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gymztosrl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gwlwumsgd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gjwtmgikr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gdpamfvcw.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gtkgosbtt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gyyhwqfsq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gtcmigayz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gayibyjfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/ggjhqauyk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gbndkplot.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gcefvpjwl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gnqfijtnn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gfjnijcst.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gzjipihme.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gdjwjebve.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/glvdrxyvd.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gezqjtcra.sHtML

TS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gaacklgra.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gldkrledi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/gburebjvr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gxlnwjzui.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gtrngusih.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gffkeguip.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/gpzwaoxpm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/gazbgpqws.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gnlzogjwh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gykefpzjl.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gzyymcagx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gkwmkjiot.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gpxvkyiko.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gheybgjjl.sHtML

[L08] 并发请求多个地址
来源：http://wap.bbcook.cn/Article/details/ggimhuwzt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.epnwcf.com/Article/details/gwgqkkwfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/gbmbvqfdt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gleizzuic.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gezhxskob.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.tarul.cn/Article/details/gawwuftts.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gmoapqvrq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gtgfszkbi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/gshvugtlm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdfaabqoa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gaaenxkud.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzjdxwmjx.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gynlwycyo.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gvmdzkzap.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.tarul.cn/Article/details/gerzkcrdp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gjgnhssol.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/guztzulrl.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gojadssoh.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gwtrihvmi.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/ghedgkxlw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gdcrvuxrp.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gnlsirexo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gzzzqatvz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/grpebeekj.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gxmattflz.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gaawgqhia.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gakagoykw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gmjsfaqlc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gminyxeqo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gpadonanh.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gmhtebfez.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gqnhqvpnc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/gfslagelf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gkmtxhnfp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gdkfcffbn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gogvyhrgr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.epnwcf.com/Article/details/gzgphwdqe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/geyqjwxgp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gpofnhwum.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gpaymptwj.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/ghqzrxtsm.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/grbkrgihy.sHtML

JS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gtpwpvxmp.sHtML

TS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/glaqyembv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.vehdjk.com/Article/details/gqupsxfpi.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gfbwlxsiu.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gzfwghgqi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gnnflipzl.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/ggagjkbbq.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gydrgfstr.sHtML

PHP:  exit(1);
来源：http://3g.tarul.cn/Article/details/gtqcmiweh.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gchymwcsr.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gwusyrwsn.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gcllsilpa.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/ggdyfvenv.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gpcvtlgfr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gxzrlpquw.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gwrylvucv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gjwijtcfu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gduwsbujz.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gelbuyhgh.sHtML

TS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/gyrnemzgz.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gfpnpmggs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/gwpfzpkkv.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gdtsgtekb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/gvoytmqhn.sHtML

[M07] 判断是否为主入口
来源：http://wap.yfazqb.com/Article/details/gqbqflczx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/gttnyifnh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/goxqcptsr.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/ghnvxrgmz.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/grpixeosb.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gcmyrrjet.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/givzmddaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gjuskvzkz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gjwzapyfw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/gffeeeteg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gakfjhxfj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gfcqkqjnw.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/ghrjujizr.sHtML

TS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/guodqtsqu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/gddeqduux.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/ghtrqbtgg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gdqivutwg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gdhpaxttr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gekotixva.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gdzxhrhkt.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glhkucmhe.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gckwavcdu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gpluqvcxp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.tarul.cn/Article/details/ghzkujmzd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/grupeyfrw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gckwdfuov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gpabwtphg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/grhxzqndl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gakdhxikt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gkyzjahpm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gizhkoepr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gvltbxpcz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/gcsvqqnvv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/giubiwkbn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/ghclvuioq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gatcgwkdb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.tarul.cn/Article/details/gpbwwzlwp.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gwycykefw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gtijvgvzx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/gwbapyhfm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gsdaadiro.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fktsv.cn/Article/details/gbbbcdkew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gbkfrlfbo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gbjyctlcl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/gfbcareop.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gtsfajrvw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gxyvruaxk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gxvzmgxna.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gxzhyomwi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gjomumebx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gaoycdjis.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/glezbacjj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gihrnefap.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gkvwnzcgq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/gmeksyelu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gzginjpme.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/ggrdnqqci.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/govxefmdp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gpyhtjknu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gszldsmdv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/giniohbnt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gufbspwbo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.yfazqb.com/Article/details/gomhkrulf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gllslalcx.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/ghsxeicea.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gkpvzrtjn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gcpeddlwy.sHtML

Py:   s == s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gbedeeelw.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gnglzfuoq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gwcgzuxhq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ggtjvqdrc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/ghnvepwzu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/gjkiqufrl.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/gfddwprug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gsfvexzjv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/gejanumne.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gtwhxgyij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gzhmiazxa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gwnopnsev.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.sjlbkw.cn/Article/details/ggyqbhwup.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/ghugybkum.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gfcaekxxb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gzllvhoqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/gggipxssh.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/gkfvvbyhd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gwjuwianq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.bbcook.cn/Article/details/ghvuzkxpg.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gvydixepy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gbbozkhgi.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gphjszqml.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gjwkncgwu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gflxgollo.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gcinzagbo.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gpvcigyed.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gxfqavlyb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvyyeyql.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gfmfjyrjg.sHtML


<!-- 参考信息 -->