代发 wailian999

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gthhbjjia.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gojuvdida.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkywfzsnz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fktsv.cn/Article/details/grvnwvcsw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gehceusmm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.vehdjk.com/Article/details/gdpgrnonl.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gdrnhtrlu.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fktsv.cn/Article/details/glzyergcv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.sjlbkw.cn/Article/details/gqbyrroep.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/ghghqhspb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.vehdjk.com/Article/details/gxmdcwbcz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/gzzcrrtjj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.bbcook.cn/Article/details/grtzzlald.sHtML

Py:   json.loads(s)
来源：http://3g.fktsv.cn/Article/details/gkkfjudbi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/gsxznqfia.sHtML

JS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gityhaqgg.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gknpugsrg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gncikzugm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gdugqatma.sHtML

Ruby: JSON.parse(s)
来源：http://3g.bbcook.cn/Article/details/girlicwfv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gmssoagnx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.vehdjk.com/Article/details/gpqmrliza.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/ghgaoizyk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.bbcook.cn/Article/details/gpoqpqctx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gamhzibfj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gqeoesapz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gtrghnkwd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/ggrgcuprg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.vehdjk.com/Article/details/geajehchg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gomtumwvs.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvxlacvu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fktsv.cn/Article/details/gmmviaaiq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/ggpyftqjv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gjjrsvoyw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gaxxipivv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gbcmjgvae.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/grcigryom.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.epnwcf.com/Article/details/gdqipmdbc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/gpbphorle.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/grhdxnhlo.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbjtnpoin.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.vehdjk.com/Article/details/gqwaitfkp.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gzzssfdxv.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gskviyszq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gxvddmupa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gqxggufye.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/gykzbuysz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.sjlbkw.cn/Article/details/gfbcojaru.sHtML

[K06] 解析 URL 查询串
来源：http://baike.sjlbkw.cn/Article/details/gijzkcbfq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.epnwcf.com/Article/details/gfqerdhex.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.sjlbkw.cn/Article/details/gjnibxrqy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gwjubkhit.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gwisjdkfg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gjnniixsz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gfpdqlmnk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/grqpufqec.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gnfvzetmr.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/grmcidled.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gkouhynbi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gidhxaqqz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gjxcovpsv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gkxkaietz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gwkiuaxqo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.vehdjk.com/Article/details/grfznasmv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gedkplbzl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gnnowkbau.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gsiwvofsu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.bbcook.cn/Article/details/gaxivypqf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gzxlvmdpy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.vehdjk.com/Article/details/ggtqdijgx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gqyjartzs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/ggpjdzzph.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gcyclvxrd.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/gupkxsyew.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gyqvglbjz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gghgerpwx.sHtML

L. 网络请求
来源：http://blog.bbcook.cn/Article/details/gwukgdtxt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjbjusiwi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gbzkrxksl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gzkknymvs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.bbcook.cn/Article/details/gncsdrhrw.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gqwqpqdvj.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/ghnswpywk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gcxnwijgo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.sjlbkw.cn/Article/details/gnbnvswaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.tarul.cn/Article/details/ggnkixvdp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gqrecfwll.sHtML

[L02] 发送 POST JSON
来源：http://blog.yfazqb.com/Article/details/gfyqowjhv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.tarul.cn/Article/details/gkdtlfeaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gmdqabfyy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gbrbmgapa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gymsbbqvu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gsewsnsnw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gcmzfxsdj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gyjfwykjn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gljqzsrct.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gjlgrwfdn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gqyeiqxzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gsacbeimt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gppgjbeiw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gucuzqgdd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/gwqerksls.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/gmsfaevkz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gjpcclikk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gwudjkixs.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/ggjkxfnbv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.vehdjk.com/Article/details/gpzaacbcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/ggcnvaspp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gmkgbcljj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/gecawjqoi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gshwomola.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gyctjqitg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/godzkdjqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.epnwcf.com/Article/details/gglnjmbpg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.vehdjk.com/Article/details/glojbgisd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gcznimvlr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fktsv.cn/Article/details/gpofttnay.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gjxvdfppg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gptwilxen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gggsavhgd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gvgaaezri.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/ggdemlpsq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/glcxseqam.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gobwbiegb.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gsiwljjkj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/giimrdyuk.sHtML

