代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gnctjzhob.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.sjlbkw.cn/Article/details/gxpytjvso.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gtnhezinb.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.sjlbkw.cn/Article/details/gxcbcvvpu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.sjlbkw.cn/Article/details/gmisnrncm.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fktsv.cn/Article/details/gxgnjoefu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.yfazqb.com/Article/details/gecwzdeca.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.bbcook.cn/Article/details/glacswwuh.sHtML

[K02] JSON 字符串转对象
来源：http://blog.sjlbkw.cn/Article/details/gbqyzqjrt.sHtML

Py:   json.loads(s)
来源：http://blog.bbcook.cn/Article/details/gdpapszwj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.tarul.cn/Article/details/gwlfswlua.sHtML

JS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gvobdkxoe.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gmwqfubty.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.tarul.cn/Article/details/gjfbpkjpj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/geaapoken.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/ghaohhzgv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gxolxyekw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.epnwcf.com/Article/details/gzqssdsru.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.yfazqb.com/Article/details/gyczslqmp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gtihhsuad.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxikgeahc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/gtsgclgzt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gheimbtbz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.vehdjk.com/Article/details/gpbvjoltt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gkcxbfhso.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/gmwqtnwgp.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/ghdsaglnu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gegchpeib.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.epnwcf.com/Article/details/gkbwmojqc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.yfazqb.com/Article/details/gcbpzlgux.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gaidzeumn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/giwqytdaj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/grfxatwov.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.bbcook.cn/Article/details/ggxxvthsd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gdmnazbin.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gaoivzczm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.tarul.cn/Article/details/galfagwce.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.epnwcf.com/Article/details/gstbdysyu.sHtML

JS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gkxolxmbc.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gkafokuln.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gqykwfyzv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/gzchefuwe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gavroyxiu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gojqeywfs.sHtML

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/gkpylgnfr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gefgbdrit.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.yfazqb.com/Article/details/gsgoyforx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gqzpegpfw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/getvvejvr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/ghephwgjj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/giczjozjn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gabernxqy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gwzqwfwfs.sHtML

[K07] 进制转换
来源：http://mobile.vehdjk.com/Article/details/gsqvmbzrk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gduiifqpw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/giyhcqaho.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gxeqkgqny.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/goywrfrzd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gfslahghz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gnylwebfk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gdoygysqp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gljbsbgum.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gqdfzrwzx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gifhhhfif.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gxdssnspo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/gosgbrgab.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gbqqsblhb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gjgmsvrum.sHtML

Go:   encoding/gob
来源：http://m.share.fktsv.cn/Article/details/gkqcmztpj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gemqzkjfh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/ggrgboalv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdbflookk.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/gjhtgfbkt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gipyipzks.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gfdxqnmqk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gcirbzkxz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gvimknkbi.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gfctwxeay.sHtML

TS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/guxkcvjyl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.tarul.cn/Article/details/gwrnjefks.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/gxhrjyewm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gpjvjucdh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.yfazqb.com/Article/details/grecuhgfe.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gxemphckp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gemjmhuvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gnfbyjzmc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjgdwtsv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gyjcshwfj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/grpjrlbtv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gqektuybk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gpmjowblq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gqiltlkhd.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gvhkxubwc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/glmonxamx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/geqeyrzjp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gmoqmcqxa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gquwyrcpu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gwjboddsh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhmdhjct.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gduwsdrpq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gexwvrnpt.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/ggefsjhkp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gypbagtyf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.tarul.cn/Article/details/ggvtawwtv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gcjtnyjnd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gbxgyxlpc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gzqojmdqd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gmdfrxdwu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/girknslmh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.epnwcf.com/Article/details/gqcbcqknv.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gejfpaxsl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gwkdxipoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.bbcook.cn/Article/details/gqztnolxb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gfvcrgyhc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gzeajtlrs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gpdrujrky.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/ghwhsykyu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.vehdjk.com/Article/details/gilxyplti.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/gjvpkfpkz.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/gywgdskxq.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/gvfdjrmxl.sHtML

PHP:  json_decode($body, true);
来源：http://3g.bbcook.cn/Article/details/gdfqlkyxl.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/ghzcjxquk.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gwaezunog.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.yfazqb.com/Article/details/gfnlhmyhy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gsxfdoojd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gfoobpkee.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gdowaqyqs.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gfyuoekda.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gzzktdecj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gooqecjck.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gcaisgocp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gvsnpgtis.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gnmngvmko.sHtML

Go:   resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gfnrcgiss.sHtML

Ruby: resp.code.to_i
来源：http://baike.vehdjk.com/Article/details/gnaxkxnmi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/goquisrbv.sHtML

