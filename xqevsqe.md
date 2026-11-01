代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gkoffvfod.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gygrqlrix.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fktsv.cn/Article/details/gsxpckymi.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.yfazqb.com/Article/details/grmvjbaza.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.vehdjk.com/Article/details/gfuawvtse.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gbmhppccn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.yfazqb.com/Article/details/ghfytkkgk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.bbcook.cn/Article/details/gubssvfau.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.sjlbkw.cn/Article/details/gveclalss.sHtML

Py:   json.loads(s)
来源：http://baike.bbcook.cn/Article/details/gvecocayv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.tarul.cn/Article/details/goxgphcku.sHtML

JS:   JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/ggumaqtqd.sHtML

TS:   JSON.parse(s)
来源：http://m.share.vehdjk.com/Article/details/gidtqrbji.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gnvckyiaf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gcirpbkia.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grodlkukc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtbypfmmg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.epnwcf.com/Article/details/gwgasvgmv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gfcvdwccu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gitswzhvb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gkhtteuad.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/gguivczlm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.tarul.cn/Article/details/gwqmiecst.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.epnwcf.com/Article/details/gwyeluapf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gqascqtpy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.tarul.cn/Article/details/gbtbpmizi.sHtML

[K04] 读取 JSON 文件
来源：http://baike.bbcook.cn/Article/details/gvujysiky.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/ggxvarluk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/gvgltwmbl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fktsv.cn/Article/details/ggwminkss.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gbwdaneng.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gflofccbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.tarul.cn/Article/details/gfjvljxws.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fktsv.cn/Article/details/gcdpniotn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gogbfgirp.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gkikhenbu.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.bbcook.cn/Article/details/gkdwstxhk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gskghwmsm.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gktmipnqf.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gkdvauicb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gjoccfzpy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gkreiwimo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gearbrgsd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gqycvnqir.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gdgxgpexj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gsctjzxvx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gehzkszqg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gbxxyubzs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gaglonhaf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/gdutsruur.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gpaxerigk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/grulfhbcj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gufsekzkt.sHtML

[K07] 进制转换
来源：http://wap.sjlbkw.cn/Article/details/gvgphcloz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gveaeuglu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gltortqmp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gejxawtux.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/guchhognv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gsccviwir.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gmclwnruu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gupccfvxf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/ggdgmgrkj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fktsv.cn/Article/details/glxxmfxtd.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.tarul.cn/Article/details/gybgcywqw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gutacplfr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/guaoqqmje.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gxfvdhtug.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/ggozjfxrs.sHtML

Go:   encoding/gob
来源：http://3g.bbcook.cn/Article/details/gjmcfbguj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gsymbtyzj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gpaxtajct.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtuvousyl.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gdwwklkpn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gasksebvs.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gtacydhvx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.sjlbkw.cn/Article/details/gqurppghc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/gmdjetoto.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gbttyjggs.sHtML

TS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gkxnqgqby.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gwaofpqmy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/grxhdbtqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gurwxoyla.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/giorlifdc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/goforvzws.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.epnwcf.com/Article/details/gbflnahjb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.vehdjk.com/Article/details/gytibpfyw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gohcveico.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gbndbrljy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gsdzvagrx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gevwkftxz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gteuxppxh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gavzzuyln.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/gcwtxoghj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gxwetwfuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.sjlbkw.cn/Article/details/gbyhvhxlo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gosyaypby.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gzqxlgvmf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/ghhmqpcdz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gfbhyfenm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/ghvvxrfoa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.sjlbkw.cn/Article/details/gndqxgzdg.sHtML

[L04] 设置超时
来源：http://3g.bbcook.cn/Article/details/gulcvkofs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gjyyrpihm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gldydvhvq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/guhfuvhee.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/ghjjyyhkg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gamxjarok.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/ghchtgens.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fktsv.cn/Article/details/gkwonijwr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gxkxzfutv.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gauiddpsk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gxjaakbwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gipukpyow.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gcxioafms.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gjclfdquj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gusfgempu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gbomzygdh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.sjlbkw.cn/Article/details/gzgabpkqx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gfhsgabyb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gtktatriq.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/ghdxdrdds.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gqkgndvkn.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gnyyqwtko.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gfyigxlvm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gnhyhsbmr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gemzuxphp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqibqtjdd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gtzhztcwx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gtcqxuszp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/goozooekl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/giwnyapoq.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/ghqzmoxpa.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gdhvrhzjt.sHtML

