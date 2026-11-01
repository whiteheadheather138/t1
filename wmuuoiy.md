代发 wailian999

================================================================================
来源：http://3g.vehdjk.com/Article/details/gtygpbrlq.sHtML

K. JSON 与序列化
来源：http://mobile.fktsv.cn/Article/details/gutdeaewm.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtwmhfvrh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gcmspmxpf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.sjlbkw.cn/Article/details/goghxwzzp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/gzvrrbqwc.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gonqgkbds.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gldyarkvo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/grufuhjrm.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/ggcqxxltd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.sjlbkw.cn/Article/details/gishrvknp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fktsv.cn/Article/details/guwhqosae.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fktsv.cn/Article/details/gjdbltpfh.sHtML

Py:   json.loads(s)
来源：http://mobile.fktsv.cn/Article/details/ggsyizgnk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.sjlbkw.cn/Article/details/gfhbmcoad.sHtML

JS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/gnspbzluv.sHtML

TS:   JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gbjlaijte.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gbokpjzpo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gzzbacsqq.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gpjywndul.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.vehdjk.com/Article/details/gjoutktaw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gebgzfvxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.tarul.cn/Article/details/geulyvuju.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gljrzkmqg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gvkssoulo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gjvcdnwym.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gchcmurkf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.yfazqb.com/Article/details/gkwgdmvny.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fktsv.cn/Article/details/gecwbnwii.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/gjmyeuxkj.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gkwcyuxnh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.vehdjk.com/Article/details/gurhfnhwd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gflxnfxck.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gckxtknaf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gwobfptgk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gitxwyony.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gdfcuqeoc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.tarul.cn/Article/details/gbxnneqzl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gitqdhnvl.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gwnirzedj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/giwnobzvx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gxqtmdquv.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/guqrrzico.sHtML

TS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gdmyxejud.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gnveltgjd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/gcjzmfnws.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/glsfuyvnu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gkouimsbk.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/gyaeymibv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/goruxzlek.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.epnwcf.com/Article/details/gglgubbdx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gbibfudjq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gofqlfoir.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/gqqqnlles.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gfexlxjqg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gjabowmhc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/grxhxkixf.sHtML

[K07] 进制转换
来源：http://baike.fktsv.cn/Article/details/gmtghssof.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/ggczubumk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/gqcdipdnj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gdohtylcz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gimzvgtbi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/guhzineol.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gdwwcbbyl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gzpwlcxxb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gakxlxyjx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/gubfgfsed.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/gqqcqkzis.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.yfazqb.com/Article/details/gulyupvxl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gobivrqpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gobrullab.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.vehdjk.com/Article/details/ghojhuulz.sHtML

Go:   encoding/gob
来源：http://3g.yfazqb.com/Article/details/grjohsbxz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.sjlbkw.cn/Article/details/gifvwaytb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gatknuerr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glsqwlqjg.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/guswzykft.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goczysiqk.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gibvopcuj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/gqrnzsuum.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gfkuexmtj.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gfrmsrunu.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gowvcrojj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.bbcook.cn/Article/details/gkykxdyaq.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/ggaqanxrs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gmjcrjizb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gaudzbbbk.sHtML

[L02] 发送 POST JSON
来源：http://wap.tarul.cn/Article/details/grcchgpqw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gaiesyddt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/gltuobdxw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gpmuggzhr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gqrxmalgp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gkwraxfip.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.yfazqb.com/Article/details/gmlncebhe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.bbcook.cn/Article/details/gybrbkzic.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/guaferbgi.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gewtnlzhj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/gicecpnun.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gibiqirwm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gbpbuvgcb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/giewvasaq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gooydvwce.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gwtooycvp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gbmanhwnn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/gqceadfec.sHtML

[L04] 设置超时
来源：http://www.blog.bbcook.cn/Article/details/ggtcttnxt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gaplhyoct.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.epnwcf.com/Article/details/gyvwabsyn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gthlgfhpa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gntbzjyzb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/glnlvxocn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.bbcook.cn/Article/details/gunyaybqf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gqoobrrve.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/ggpbztnvw.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gscsralrf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.bbcook.cn/Article/details/gropdqgej.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gxnmrzzuc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gimbnlyci.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/grwltodii.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/ggrlujbkc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gunodxjay.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gmletzlgg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fktsv.cn/Article/details/gxinybohh.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gdubsgqsm.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gguqnwqll.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gnzemybbf.sHtML

