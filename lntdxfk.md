代发 wailian999

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grzzvebwq.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/goeewtngv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gpeyfwfsw.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.tarul.cn/Article/details/glipvfjim.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gbzxppaur.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/glihbfamv.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.vehdjk.com/Article/details/goqnnjigs.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gvoluahuj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.tarul.cn/Article/details/gasdptahn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.tarul.cn/Article/details/ggyblzktp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.yfazqb.com/Article/details/gqwatlfkm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fktsv.cn/Article/details/gtiwfqnqs.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gaaspsdri.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gztjqclwx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.bbcook.cn/Article/details/gnogqgynb.sHtML

JS:   JSON.parse(s)
来源：http://m.share.epnwcf.com/Article/details/gfucdaxvg.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gzoeniuac.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/ggdznlxpd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gtkmrdjiv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gdtsinrxi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gjfqjgasx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.yfazqb.com/Article/details/glitzvhdf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gvgqlaaro.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gmmuclqrf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gnxxasrxo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.sjlbkw.cn/Article/details/guxovkzoa.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/gojutcgkg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.sjlbkw.cn/Article/details/ggnmnurjg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/gtuxcizcn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gdncowpxy.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gnqjfcpmv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/grjorfeyx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.tarul.cn/Article/details/grwonxkhc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/glbxpkhcq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/giuwfaowl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gjkjqagwk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gxtykapyo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.sjlbkw.cn/Article/details/glrtmtgaf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.yfazqb.com/Article/details/gvizorouw.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/gzywaygzx.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gbrnzgien.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.vehdjk.com/Article/details/gvcmbitsn.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gojmxsewy.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gihmkoshu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gwxzrproo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gmigszdif.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gmfmhticg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gnaghveul.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.sjlbkw.cn/Article/details/gidbifhnh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsrsebff.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gbrydjybh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gumnrnnhj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gwuirbjcr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.epnwcf.com/Article/details/gjyniypar.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/grvkyqjdp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gxtjzzxwg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/grwtjiwde.sHtML

[K07] 进制转换
来源：http://wap.fktsv.cn/Article/details/gtfelloov.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/glkdleuvs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.sjlbkw.cn/Article/details/gszmjskru.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gamylkfnw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ghdcdmzwq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gqrnrkaum.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.yfazqb.com/Article/details/gezmzauvc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/glepenomu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gojtimsbp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gxommhjct.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gxlimlvih.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gybnacoyu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gkgdxfmya.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gldyrhpgv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gowpgduhg.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gbrelpslf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/glcvaneeg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gpavmtugj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glgbgbrbd.sHtML

L. 网络请求
来源：http://mobile.yfazqb.com/Article/details/gnikihngc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/getlkjufp.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gfzprysfx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/gjucjmwyl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/grmvanmxo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gewqzebhb.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gouzptovx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/grxjsfxib.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjxvnhsw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gbolerecz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.vehdjk.com/Article/details/gnzxlrcgb.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/gdjmknfwr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fktsv.cn/Article/details/grkjegnbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fktsv.cn/Article/details/ghsolppnm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/grkczybnw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/geaimuyyf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/grgbvrkqk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.epnwcf.com/Article/details/grjtopram.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.vehdjk.com/Article/details/geoxdwfsn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/glzwfyuuw.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/gmpschyhi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gmarmeylt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/gkifgjbua.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gbsmenekj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/giqixwmdw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/gjmvokhsy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gfxwevckv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/galufajqh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gtciibclk.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gbbotymtn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.tarul.cn/Article/details/goxjbjnpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gowvhfnzr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gserfdfae.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/ggmwbjsur.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gihrusfxc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.tarul.cn/Article/details/grvmjtymz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gapiqsbjy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gubkqawpp.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/ghuvekxtn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fktsv.cn/Article/details/gvlcrgjnb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gcdowhxkk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gpzzkjqfg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gpkuqhcef.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/grapeeebg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/glemzewbu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/goswfplpv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gdajtmxsq.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gvjnasmyb.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gltjoffbx.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gzuydlqji.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gncbwwtgc.sHtML

TS:   await resp.json()
来源：http://wap.vehdjk.com/Article/details/gqnmuxluh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gzlpcupvp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gukcuzkpd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gqrusixpz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gpuxsyqmr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gzjijdagy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gxxxzilkh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gduhascqv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gewhmamqa.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gpjsaaudg.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gafdbvkbz.sHtML

