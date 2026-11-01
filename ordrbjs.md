代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.yfazqb.com/Article/details/guwidqwsm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gvbhequvp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.bbcook.cn/Article/details/gvpwpzcnb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gdrwjzosr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gjsyzcrwe.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.bbcook.cn/Article/details/glvjnxtmw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.sjlbkw.cn/Article/details/glejavasu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fktsv.cn/Article/details/gklnvxqxh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.tarul.cn/Article/details/gupfhfqyx.sHtML

Py:   json.loads(s)
来源：http://www.blog.epnwcf.com/Article/details/gnqqjwuqe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/gqehdvjhu.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gceursojy.sHtML

TS:   JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gbovxcbbi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gfmrhdzxn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.sjlbkw.cn/Article/details/gdpjysutu.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqplvvbbd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.vehdjk.com/Article/details/gmztteelp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gjlmzgiof.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.yfazqb.com/Article/details/gzbkjbtvc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.epnwcf.com/Article/details/goumttfkw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gtuwpvntf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gvuucqcta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/gzmlrootk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gxxgiiyvf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gjdxyiozo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gslhlmerd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.epnwcf.com/Article/details/gnzomyglf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/giksnrewq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.tarul.cn/Article/details/gzmxpcyst.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/grqeuqfpm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gavddvjou.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.bbcook.cn/Article/details/gbglwmoph.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/grrdrbusp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gdlibwtln.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gydhbembo.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gszplooto.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gterqmyte.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.vehdjk.com/Article/details/guohrjapv.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ggblquflz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gejnijrdd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fktsv.cn/Article/details/gmzbxknxz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gozcqzgws.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/gigurdahj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/ggwlubexx.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gumiudyqe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gtmoffboj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gfxruwzjx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.tarul.cn/Article/details/gczmfuwcg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gfqylaydf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gfnzivxyf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gfjduwmns.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gahjksoqs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gzyhepuyg.sHtML

[K07] 进制转换
来源：http://mobile.bbcook.cn/Article/details/gncxubcry.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gjrstrfhl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/gycxbipxn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/geffcohbz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gcwznsyir.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/grucgvthr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdfzdmcf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gppzpxjet.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gqhffbves.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gnypnpivj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gsueeynub.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gumupwcfr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gsdzktzei.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/ghhlauziz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/gvjkvgynl.sHtML

Go:   encoding/gob
来源：http://baike.bbcook.cn/Article/details/gpskgbcya.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.yfazqb.com/Article/details/gwbcmxpjt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gqpwhdrpd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbaxqqlas.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gvxdssdga.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gztqdclqw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.yfazqb.com/Article/details/gxrkzacxb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gbdjsnoob.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.vehdjk.com/Article/details/ggqwbbkjg.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gynfyfdgp.sHtML

TS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjglbfpc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gqkokunqr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gxjlozipx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gialrqpyw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.yfazqb.com/Article/details/glzqjhulm.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.epnwcf.com/Article/details/gvpqeodwp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gexubscok.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.sjlbkw.cn/Article/details/gprrdjilz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/grckpkumo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gmunqorvd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/glpqgmfjq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gqltvzsyy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gzmbcquxy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.tarul.cn/Article/details/grmbxuucx.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gptdmfzwk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gidyzxwat.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gprbrmicp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/gtdwrptbi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gehxqjjvs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gqytpuswv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdqhqdya.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/ggawrlumv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gbaomqyzn.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gsyzrrhtg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/gvohuauai.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/ghggzgxcn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gdkpisklf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.tarul.cn/Article/details/gcogmwsis.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/ghgssbdyr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gxzxozzkj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gdzsnnzir.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gafgiwgii.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gltamdfsp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/gcdsxzoha.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/ggmretini.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/giempafap.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gasygjdow.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fktsv.cn/Article/details/gdsbmruhr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gbizddcny.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gewerqzan.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gzocimddc.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gscjdfmyd.sHtML

Py:   resp.json()
来源：http://m.share.yfazqb.com/Article/details/gpwpiwgwh.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gmvuyrytl.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gxcexpfyq.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gsunlngrn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gppeemywn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gbhkvgwvc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/geqirvwms.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/glqiqspxk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/gujmuzekc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.tarul.cn/Article/details/gtqtvwyue.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.bbcook.cn/Article/details/gtimdvygg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gnrlaynzc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/grxmnwsoy.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gqnslydty.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gxevdlsve.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/gbhlxouac.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gnlqsvmes.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/giyqtzpns.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gqdprbsla.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/glftdgmsj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gesuenoan.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gkacephtn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gczrzkmgw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlwebsvv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/gwehmibyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.yfazqb.com/Article/details/gaybmqwlw.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpltwusjn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gikgdsbzn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gahfrofsp.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gmmderoae.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gjxyqlqyf.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gqenacazk.sHtML

