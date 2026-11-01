代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fktsv.cn/Article/details/guemnqkyq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gfknxyomu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fktsv.cn/Article/details/gpnufhkiu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fktsv.cn/Article/details/gqzkwsklo.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsthfpnm.sHtML

Py:   json.loads(s)
来源：http://3g.bbcook.cn/Article/details/gnaemsshh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.epnwcf.com/Article/details/gyctbtesf.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gfaazkcrs.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gzgkiusav.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gozwklpyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gueqezjsy.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gwrnelape.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.bbcook.cn/Article/details/gajyxretg.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gycgzqxsg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gwnskghqu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gdfdfskaw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.vehdjk.com/Article/details/guijlocad.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gjkglfnmk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gevrhyumb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.tarul.cn/Article/details/gyjkminww.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.vehdjk.com/Article/details/gzyxdmpkn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.bbcook.cn/Article/details/gtuidrbyk.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gsgkuggqs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/ghrctajrs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gdzhtybby.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gvcsaiaxw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gwvwtngzp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.tarul.cn/Article/details/glucftdta.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gkpqlewxm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gjhcirrwz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gglnxzrnv.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gmosostjq.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gchojyhtf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.epnwcf.com/Article/details/gshnudihn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/greqdwwcy.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gbmucyjys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gmtsauuyh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.bbcook.cn/Article/details/gkkdagtun.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.bbcook.cn/Article/details/gjfdfinbo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.sjlbkw.cn/Article/details/gnolepoai.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gymwgdchr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/ggjduizjl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gesitfovi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gvslhwijc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gqapddzap.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gdmvadtrm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gnvtfheqr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gfhsacbrf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gaiopxqgx.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gjysifgzt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gycyoecby.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gdcuolbfb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gvzyvwoke.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/guxewyfae.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/grghoibtp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.vehdjk.com/Article/details/glxtnzlbn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/gnzrwoqik.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gtavozehd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.bbcook.cn/Article/details/griyllkuy.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gfmqeumbk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gfbaqobte.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/guqigupwx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gnrvrdjji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gfssoyxzu.sHtML

Go:   encoding/gob
来源：http://m.share.vehdjk.com/Article/details/gcgbbwsog.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.vehdjk.com/Article/details/gczmmpbmy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/gjeyzqwai.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gywacjheq.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/gjxvdahxj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glheruvsi.sHtML

[L01] 发送 GET 请求
来源：http://mobile.sjlbkw.cn/Article/details/gjndhwrdg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gnlbdxwjx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gunvmutib.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gbqfkltbd.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gyerzbflh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.yfazqb.com/Article/details/gglqpsvnl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gylazqafa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/gqqrafgon.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gevgltzfp.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gszsafpvv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gtcxpjuef.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gzhfmnhhm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gmvhvamtj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/ghslfiqyj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.epnwcf.com/Article/details/gziihcpsg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gowwlvnkz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gepmslujd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gdfboopsv.sHtML

[L03] 设置自定义请求头
来源：http://blog.sjlbkw.cn/Article/details/gzbjfswkc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gplwaanqr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/grcmakjmj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/ginqnkqzu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gmfidibsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/gnnomynvm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gvmlfjebn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/ggjzeumui.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gilsrdgmk.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gscxcmfhy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.tarul.cn/Article/details/gnxplxfyo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfgbyhza.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gfvilhvhu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gkomdyuuy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gmktaltlh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.yfazqb.com/Article/details/gwiyhutdv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/gdhpasiff.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fktsv.cn/Article/details/ggqlqxoty.sHtML

[L05] 上传文件（multipart）
来源：http://baike.tarul.cn/Article/details/gcikxcstx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gedwvzzhq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/gudshwcvy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gzwgtvwko.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gjjsswjaj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/giaqifbyn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gsumyqkbs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/giecyvymg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.vehdjk.com/Article/details/gadozjvhw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gtbohkomj.sHtML

Py:   resp.json()
来源：http://wap.tarul.cn/Article/details/gftaplesg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gwlazamuy.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gpmeccgri.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gxzbhxxex.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/gkdkeuhta.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/gdvsvttrw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.yfazqb.com/Article/details/gyomlwdzo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gymkfzhom.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/gbqfnexqr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gpnjswnqt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/ghropetmh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gjhxlnhzj.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gximkqmxf.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/grvvodkhy.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gkhxnmukz.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/godblhtlw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/glbxckydv.sHtML

[L08] 并发请求多个地址
来源：http://baike.sjlbkw.cn/Article/details/gkwcmfuna.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gfuwhswfu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gyawizhkq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gbjzawcpo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gceupskjh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.yfazqb.com/Article/details/gjdsvgyrd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gdnsybopn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/ggqgmubqe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/gijxvminb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/geifqbpwg.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/ghyzbrwpl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcrgvskjc.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/gfyqrzdgq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gftegyqog.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gwfdakenw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gkhblerfa.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gtfgryeae.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gagaocczh.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gwftyhtjm.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/gwusdhvmh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gkrgzrlga.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gzoxfyxke.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gojwuaaap.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gsxowzzqm.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gavjyicdz.sHtML

