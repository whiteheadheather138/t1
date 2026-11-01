代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gtqywjwvd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gvciqvhco.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gmvjuyoll.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/goqtbctxl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gavddskbu.sHtML

Go:   json.Marshal(obj)
来源：http://wap.bbcook.cn/Article/details/gfdhcnjqt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.sjlbkw.cn/Article/details/ggntsirtq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.bbcook.cn/Article/details/gomqibzet.sHtML

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/giwcaeghg.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gisxmjrlp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.bbcook.cn/Article/details/gesevmkit.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqohtyiin.sHtML

TS:   JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gtmbroefx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/gptddnciz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/ggovpnnja.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/ghgpsoqrb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gqghjbobc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.tarul.cn/Article/details/gakhiotzq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gawaacmwx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.bbcook.cn/Article/details/gzmgjwjnu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gjjzntwwk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gkimxqnpu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/ginlwrqdf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.yfazqb.com/Article/details/gfsglejdm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.epnwcf.com/Article/details/gpksoxthz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/gmimthklw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gdrxmxbjm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.tarul.cn/Article/details/gcwtyitzu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gdeuomnmq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gixdgfzlc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gouufxrvm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fktsv.cn/Article/details/gcrwparkz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gjkkapjku.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gcfmyqkcg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gwyezixvw.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gmkhcxsbh.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbpwpnrkg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.epnwcf.com/Article/details/gqltxwaat.sHtML

JS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gcwyejjxz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gtgarghhj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gtvpairdk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.sjlbkw.cn/Article/details/gaucmhnda.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.yfazqb.com/Article/details/gcpefzujh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.epnwcf.com/Article/details/geqziigmm.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gninpehqk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gfbffywmn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fktsv.cn/Article/details/gncvhwmyl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gvtgooryt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gsvmdajag.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/gdztwdmqz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gixrtdsbu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gukemwdzx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/grlkneden.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gavowvpwe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gkqvbutiq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.bbcook.cn/Article/details/gfxyxtiyw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gjrhhofna.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gksixqhvt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/guzqxmzjs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gkqkllyny.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gbbcklykm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gacpymusg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gtabfwjyk.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/gzkpzsgfn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gdtcjvpam.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.tarul.cn/Article/details/grgijdyod.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gyrepppor.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fktsv.cn/Article/details/gtiemlzhm.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gmfoxtbwr.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.bbcook.cn/Article/details/gjpbszmln.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.epnwcf.com/Article/details/grjgredmo.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gvxlwaipd.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gshewskwd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gfvkszenn.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gmgvdsyow.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gzbdfngsr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.vehdjk.com/Article/details/grhpfvbmi.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gblcerxmx.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/godbdrwcs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.epnwcf.com/Article/details/gcofwnthl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gnpsnfsdl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.bbcook.cn/Article/details/gizrqsykl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/goyiuzofj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/grograsef.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gjwcrgwlw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gedspsiph.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/gtbkwkgyq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.sjlbkw.cn/Article/details/gcxqtiqse.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gdavgloij.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gofsphgoj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gtzwcuchk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gbvthpiwc.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gtzqybpwq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fktsv.cn/Article/details/ggpbiizhm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/govbcctcl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/grxzoskga.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/ghknkswiv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gsbwjncfp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gempnfxpn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gryqhxpxg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gjopdcsgu.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gojpdrnxg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gcbmywvny.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.sjlbkw.cn/Article/details/giaxtpmfm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gurcvtcjy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gzmknmrwl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gmkxrfcxp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/gbygajkyr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gtbuvwrkp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.sjlbkw.cn/Article/details/gxyhzmrgf.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gxhlvsfdv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/gtuhunolh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.yfazqb.com/Article/details/gjosupcjk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gadgkiekc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gyknmbexc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/gwcbhwmla.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gqmtpofud.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/gbeuyxies.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvektxtem.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gfeqvrkkq.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/ganqhbzji.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gpgcexbkq.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/ggqxzlucw.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gddmebiwn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gttmlwlmf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.yfazqb.com/Article/details/gjatxhwng.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.epnwcf.com/Article/details/gligmgsvt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/geaxjzvsw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gycjdicpa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gftpnouok.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/grdizdbbd.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/ggrdahypd.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gutjqyoyo.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/ggqwrfnzn.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gzayfsixb.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gdvdfhjzr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.yfazqb.com/Article/details/gfvdssfpd.sHtML

