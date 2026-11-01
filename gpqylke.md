代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnpdgozb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/gymplenjg.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.bbcook.cn/Article/details/gycwilpqi.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gjcxyrwvx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.sjlbkw.cn/Article/details/gkycoxxoq.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gpbixgvqf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.tarul.cn/Article/details/ghxwjxzie.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.yfazqb.com/Article/details/gzomyjzth.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gqgpimgqy.sHtML

Py:   json.loads(s)
来源：http://read.share.bbcook.cn/Article/details/gmxpdzggy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.tarul.cn/Article/details/ggttswpav.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gkdtyqlbf.sHtML

TS:   JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gajyejure.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gwixirctx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gabdxrgxd.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gvmpubgll.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.tarul.cn/Article/details/goqchbtkk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.sjlbkw.cn/Article/details/gechdwcfi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.bbcook.cn/Article/details/girhfiajs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gimwnuqrb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gligxebtp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/ganomkhil.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gytjydpnf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gnhzstlbv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gauwtevcu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/glxxaimkj.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fktsv.cn/Article/details/gjqoayell.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gediybzsu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gzoxvjpyv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/glfsjnvvl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gddevtcnc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gfvuxunbn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/gkmcyprsp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fktsv.cn/Article/details/gcpanjaei.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.bbcook.cn/Article/details/gykegiywr.sHtML

[K05] 深拷贝对象
来源：http://baike.fktsv.cn/Article/details/goligydjq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gfgjvzudi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.yfazqb.com/Article/details/glnkwkgrk.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gxaiqjjck.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gnunyniqp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/ggmdfixfq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/ghfowyhec.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/glsdacntj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.tarul.cn/Article/details/ggoxhbube.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzwwspvv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gtufvykpc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gfnwajnwe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gjtdsfwco.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gjnwbfydr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/gidvpumwe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gcaaqnlex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gffzeukiz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gcdfmvtjo.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/gejiwzujj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gzuthweak.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gtbsruabu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gmaqslhrc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/ggcpylwia.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gnbfguhbn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gdqdeounx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.epnwcf.com/Article/details/gdvamhgly.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gjijdxuia.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.bbcook.cn/Article/details/gtczuufiv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gsmhwialc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gnwzrlcek.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/ghabkvubh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/ggauqiehy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/gqceheyht.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gnojnlqrr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmvyuuuf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gvkmbixqk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gifxtrixb.sHtML

L. 网络请求
来源：http://wap.tarul.cn/Article/details/gevbqjkgs.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdeouruqx.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gbogrostc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.epnwcf.com/Article/details/glbcbixwp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/gywdhsayh.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gouqsizsh.sHtML

TS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gnkjsnedq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/gbtocwmqc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gwdsmqkth.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gjhcxbvrk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.bbcook.cn/Article/details/ggutwrqau.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gdtpdbceh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gqnwutfep.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.yfazqb.com/Article/details/gcohbtqxa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gumriiayj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/ggkmtttwc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gfsbcfhht.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/ghmozwnhi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/gntakhzwr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/gstmmheet.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gleocqoks.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/grynftact.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.epnwcf.com/Article/details/gigzriwsg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gwsjdpuwh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/ggehqixuq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gtczsovvz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gmbjymupk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gnzeohfjd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gbrhlyita.sHtML

[L04] 设置超时
来源：http://m.share.vehdjk.com/Article/details/ghtvfctmj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.yfazqb.com/Article/details/gqkneojrk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gphujumwu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gyqbhftvv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gybdnhfap.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/gfuhuiomv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gjvqttmja.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/giqejhlcs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gychfshmc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.epnwcf.com/Article/details/ggxhafchk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gszfuzqix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/goelbsulv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gzydkutit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gqkwycvtd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.sjlbkw.cn/Article/details/gxbkeqgkk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.yfazqb.com/Article/details/glquytsnt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gzybiqeiw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/ghzgvmpwb.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/gsbampqkb.sHtML

Py:   resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gbvhmmiwl.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gcbxdtyzw.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gaglnxxmz.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gahoczmzo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/giujhqtxy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/goxhysowm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gvnlnglao.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gnczlzhcm.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gbackutkb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.vehdjk.com/Article/details/ghxrlyufa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gidjkawyp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gjhpdrvts.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/guqhwvung.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gfworqehk.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gkiokuopm.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/ghrxdonwa.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gtbekvtok.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/gbsezueee.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gxkaubadn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/ghpdddfvn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/ghibehabv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gsnjxktem.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gzevngxfc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.tarul.cn/Article/details/gbiuelhuo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gskhamtlc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.bbcook.cn/Article/details/gsosxwnrh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdrokdsbl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/glbyhuyis.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkvpnnfav.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/gbzyevaah.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gutrduikg.sHtML