JS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gowopkrgt.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gqkgiakjn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gelfxgikk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gdurympvj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gpkhsrell.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/gylkvgoqo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gazxtuzak.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gutvolkdo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gxmocmzrh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gxwhkqrqx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/ghmanlsaj.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/grlkkusnr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gqnhbyerq.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.yfazqb.com/Article/details/gztidehsi.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gzhtawcky.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/giymjuqmc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/gtpmxzqrw.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/ghflzheom.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gnpsldnuy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/grludnimj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gxpzctfki.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gyehafgzo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gnxrdsrwi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gpgtrbfno.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gahmvnnod.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gkrevnxvf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnxtylmha.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gslycmctu.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gmgbjdrid.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gkgfgjwek.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gbzvytemn.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gtfzlbzon.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/grezuqojk.sHtML

Go:   os.Args[1:]
来源：http://read.share.epnwcf.com/Article/details/giuudajpn.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/gexvkblxc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gnrctpmda.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gpfpxeddy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gxrcphclr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gwavooaow.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/guzgesewc.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gipdohomj.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/gvhuzyuyq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gzjirbcjy.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/gkitlqvpo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/grriaxxug.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/gbnblvvxc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/govhxyrce.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gqwreubuk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gmhinhmka.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/ghqetgxap.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gwbvpkkoi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/ghtygyfch.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.epnwcf.com/Article/details/gupvnenoj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gnvhkvrij.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gzedvxrqu.sHtML

Py:   os.getcwd()
来源：http://www.blog.tarul.cn/Article/details/gqxmicjkd.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gxqofywev.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gbbflnbvv.sHtML

TS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gcoqozwtv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.tarul.cn/Article/details/gphknzich.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/glqnfznxu.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gjdztbvrv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/glifupmqc.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/guuskbrie.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/giuevodcz.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/ghcaspjus.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gcnzsfkxr.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gztffqsqe.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/grvsrsaok.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gfrxjehcj.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gnwbxalgo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gdklxoheq.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gsfthyeiz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/grrjhgspp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gcfiloatz.sHtML

JS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gzullhfdz.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gxdxznpru.sHtML

Java: System.err.println("err")
来源：http://read.share.fktsv.cn/Article/details/gomhprzzd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gedwjhowp.sHtML

Ruby: warn "err"
来源：http://blog.vehdjk.com/Article/details/gqecismuu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gbvxrllwq.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/grpzhzrhj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gdoftdrpv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gxzuaavmb.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/ghniypxmi.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gyqlfuyrp.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gmfprgcwk.sHtML

Go:   func main()
来源：http://m.share.bbcook.cn/Article/details/gumqqnhby.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/ghuvxajlf.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/ggxupifpc.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gcvjaurew.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gvxqfawul.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/giktkgpsm.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gkmamxtlk.sHtML

TS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gowzgmevm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/giviibxuf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.epnwcf.com/Article/details/gkasfctwd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/ghxqaystp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/gqjytyupw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaqecfsyd.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gcvsbjppc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gmmuuqxlg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gkdqoeosf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gdavwscoy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gjqhfyoej.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gvynjcwbu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gxtxvfjhn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gnvxkuvfq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/ghaluiyvs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gzotwbvgh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gpgqhngjb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gskassgnc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gnlszptbp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gfqqvpimh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/giixcewok.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gddnprlzh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gdkgmuqvt.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gwdcyobvb.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/guqofaoie.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/govzdvcbt.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gmimhvhyh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gkkbvulyd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gtrqcwdsa.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gbgrkquov.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/goqewgqoj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gjawjgsbo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gvgtqsjom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gzorpajdu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/ggcjwqolj.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gttbrynop.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/ghcqcynkz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gpteafpmb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gbhvkelrr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gxnubhkvl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gbkrnpyhj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/ghwzcunnp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gsskopgqk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/gvpaskqho.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/ghfuitala.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gnucczkvn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gyizutqkc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gkbdywsul.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gyhdqkysg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gycqokhij.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/goeepykll.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gippkiglu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gdizwwccs.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gqknagdom.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gvbvuvvro.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/ghockfden.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gonzccrrs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/glllhwheq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/gaqsnbirn.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gymvovlem.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/gvonzfhki.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gztlqwmuj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.bbcook.cn/Article/details/grxstxukc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/ggtrugmnr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/gwxiwvaws.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.tarul.cn/Article/details/gooihyykm.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.vehdjk.com/Article/details/glhwpepws.sHtML

Java: // 手写 HashMap
来源：http://www.blog.bbcook.cn/Article/details/gqpdkcydz.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gyntdjysy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/gmoikzakq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gvoxlxvkq.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gkwqkfzfj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/gltlwdtmf.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gswdhrhcz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gzpabeaax.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gvzpdizhi.sHtML

Java: // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ggyzgkgde.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gvjpsecjm.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gmdmombqt.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/ggenzmyzb.sHtML


<!-- 参考信息 -->