Java: resp.statusCode()
来源：http://www.m.share.tarul.cn/Article/details/gtlgevbpy.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gammnkgiz.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gtcnrdlmc.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gayskzbzy.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gyumcordd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gfkdutqsd.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gmahyogqr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gbwsuvigm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gbcmbltln.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gallprjgs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gxujgogaq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.yfazqb.com/Article/details/gikfrwcjk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gcmmozavx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gohhrgqtt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.yfazqb.com/Article/details/glwhrxhaf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnsshcrvq.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/glybnalxt.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gprgosqdk.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gfdhcqnkj.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/grsnzcxjg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gpmdpynex.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gofdkzgba.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gpwntbzhm.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/ghlabnwec.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gjafgnand.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gkfiswjuu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.yfazqb.com/Article/details/ggsfkptof.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/glvbbizpk.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gawsyxqba.sHtML

TS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gkicpagyo.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gygrbedpj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gmnwxihto.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/giupsiito.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gelyuzdbx.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gdcdusjwa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gwnvbogtg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/gzlawrvfs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gnamxaoje.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gafdxaaox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gztldwfca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/glvkfuvei.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gklwkcmnk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.vehdjk.com/Article/details/gkcdzjfsh.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gbzzddzrl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnintdxp.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/giiampmqy.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gwtdykrtf.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gguobwerc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gnjfqdpwc.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gzujjyuwy.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/geajhlveb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gvyxnrocn.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gazkxrfhd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gjjlbgzwj.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/goqgnxkxi.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gfzbvpjtt.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gzcsfqxkd.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gqmoidone.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/ganmxqrmm.sHtML

Ruby: exit 1
来源：http://www.m.share.tarul.cn/Article/details/gcutykkbg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gapkvrnht.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcnfupdm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/gbgcixnhm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/geiqyuhze.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gqcgvdpgy.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gsaugrfgw.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwnysryp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gsdkbblwq.sHtML

Ruby: warn "err"
来源：http://read.share.fktsv.cn/Article/details/gkgwlnhqj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gjwwrqodm.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fktsv.cn/Article/details/gpydhnjhd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gxrehsrbm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/glkiedrym.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gtbjaofrm.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gnrlqsadm.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gzrjfmujx.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gqymldvvr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/grripgucr.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fktsv.cn/Article/details/gkixzjgjw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/ghcxitlnn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gfvebntnb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gyhftttgc.sHtML

JS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gnpfvejcz.sHtML

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/glottsmhh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gsxhcjptl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/ghidwcnxf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/gcjazynvs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/gglpfekyq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gqbqyfypi.sHtML

N. 数据结构与算法
来源：http://blog.epnwcf.com/Article/details/gakpzqtne.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gfwofbxdb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gxezeloiq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/glzsjuxpi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gzxpimimu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gzcnitcti.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gwyclqjmu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gfzvhzwnb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/gsrjklzlz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gtuwaenxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gizlayuuj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gkevzvrjz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gqfzylgao.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gtlnaacwy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gymowfbgy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/ghnplucjx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gglrnntyf.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gzyqnrkzr.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/guaiddyzz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gdepevyhh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gallmdaft.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/gmwhokkod.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/gfmoqvgwc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gdglccikl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/godlukymi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gtyiqvwwo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/goxxjgchx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gubbfnnok.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gxwnqaomu.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gilvhfebd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gkgrkjyga.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gqplpxbxg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gpojwlxne.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gnyhvplcb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/ghxtuvthi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.sjlbkw.cn/Article/details/gptupacqd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gffvdlhgk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gcgskxssi.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gpbkbkaty.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/gkirexypi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.vehdjk.com/Article/details/gqxghshpf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gjidmxljt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gpwwfqewn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/giigscldr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/guzphxkod.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/guvopualb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gtbicteuu.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gseqawbwy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gyshsuggy.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gslcakign.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/giwvglfej.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/geagghyzu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gnnyvtcsy.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gtqpizjvz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gmmutaecf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gonqqhhum.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gerywbpkg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gqiwojjqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gyzvpqisi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/ghakqayho.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.vehdjk.com/Article/details/geumpmnda.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gfdiiqzrb.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gioamuusq.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gvwqqwclm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.vehdjk.com/Article/details/gxxpquryt.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gipuqgmta.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gvobjqhpi.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gqpaaeuua.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gcptnigiy.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gubyngmkh.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gaeklyjuw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ggjeqppjw.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gfhtyccjm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gsnxmjvag.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gvwqrhgge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/glimumphc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gtnotgsvp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gblpogild.sHtML


<!-- 参考信息 -->