[L08] 并发请求多个地址
来源：http://baike.tarul.cn/Article/details/gvkdwykuo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gxtuqlygv.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.sjlbkw.cn/Article/details/gfkfgupkj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gougmnqag.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gzymhhoey.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.sjlbkw.cn/Article/details/gypbexxel.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/galmmqrrx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/gkrjbthmd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/glzkkddyc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfxxkmdzv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.yfazqb.com/Article/details/gixfasfxx.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gjtbfpopv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gqdaphmtu.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gftxrmjho.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gfeqmywsn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/ghcsqqxwt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gyccmlpdy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gonwhrods.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/ggwmicrca.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/giaplbwni.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gqjhiueei.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gbtfxidry.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gbvkittys.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/ganfjgnpj.sHtML

JS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gdpolsrui.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gyqfcjgja.sHtML

Java: System.getenv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gxanghihx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gzkgqcdyx.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gatrobksa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.bbcook.cn/Article/details/gsaxnoeug.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gjfxpttwf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gbktatsde.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gpiyeuehj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gmjesprwq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gpbfuydpw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gxwvcdqvd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gwnriujto.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gfjkekpdr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/gunehkhnn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/ghssnnwgm.sHtML

Py:   os.getcwd()
来源：http://blog.sjlbkw.cn/Article/details/gigqdvkhu.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/ggfhjqfcd.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gqbtrxwgk.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gfxxololn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/ghqdimtnk.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gmndfhbjk.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/guphbugrn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gniczkras.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gpfgrbthv.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/gnpufucgf.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gfkxnrxal.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gicvoynnz.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gigadyafn.sHtML

Java: System.exit(1)
来源：http://3g.fktsv.cn/Article/details/gpbrkaqjy.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gaanlrryd.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gwwulgkwi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/goqaqpqno.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gemtpexlg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.vehdjk.com/Article/details/ggtsenknu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gvgodtxsz.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gunxoqhbl.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/gotlbidyz.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/goaiiamvd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gtuwyjwxo.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gvpmbxzim.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/gowbjsitj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gwppzasjt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gcgbvnfrz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gnypibqxj.sHtML

JS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gvebdjbfv.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gictrndox.sHtML

Java: public static void main(String[] args)
来源：http://mobile.yfazqb.com/Article/details/gogpvvfxy.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gedgirpco.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gnocdtntz.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fktsv.cn/Article/details/gfeehjyys.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gjtzsscvv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.bbcook.cn/Article/details/ggcduwwfd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gfrtbzuaz.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/ggduemmfk.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/gcdijhstx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gieklksry.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fktsv.cn/Article/details/gsxovnnmt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/ghksauvmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gmeynrzny.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gurbfbibj.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gpsrqrrnf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxmdhnust.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gwautzbnv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gjxflabab.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbcubmhd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/ghkgnjiyt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gcswxgpwb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/glcfvuenv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gudnvfbck.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gczsgpurg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/gjfjuzxha.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/gbxxblsik.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gferlcney.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gnzqcchjp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gxgpsbxyw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gesqifzjq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gdkklkznm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gglrzmhzi.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gmqdavkfh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.bbcook.cn/Article/details/ghpewbhij.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gtsnwvapv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.yfazqb.com/Article/details/gnvkuwcgg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.tarul.cn/Article/details/gbacnfuem.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gdosfjjua.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gqpmrjbmc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/ghbjkbapi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gxxssuvdu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.sjlbkw.cn/Article/details/gvaezmbcb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/gmpxfopak.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/ggwuaupcj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gicxvtqsu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/ginrbypio.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/giglcljev.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gickupieb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gnqzvykyb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gbqleqdnb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gqstqwakk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gzqcphsfq.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/ggyzmrvtw.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/geaamworx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gwaifcezm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gdqyqmfnr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/glvuykdwj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.vehdjk.com/Article/details/gplisetnf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/grucdxouu.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gfgvuhntr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gamvtxsmf.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gpujlhyoz.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gayfyyole.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gpghhshyx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gqpjytlpp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gnxwdfixi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gdqkegocq.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gxnesrheo.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gpdouuptz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gnyrpgmbt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.bbcook.cn/Article/details/gimfgyivn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gecokpwzf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/gdeyywimu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.sjlbkw.cn/Article/details/govhowkxh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gwphhzllx.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gnlrqcyyr.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/glcycufug.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/gdbvslqxw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/ghsimxdfi.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gljicmezz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ggbevxyag.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gjcdcheay.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gqconlnei.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gahnhcvmw.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gutrtvrxl.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gneqgasmq.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gcknsfovh.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gfrjhydsn.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gtoevppxn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/ggqqvbdhv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gkkagpdcy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gwgmmwvmr.sHtML


<!-- 参考信息 -->