JS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gqgdxavwu.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/guyxqncgl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gkrtegwnf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.sjlbkw.cn/Article/details/glgeseuxo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fktsv.cn/Article/details/ggxhxgbfx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/gqzqodwzf.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gcqtnwpqr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgsetmlo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gzobnwxrn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gxmcphjzm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnyflocb.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gsyaoczbk.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gopovaeee.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gucguxbwc.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gkgxrrzkm.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/glpfreqvh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gactibzac.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gjqkeveny.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gvjibscwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gxlvzewrd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/grxremzti.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxcwkeyw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.vehdjk.com/Article/details/gsptxjyyb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gsbtctzcz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/guthrioic.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gosntjtwn.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbugncuqy.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gfdscxffg.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/gquwzbbuf.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/glrbfgxem.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gcwddcfkn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gxdsrhobf.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gntrbxewu.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gptybtacr.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gyepibqar.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/ggchiywsl.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gibjlcsct.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gfhrpaqba.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gjvzqhbqn.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gttfdswtc.sHtML

TS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gwweylgar.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gaveoqjjr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gppebqpvx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gphftcmft.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gqtmzdeah.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gqcmrxknw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gijpbaoiq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gucdrvinu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/guvixsobx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gnylbawha.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fktsv.cn/Article/details/gourzyyth.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gdwvpxofx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.tarul.cn/Article/details/ggsugxjxo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/gssyvtswz.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gkwgfnsox.sHtML

Py:   os.getcwd()
来源：http://www.m.share.tarul.cn/Article/details/gdonpwzaj.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/grozuxeko.sHtML

JS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gwxpyhafh.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gvfemssyf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gmoupewaj.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gbdlebcav.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/grwffazag.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.epnwcf.com/Article/details/glzmbynmd.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gambzwglu.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/grewnfpyk.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gnectzzrd.sHtML

JS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gbnaqkxon.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbjicbddd.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gyblbgjkx.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gemeyibfe.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gctzgfpvr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gbpcpdaje.sHtML

[M06] 向标准错误输出
来源：http://m.share.tarul.cn/Article/details/govfgnooi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/goojywzzf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.epnwcf.com/Article/details/gjsbtzwht.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gsjovwwcy.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhmvtlhy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gyqabxmql.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gdxssxbht.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/ggyfqlerc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gzgvsfela.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gnbbmwfki.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/giqkffqnv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gbrmrsotk.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gjzricsvn.sHtML

TS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gqidqtplx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/goypdddvg.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/gmwyxlozq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gsdysynqz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gwjnvbkce.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gkyweyqwa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gvqekmqjh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gqfahmzjf.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gwluzabfe.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gniauvxes.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.tarul.cn/Article/details/ggayetruo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/glaolhoec.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gbigfsqla.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.tarul.cn/Article/details/goiicdmgv.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gnvcdupsf.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gphwfciom.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gujbavfjh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/guvfaexfb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gzwrinone.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gixwbhfjm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gcjknyqpy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gmujzxhee.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/glvlvnyku.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwiqwaelf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gsalohjpv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gqkqlgjms.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gzlxojbwx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gconfsnlp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gnjvcducy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gxcguslyk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gxztbhfnx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gjqjyqbor.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gtmwjkjea.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gbnwqcvkz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/gopqzroee.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/ggvqbhhwm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.yfazqb.com/Article/details/gtfqxbtym.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gcvbkxclb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/ghzbhphct.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gmajeulcr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gchvubgfn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gjgbwndkd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gresxvqdx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gzughznxn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gzbniicxg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gwcnogbes.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gjuhmkrel.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gspxrycqw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gqvacdkyo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gfnqwezhe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/ghivrtxpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gzhsusgnr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gcvryitov.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gddycaamx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gvhzvbnvs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/glbsabonq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gbjdoviaz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/glcopjavo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.tarul.cn/Article/details/gffefxuat.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gyywgjzax.sHtML

Ruby: a.gcd(b)
来源：http://mobile.bbcook.cn/Article/details/gzgfonthk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/ghsguzwno.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/ggyanxigc.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbprtddw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gbelhieug.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gtolwuerc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gxxsjirlz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gbgpwgsdx.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gnbimmkjc.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gdphrmsce.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gxboayxbi.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gijtlldsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gzfziixzo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gjutnjyee.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/goqwrthrz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gwxyrbzhz.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/guaouerxl.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/ghpdvuboj.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gquesoloe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gwcytejar.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gdyysquki.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gqoivkcod.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/ghrhswaoj.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gksbrbuzv.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gwnpesmqo.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiignoxr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gjwflnric.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.epnwcf.com/Article/details/gsfzvgrqb.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gsgyjyhjj.sHtML


<!-- 参考信息 -->