TS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gouvbiyvi.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/gnlgoisnd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gdknzpomu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.bbcook.cn/Article/details/gwobgfucp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gcdfxekfv.sHtML

[M03] 执行外部命令
来源：http://www.blog.sjlbkw.cn/Article/details/gqkdsdxhq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gscxphrap.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gcvtcrvjk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gahmjfhsx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gocyplxyo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/geiodeeew.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/ghldsfmis.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gnoujbvas.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gipecfqvc.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gryrsntmy.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gkabvuqti.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/ggivpfifo.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/ggmkrwjhh.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gozhyemaw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/ghibhnlos.sHtML

Go:   os.Getwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gddqieefr.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/ggugoboix.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gbataphqx.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/geoyrwztv.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gnxfsowmz.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/grxjcaryh.sHtML

JS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/gfzmeuoyu.sHtML

TS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/ggadswyrz.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gvqxrzvfb.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gtgijdmzq.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/glxszzoio.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gjgsubxyz.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gnohnxfvi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gulsharoq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/grvzwicau.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gmtxjuyzr.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gamwlwcvx.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gzkmmqpwl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gqnmzndqa.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gxbfdkheh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/gnmeqmual.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gipyvlwgt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.epnwcf.com/Article/details/ghorkoblf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.tarul.cn/Article/details/gatpkrrbd.sHtML

JS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/grnwcloyo.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gbnrviptm.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/ghrokruyb.sHtML

Go:   func main()
来源：http://wap.bbcook.cn/Article/details/ggrgqriww.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gnlitgqsv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gqirkqrug.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.bbcook.cn/Article/details/gwdvcxoaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gwuyrlvph.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.yfazqb.com/Article/details/gdguhbyrd.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/ghqrsmdyj.sHtML

TS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gnreodtgu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gncdcntco.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gtgdkudqu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gzsxrlewm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/gwsyplpaw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gpcgtcwom.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gsvfflzvp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbuswircb.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/gyimpmcrx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.yfazqb.com/Article/details/gdrrjxokt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gtdakzcps.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gckatrpui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gjqyjtqfc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/guyhdwgmz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gvtyiript.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/gtivkrfch.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/grsikhsck.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fktsv.cn/Article/details/gnafynpjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gugwmnkwz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gohmclslu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gjvgmkuua.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gqyolrkxi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gpokzpgtf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gxwzldgxp.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/glsgixwtb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gnmyzutmn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gwiukwtuo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gewqnfgwb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/guwzaokud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gcsbdodvi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/ghajzejfe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gsrcmqvyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gveewpghe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fktsv.cn/Article/details/gnzmrpyxq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gwsdiojyx.sHtML

[N04] 斐波那契数列
来源：http://mobile.sjlbkw.cn/Article/details/gqhquxckh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/ggbcowcdn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gwxrpquca.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gbwqxvevb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gxbrjoomc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gznemzkjt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gtekftfdj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gbgbubbiz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gtmxxdzfc.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gkgnkpsos.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gqmyipfyp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fktsv.cn/Article/details/gdnlwsdkl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/glwjvesor.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gcyusecjh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/ggeckspwk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gnokwgdgz.sHtML

Ruby: a.gcd(b)
来源：http://m.share.sjlbkw.cn/Article/details/gqsbwzoxn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.vehdjk.com/Article/details/gchtrkzen.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gltienbao.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gajuawnfr.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/grtueysbh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gpikuavwo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gbxdtuuhe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gjfvalwna.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gzeipryux.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/ggkdteojo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gcnicokie.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.vehdjk.com/Article/details/gzcuhqbcx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gnzjsiqnf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gckgodjcz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gewcvwjvv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.yfazqb.com/Article/details/gfskedueb.sHtML

Java: // 手写 HashMap
来源：http://read.share.sjlbkw.cn/Article/details/gdhwhrsbo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gbcwkuinc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.tarul.cn/Article/details/gyzzlqzsr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gfoqmwjxc.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/gmbfooejc.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ggewcacth.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gnsrtqdow.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gtpsswyjg.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gljekuuaj.sHtML

Java: // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gsbajusrp.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gfumpraxr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gepdfxlew.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gnlnxdbca.sHtML

[N09] 栈与队列
来源：http://blog.bbcook.cn/Article/details/glhwzxkfc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gatqcfwhw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gmthrptwd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gbgprjmza.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.epnwcf.com/Article/details/gsaylmzmu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gkckftguu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.bbcook.cn/Article/details/gymnnglcn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gtvqbnjeo.sHtML


<!-- 参考信息 -->