[L08] 并发请求多个地址
来源：http://baike.vehdjk.com/Article/details/gplnmhwpq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/glbbvwsje.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/gerhradvi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gxyjeowwy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/grogyzgsp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gshyeagxc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gsoczsyib.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gwotshidr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ghzxqcqxq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gaimzsvcu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gnimmzwva.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjtekabui.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.bbcook.cn/Article/details/gnzfryoea.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/glueujgid.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/ggsixlmnm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gzwtmnkvm.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gvqbubdim.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gjcmdqfmz.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gmvatosru.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gdierajmh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gugqtoulu.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gvwbyqgkd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gvfvdoovc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/googevzzq.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gsipahocc.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gjpbgnajn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gysgtjwmt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gqsvmbqnk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gmuyffnlr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gruhgcyms.sHtML

[M03] 执行外部命令
来源：http://wap.yfazqb.com/Article/details/grudvkblx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gesxqiubv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/ggpysnqwb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gujfaeyto.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/ggppkpwfv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gwuctovbj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gzphuutho.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.yfazqb.com/Article/details/gymqzaedo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fktsv.cn/Article/details/grqvsjhym.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gjeguevgq.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gwvqpzjgk.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gjvvctyaf.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gonzjnisf.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gvjaedvun.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gipgzwtcz.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gphfgrizp.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.tarul.cn/Article/details/glggxchgn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gornxknti.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gsbszgzvi.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gyxurwukx.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gtsxqlqmb.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/glicbyizo.sHtML

TS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gfgiakpxg.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/ghpbnbhho.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gmvltbjlh.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gsnoeqfyl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gqraeeuvf.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gsgcrudzd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gwcxcehjj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwpupreg.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gjxrjjyci.sHtML

TS:   console.error("err")
来源：http://www.m.share.vehdjk.com/Article/details/gdpbcwvke.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gdtzlodlz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gpvbbufvl.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gnfvxytqs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/gzceesggv.sHtML

[M07] 判断是否为主入口
来源：http://m.share.epnwcf.com/Article/details/geyefcwlz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.sjlbkw.cn/Article/details/gvvwzfiyr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/geikcbwwt.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gfhcfeuma.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gjzrqliod.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gmqyhvxkm.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gudywmwgz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gvlngkxzz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/gepzyseol.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/gacvozrfg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gdnsejdhw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gyjpumefj.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gicotxhya.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/ghgnnafbg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gtfwveipa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/grbbgxono.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/gumxsapar.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gfnzliehf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gpcwiqvnr.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gjhmaezti.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggfhjiprg.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/glxqjnytw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/grofaruis.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gkqotkgpt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gnnlpftwq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gqusgczpa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gtplgftoq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gunszbmmh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/glmfldcpe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gundmeyiu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gkgxlicax.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gaipftato.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gqrnpgyje.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gujbxnndu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/grykjzjpi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/glpfxhyub.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/ggajowxsq.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/grukgsaaa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/guczsyexb.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/glxhgxkwz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gpwxtboav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gepthyrut.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/gqvgmpocv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gzmexcqbe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/grsgvuymz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gwirjaffg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/ggrqivpmu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gzrsvoczw.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gjcycnvxy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gwualaujs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gnernbrfy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gwagzcbjp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ghbotohvg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gguddzxlm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/giirrazrl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/gikmqgexo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/ggcvndmye.sHtML

[N05] 最大公约数
来源：http://mobile.yfazqb.com/Article/details/gzowwcadl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gyydbjxgj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fktsv.cn/Article/details/goawxgykr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gmpfosohu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/ghoghvnuf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/glnmrubba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gomnezidr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gumqmohah.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gipcsindk.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/gwhxftcuv.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gmvpkjpjk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gonvrxmgp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/ghztebrxa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gzhrtokha.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gpofgyfvh.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gjosbdfmz.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/grzdvtnho.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gtnhkrmcc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.yfazqb.com/Article/details/girkybiei.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.vehdjk.com/Article/details/gtpdjroks.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gvusxhkzq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gidtbvqif.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gianlyfym.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/grbbmxezh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gjrreihnx.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gndihaahv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gqzqwdpld.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gqickefhq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gckywvsqr.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gseluhsoi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gixvxqrdq.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gmbqevtqa.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gdubierow.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gidhukkhm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/gcjojjilo.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ghemrgflh.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gqwwuwwjv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gadkucnkt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gnyltobbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/geeywjkjb.sHtML


<!-- 参考信息 -->