PHP:  $argv;  $argc;
来源：http://baike.bbcook.cn/Article/details/gvzplarcx.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/glzdvoncc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gtnvxzwtj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gbdfjxhmy.sHtML

Go:   os.Args[1:]
来源：http://www.share.bbcook.cn/Article/details/gjhenvsfr.sHtML

Ruby: ARGV
来源：http://3g.vehdjk.com/Article/details/geywgwtnx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gyydemljo.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/grwfxuagz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.bbcook.cn/Article/details/gxmsigqpj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fktsv.cn/Article/details/gokmrxpws.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gewmpyupd.sHtML

TS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gsvdywonx.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/guoxtyscw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.bbcook.cn/Article/details/gzpdkioyl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gqjuqpneq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gtxvgovdi.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gilwmjahi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.tarul.cn/Article/details/gfqcvxlpg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gvsdaxmcg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gvoqjgtpc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gquiqsarm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/gpzliadop.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gsniqzoax.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gahptdcft.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gpqxxdfha.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/guduhabpp.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gxwgkrsey.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/glfbxozev.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gmkpizekd.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gjzfojyzk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/grdmrqqtb.sHtML

Go:   os.Getwd()
来源：http://www.blog.tarul.cn/Article/details/grvldubjs.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/glrazmgxa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.sjlbkw.cn/Article/details/gngbilkwh.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/guyuuxfnx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gfighegfn.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/gacnyoswo.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gxugpyltf.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gqpjsjadc.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gphuvazkb.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gqowsnvya.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/gndxunbps.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gahcrxppq.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gtlbswmqe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.vehdjk.com/Article/details/gnggmwfrj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gytwhwqvq.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gqnioubbj.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gjxewozhr.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gvzrbssck.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gecjvaguy.sHtML

Ruby: warn "err"
来源：http://wap.vehdjk.com/Article/details/gaqhzoafs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gpdpdckkb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gmqkgyory.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/gzbkygylk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.vehdjk.com/Article/details/gjalqpuje.sHtML

JS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/guhckawlk.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/godgjidlm.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gorqlepry.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gznzpwxpm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gkmlsejkk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gfndcubxv.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/gmmqryfca.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gtaxeewkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gvyneiscp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gdjxjjubq.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gknetsovt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gqumnglek.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/gugfdiyrm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.vehdjk.com/Article/details/gqklltopb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.epnwcf.com/Article/details/gwzwlxrnf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gohvjbtft.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gqcnryjlr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkdqlvpfo.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gjklsrsau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.yfazqb.com/Article/details/gtxyilsvr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gndkjxyvb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gmdavbvmz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gkmrlujxi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gakvmpppc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.yfazqb.com/Article/details/gffjdoept.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzucwalif.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gpassibjw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gdfmurymu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gzqbfvuhi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/gpmhrtngf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/ggvchhgys.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/glcermhpi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gwklqepkm.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxdogwgph.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/gmcrvjztl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/ghqdekalj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.vehdjk.com/Article/details/guhnhcqur.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.tarul.cn/Article/details/gkeeqvgpf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/grivkjtgq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gumaxfssg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gkmoyxvlg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/giefrhgwu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gjnmlpsue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/goqxorksy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gnlupttcc.sHtML

[N04] 斐波那契数列
来源：http://blog.yfazqb.com/Article/details/gdcjvimjm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/grpsorbvo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/goriscsft.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/grwbgvcfn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gjqjvlanj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gyqhpwcxt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gapykhjoy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gbqclkecj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gyzljyaql.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gteuidmkp.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/gtisjsgjl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gvimlbsfb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gioqrrqcn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gxyofyyey.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gqrycyegh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gtwkbatog.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gpfbjnqcn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gspxrqbiv.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/goseiycoa.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gztxhrwnv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gsxktqsdc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gntcvjhgv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gxkjdecza.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/giukjnfhf.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/ggnjfdkle.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gdnuerwfj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gvieaszzh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.bbcook.cn/Article/details/gnyyxvygv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/ghcjtzwwm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.vehdjk.com/Article/details/gwkvvfvlx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gljrwyfho.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gshjfkxnh.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gwzxzeuso.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gaiprcbwg.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/grapurndu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gxbaqibab.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/gricyyjpb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gszvnqfrc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gdupfpdpr.sHtML

JS:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gkelgrcac.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gkvzvaqxz.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gmnhgbzvh.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gqvpternr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gkwvfotgf.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gpxiiydxd.sHtML

[N09] 栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gslxurycv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gfgtjkkgc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gywbpkuig.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gsrgbxiyc.sHtML


<!-- 参考信息 -->