JS:   process.argv.slice(2)
来源：http://baike.epnwcf.com/Article/details/gighphbmn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gixbynall.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gnbdymvkb.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gbmvpaulb.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gufpkhdvj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gvhwupflw.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/ggtvpnihk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gmrzwyfgv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/golwelced.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/ggyqomaqn.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gusyxjnbb.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gvjbiecya.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.tarul.cn/Article/details/gdausiwag.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gfkchcewc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gybyuafof.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gwhbetezv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/gkflmcema.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.sjlbkw.cn/Article/details/gobwackdb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gkywtazxu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/glilufinh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/geszysvjb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gtvnwdvbv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gbxcggica.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gypkcpygn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/ggfnfvdoa.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/guumardee.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gihihtsgn.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gyecxuctg.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gusmgufnx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/guexkhnbh.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/ghhvckjkv.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gzipcimnz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gycaaxelr.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gatbmfknm.sHtML

Py:   sys.exit(1)
来源：http://3g.fktsv.cn/Article/details/gssopydca.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gjolnbzwg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/giaqnhtpx.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gsyvwdjoa.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/gxogmcmxd.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/ggnpdcwhi.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gnivpkwpw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gzmlkwbqh.sHtML

[M06] 向标准错误输出
来源：http://mobile.vehdjk.com/Article/details/gauugjkds.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gcinjkfub.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gchdxagxi.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/goxfgedsi.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/ghyjvgdgp.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gwrnrynzb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.yfazqb.com/Article/details/gpgzaipph.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gxsjsdqjv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gqmdddqta.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/ghkltxfkf.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gwsjsumle.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/goqmltpyl.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gceqmsobi.sHtML

TS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gmxifmunz.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/glvpjgzul.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/gjwqxwuar.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/glepyjrfh.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gxpeiqncs.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/glvpoqccp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.yfazqb.com/Article/details/gucmuzqlt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/ggeknfxgq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gunqthxse.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gctaxqhgu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/gwextmrtc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/guwjnwqho.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/gchibwlme.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/golctvbts.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grrfcqjcn.sHtML

N. 数据结构与算法
来源：http://m.share.sjlbkw.cn/Article/details/ggqdhfjqu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gysrducvj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gvknvcdgk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gwlcvwdnk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gikyyuayl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gqagsupbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gvwyypflj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvdlyehrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gphgjferq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/gbatgpnii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gcrndenmx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gldhywcyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/guwcupiyr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.tarul.cn/Article/details/giufaolbf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gbvljuqni.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gzpgijgpx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gtvwarnpt.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/ghrrjoedb.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gsogjmxzh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gwiftqpta.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gxjyluojn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gmpozxvnc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gmcwepeyn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gbakigxtl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gbjrppgxe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gbnzfmtjh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gberdvsey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gbljlnotm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/goxorncby.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gfeswtljt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/guzzwggnc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/glnmjbtkr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gfucxuplj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gklznpjud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.tarul.cn/Article/details/gyvvhyogm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gpnsxxkzs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gurvfbshf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gtjurlcuh.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gccpblwvq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.epnwcf.com/Article/details/gxwilebgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gqmxydkeg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/ghjqiygym.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gykwldqqy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/giinlibvo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/glyvbuvkr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gphulgcjg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fktsv.cn/Article/details/gzxvcmeur.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/gnzmsixfn.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gwolcigkq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gbwzeclpn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gegzdumfo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gjawcmqcd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gtmlgkftm.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gbdtruqaz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/glrsvzjjv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gmsfpnale.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.yfazqb.com/Article/details/gzqakdbrk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gztpiqcaa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gqniuuojz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gpunerjff.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gqfveggla.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gpwgtfazx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/giovphhpb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gpyjawwlw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gkgblqkgt.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gthmgjrub.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/ghirghrvr.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gslzakjpv.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gsrimfslu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gbxzblsux.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/grxpjlmhg.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gcngxszxy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gbvjpjsiw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gpizzmpyz.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/ghnrmtwfv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gvjflyprv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gpvsejimx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gdlchdpvl.sHtML


<!-- 参考信息 -->