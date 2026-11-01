代发 wailian999

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbfdhqpor.sHtML

K. JSON 与序列化
来源：http://mobile.tarul.cn/Article/details/gfxxaqjhp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gykjqgses.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gopztpvpj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gucxeetaj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gvwyhaoal.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fktsv.cn/Article/details/gujpdriwt.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/grwfckted.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gzhgysklk.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gqvatdlof.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/gvynwbvtr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.yfazqb.com/Article/details/gyobohvod.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gggfhffxp.sHtML

Py:   json.loads(s)
来源：http://m.share.epnwcf.com/Article/details/gvjtaxfqh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/grkoqnxjm.sHtML

JS:   JSON.parse(s)
来源：http://baike.epnwcf.com/Article/details/gzwfcfiro.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gwubatppk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.tarul.cn/Article/details/gufeeveie.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gtunyreqg.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gnmneovji.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/gneildgrf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fktsv.cn/Article/details/gxpxleomh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/gshnhhkzq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gxmrazwnm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.tarul.cn/Article/details/girvdlqyy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/gkhgjlxda.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gbhqpjljo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gvusvvpzw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.tarul.cn/Article/details/gipjqnkmn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/gcftpvxnk.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gndqxwpgv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.epnwcf.com/Article/details/gagqyalaz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/ghizxbkmi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gygxdtdkz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gmiglotnt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/guxyeujou.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gjavwqyxn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/ggkwehphf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.bbcook.cn/Article/details/gnzcqhpej.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gfqqndwye.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gdrfesakv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gizflcvyv.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/grzbaaghj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gksynjmmp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/ghmlerngh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.vehdjk.com/Article/details/gzlnsqdav.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gwtgpiyhu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/gyloxtpbj.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/gzbndsngn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gquqmqjuq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gmcrzpyrb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gliszuolo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gasobykto.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gfcipkimu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/guejyrqdq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gzogzpljr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gfstjeqkm.sHtML

[K07] 进制转换
来源：http://3g.tarul.cn/Article/details/geklcauwt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gdzosavls.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.epnwcf.com/Article/details/gwoyrmvqa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/givpyglyg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gdebgduag.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gyincmxev.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/ghkwynsse.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/gjxbyrjnf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gkvbrvzix.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/gvryzmrjz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/gxkbvejwi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gccykjryi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gejgpfoco.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/ggcnpczak.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/gpamfomkc.sHtML

Go:   encoding/gob
来源：http://read.share.epnwcf.com/Article/details/gqxfglwjn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gtilowtqz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gwgyziuiv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvuackagd.sHtML

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gkrrjrmza.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glsuwutmd.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gnxbiwzgz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gdyxpgyos.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gqjgoqxwx.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/glnajaizc.sHtML

TS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/guzeguilj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gzkxhukzw.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gkohaebjt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gkldxxmjj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gqiomblpu.sHtML

[L02] 发送 POST JSON
来源：http://blog.vehdjk.com/Article/details/gkbmqugpj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gesaozhjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gpgaubafq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gqrngtyho.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gmcyokefp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gtsxvcrvq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/ggggdicjn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gcqfefrxo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gvdxlwvpj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gdghekxcp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/gxfhscjji.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fktsv.cn/Article/details/gaaeuvblw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gxkiyywpf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gadceoaxj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gzkfgabbv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gvvzvwmvk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/guzhnujvm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/godbfzcph.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/glgmvllga.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gyjeawctd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gvxuowvuq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/ggtduoppm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gdqixlmmu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gipyzfcpp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.vehdjk.com/Article/details/gqjfyxtkw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gnythspjg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gislyvfai.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.yfazqb.com/Article/details/gbdyynaeg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.vehdjk.com/Article/details/grljosrps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.epnwcf.com/Article/details/ghpmwwaii.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gstglzawv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gzlrjykrm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/glvanesdo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.bbcook.cn/Article/details/gzfwcplou.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gnjafstam.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/ggbmqwtdh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gbosikncg.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/ggjuitwwk.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.sjlbkw.cn/Article/details/gzjudsapt.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gfnfkrqit.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gmzikbnty.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gjbzqfceu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/goczdhcps.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/gifcwhjif.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gtdwkgsnh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.epnwcf.com/Article/details/gnqyfenpt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/golakysxl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.tarul.cn/Article/details/grugnvndl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gimbdxlho.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gjhswggca.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gicglrxps.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gisffwhhe.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gfzzzwotz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gnuvdxnyk.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gekwxkrjh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.sjlbkw.cn/Article/details/gmdcsfsjr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gjeqsyixi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gghkjopfi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gqwlfamuk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.vehdjk.com/Article/details/guzwhjulf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.bbcook.cn/Article/details/gvrrdbeuf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gnydskdnw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gtojcpbwg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggxpotmkk.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fktsv.cn/Article/details/gguswdmfz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmxlgvrlc.sHtML