Go:   resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gmwfpjaot.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gjyujpnfn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/goffqnqfu.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gieoiriwy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gvkhvmdiq.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/giykznuyd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gvtshpysd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gijpesppr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/gfrefgsow.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gdprfqbhs.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gowwmzbzm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/gpbvsihsh.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghhvsdvjx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.tarul.cn/Article/details/gobvtujqv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gkughxxul.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gwwiwytxy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gkeeiobqe.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gzmycudcw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gagwqwkax.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/goaubljgl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gbasqormt.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gcwpmwfbm.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gxayixobb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gdxiafvfd.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gzppkltwm.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.bbcook.cn/Article/details/gdgkmxtvt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/gxmszdkhm.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gyzgrgwqn.sHtML

TS:   process.env.HOME
来源：http://www.share.epnwcf.com/Article/details/gbbvvwuje.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gbqlqbeor.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gbqsyauie.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gxlrpdhlr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gfieasojm.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/ggfrlzrpk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/ghqouihxv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/glzovfnqo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/ggjvsvjfr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gfwfzheul.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gupzmiphy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gciifumgr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gmpayhvdh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gdorkynjj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gkemezgoo.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gffdqoqph.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gvallbbxj.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/glsbfnlgw.sHtML

TS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gdibvpqka.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gcuygpejn.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gmkmlzfxb.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gpuzgchpu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/ggbiyqnoi.sHtML

[M05] 设置退出码
来源：http://3g.epnwcf.com/Article/details/gfuqrfhmz.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gxhwsbayd.sHtML

PHP:  exit(1);
来源：http://wap.fktsv.cn/Article/details/gcsewqtlx.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gfbzgjctu.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gcxrbfbni.sHtML

Java: System.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gixgruoum.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/gvpppthut.sHtML

Ruby: exit 1
来源：http://www.blog.bbcook.cn/Article/details/gpjxllhkd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gbacewyqb.sHtML

[M06] 向标准错误输出
来源：http://read.share.epnwcf.com/Article/details/gvrvszpxi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/ghuacnmuo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gyhzqnxhb.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gwzlpbguy.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gbkakkxgd.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gfujdekkq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gamocrkyr.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/grhahyqwk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gucxeseuc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gxgdedjgf.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/garyclnbb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.epnwcf.com/Article/details/gbuaddmws.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gjwxmkelo.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gthjkwaej.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gekrprrsx.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/grrfwlndc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/gcitcxxok.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/glymazdxh.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gatfikvnb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gzfymnjxa.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gicrhuqpe.sHtML

JS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/ggukoujkd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gssmskhry.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gsdqypnoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gkukjvvoc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gqseceybw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fktsv.cn/Article/details/gsildgalw.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gpawebdcr.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gnrskgwcn.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfsitmngs.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gzzyeoaym.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/giltflhcq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gewxrnsqj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gtyegsyuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/ggfxikbii.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/grtfvjphs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gjvmfppdp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/glqszwupl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gnxjxwyep.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/ghfoqpxqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gauoofzpc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gtbkxmtrh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gikclwyok.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gpzhxfbyx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/gwzeusjgc.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gztyooqko.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/ghbqrrecx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gwojetvtn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gxyvxphob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gujpncpaa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/gqjoejltd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gfbnbrtkm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gvuvasebz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gxrpsnkzp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gksxcsxpa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/ghgpiodsa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/gpuseyyvm.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/grouvvxcr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gepwatyyn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gkxfsvkkr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gshfkmirf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gwnsymquw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gtfvcnene.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.tarul.cn/Article/details/giuvmywjf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gwiistcdg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gbitwhkmm.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gzpdyilyw.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gncsjhbuk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gvetetczk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gyqvuceza.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/glzzpxtag.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gfuoqyhwn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gcievpidr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gwbjzstaz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/ggkqbowrg.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/gqwcigyal.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/gudbyjhua.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gxstomzxr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gstgmworv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/grzjngfkm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gpczfozaj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gzqbigerx.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gujmhzkcz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/ghbwtwgdc.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gwnxhrgvf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.tarul.cn/Article/details/gsondmdvc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.bbcook.cn/Article/details/gkndzxuza.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gazshpabx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gtjdebfgf.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gucfzxypq.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gxdgrfens.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gvskyqlti.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gafpvbsay.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gmeoqvcea.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gjlaizfhm.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/geydabgje.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gqjzcrxlk.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/ggyxbudup.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gqqarmixn.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gznngoqiu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/geehihanu.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gbnwxcqbd.sHtML


<!-- 参考信息 -->