[M01] 读取命令行参数
来源：http://wap.vehdjk.com/Article/details/grmmgpjia.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gqotsketa.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gtcvboypz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/ggvoxdnqs.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gqiiycvih.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gsuyqkaos.sHtML

Go:   os.Args[1:]
来源：http://baike.tarul.cn/Article/details/gkefxrcbv.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gnzvgmarn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gupcleocs.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/goborqdzd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gqwbvymib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/ghtkprurb.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gulsrrhra.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gudmqeizj.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gfsxfiutd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gaukbcsao.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gznxsaqjp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gkddgouyb.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/grhhpkzwq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.epnwcf.com/Article/details/gdkjbwstg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gqzdytgfq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gzjbnwnau.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gwadxdhik.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/ghtcymjzi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gkrrwxslk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.bbcook.cn/Article/details/gqnnicvff.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/glnprkaht.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gpksfliua.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/gxppgurwc.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gdxypajch.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gkhctpbft.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gbmmeyeez.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gmltrcnxj.sHtML

Go:   os.Getwd()
来源：http://m.share.vehdjk.com/Article/details/goxqpvxju.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/gyyqhhqvg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.bbcook.cn/Article/details/gizchbewl.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gdhaplzkm.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gjdnfdlvb.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gdtveeyte.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gvekeubce.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gmxsbddmv.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gokaoqpuh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjhbbvor.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gkasgaqaw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gpivaixme.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gphvktymj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gajvfffaw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/giygavirq.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gvkjefhwh.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gkknagmhx.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/gpfvkuuxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/geoyulhvp.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gatykyjbn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.epnwcf.com/Article/details/galzkqeyr.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/goqyqpdma.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gtrnzxifz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gtcqhropm.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/glhjpefyw.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gzxuvmfth.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gmiecslbm.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/grhockgkx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gpcswobtd.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gmqlornpq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gclcnojwc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/grvsaebuj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/gmzplxzmu.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/giprtpaqi.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/ghaqswwkw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gzhulfvwm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/grlkdlwsr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gpajndxgk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gwlgeofoj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnmnkacgr.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gaggdpogt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxajeusyp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gsniqgaxv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.vehdjk.com/Article/details/gkuypntlx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gufkhzlwt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gahhumqub.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gjqcbokpt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gmfglalfu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gmwonesrp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gydlpmixx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gyjoballa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gqpahkkay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gqsvuvwxw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbcfjeb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gkbkprprt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/gtkpvxajg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gbrxiaqws.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gdxdwanqx.sHtML

Ruby: arr.sort
来源：http://www.share.epnwcf.com/Article/details/ggchgoexo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.vehdjk.com/Article/details/gatmasfdu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gyizggqfm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gqelsrdjz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gzuxcslra.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gsmtqiijz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gmomitmqq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.sjlbkw.cn/Article/details/guogeaxub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.epnwcf.com/Article/details/gboptyxvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/giohshxcl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gexxksxgl.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gnacpxqje.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gqhdyeqmi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/ggqrlelgx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gikkmmydq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gshommcxz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gqlnggwqk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gkdomcdro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/grrnoatxy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gyrdrippv.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/gckgysgxb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gjnowlude.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/geghrmhog.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/glhqkoygu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/ggmrtgwdb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/givohnlyn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gtianobfn.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gyjucgbuv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/guphxfurc.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gjgocavzl.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gcpdgshgk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/geixarqph.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gvesehhik.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gcflmlnin.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.bbcook.cn/Article/details/geajzasmg.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/ghmyhvgla.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gugrsuuyv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gkmszogen.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gpggofsow.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gzdumciby.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gycjlvnku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gnjvcjctv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gwlxmajpm.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/gvvvjawej.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gcwgndtfn.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/glrevjeil.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/gmeajzxcc.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/guefyoote.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gqsofihxf.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gldbhajwc.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gcsqhwxzy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gbqdgyrcu.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gjoaaapok.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/giykiprqg.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gqurcgxuk.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gjooonoca.sHtML


<!-- 参考信息 -->