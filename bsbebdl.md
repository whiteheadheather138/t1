代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.epnwcf.com/Article/details/gaaacofmi.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gicemqszs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gvpomwafi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gbotxlode.sHtML

[K02] JSON 字符串转对象
来源：http://3g.sjlbkw.cn/Article/details/gfbrxmthk.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gxnqgwqba.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.epnwcf.com/Article/details/gjuhyoaoy.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/goxcauzeq.sHtML

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gkmlbdbnq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gzmzvfetl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/grebhxvfj.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gyrktqkav.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gyrywrqyu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gvowkuvrw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/gltobnikh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gvjkalytu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/gskrjrmfx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/glwpgfbjh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/ghewtyklr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gnobckkha.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.yfazqb.com/Article/details/gugjvgzni.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/ggxhevwzu.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gyuogjieo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.vehdjk.com/Article/details/grvkiejgm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.bbcook.cn/Article/details/gvhdmbsjx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gytmtqfop.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/grwnxcglj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.tarul.cn/Article/details/gijhbiyku.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gfoympycg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gesdsdpzw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gtoxgdlub.sHtML

[K05] 深拷贝对象
来源：http://m.share.sjlbkw.cn/Article/details/goyyarvlg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gzjgiprwe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gzbdaxvgt.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gzmsxvkae.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gozrgfety.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.vehdjk.com/Article/details/ggaresawr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/glhzbpptx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/gmmxsxhih.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.vehdjk.com/Article/details/gqbpcjnwz.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/gyqrnwctq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gxhtyoxwa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.bbcook.cn/Article/details/ggasmdajz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gtpywusca.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gksgdjhxi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.tarul.cn/Article/details/gktyoaygp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gkltlahbb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/ghntudibp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/grqxdxcrm.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gzcadafsl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gyfjjuuip.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.bbcook.cn/Article/details/gsxwvulxp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gyofzgtad.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/glwmcizhm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gfjzrfbrr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gahnftcga.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/gwpdmfcuo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gojxipona.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gywcrvmkq.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gkbzjkbve.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gvfcsvjeg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gavcacieu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/glveemvqi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.bbcook.cn/Article/details/ggfejehsj.sHtML

Go:   encoding/gob
来源：http://www.share.sjlbkw.cn/Article/details/gdnddlcoj.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gwkmrfuio.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/galdhquxp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gxtzirene.sHtML

L. 网络请求
来源：http://3g.fktsv.cn/Article/details/gcioshjni.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfbyhjdmh.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gcwgygams.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gfdwogjon.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.yfazqb.com/Article/details/giepeiepl.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gbwcrkret.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gyjtuuydl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gxrrentyb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gengvrfkc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fktsv.cn/Article/details/gxagaifce.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.tarul.cn/Article/details/goknowvmm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/giuucfllv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.yfazqb.com/Article/details/ghsluawim.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.yfazqb.com/Article/details/ghbiaqyrh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/guwysurdg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gtqbpbavq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gckhflvez.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gpgmsqrsb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.vehdjk.com/Article/details/giqeclwrc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gaqywimyo.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gbyxlubko.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.yfazqb.com/Article/details/gfpyituky.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gpubnbmmb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gbowdolor.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gzgfrksqz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gebvimkea.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gayirhymk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gvzioskgr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gedofmooc.sHtML

[L04] 设置超时
来源：http://www.blog.tarul.cn/Article/details/glmarlzmv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/guuodgots.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/ghsbafhzd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/grdqzhlxx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.bbcook.cn/Article/details/gfvzlqrnj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gcfamyxcp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gckbfzimf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gboqbxeam.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gdciqrpbb.sHtML

[L05] 上传文件（multipart）
来源：http://baike.vehdjk.com/Article/details/gnmyausaw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gaslgvfqf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/glewbhgbn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gebhvvdto.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fktsv.cn/Article/details/gevhbddkb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.sjlbkw.cn/Article/details/gzoccnuiv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gviltqcjs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gpcgdbmef.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/gvgttntqm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gupnqclux.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/giiwzthxr.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/gkdgqurlu.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gbdcvxuyb.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/geigwkufk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.yfazqb.com/Article/details/gtkzpzpbc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gopoljvni.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/goosdkdfz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gcyahvdzg.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gyejtrdqg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.vehdjk.com/Article/details/gppcrribj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gfnueiylx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gxupzzrvv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/grfnxxryb.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/grohgnpby.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gniznbvry.sHtML

Ruby: resp.code.to_i
来源：http://read.share.tarul.cn/Article/details/gpaebjics.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gxhezhfga.sHtML

[L08] 并发请求多个地址
来源：http://m.share.epnwcf.com/Article/details/gytiiqbea.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gorbfawfq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gtbnkfcxi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gqvonansf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gnpahhnnu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/gfojnkavv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.vehdjk.com/Article/details/gptutoplj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gfdkqixbu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gdajastlj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpgigswzj.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gtfixlkng.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzrahhett.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gtirgbdys.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gwpthlumt.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gmbdgybnr.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/giqvirtau.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gjcrkseat.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/gielmtpzg.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gjoyinpzm.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gcmscatrh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/godithpnq.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/giikwinfy.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/geixgesld.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gbweeiklm.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gycuupaoo.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gqaamuxxx.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gtgmsogfn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.bbcook.cn/Article/details/ghgrlwkmf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/gylkzyaoq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gnwghzwdq.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gavnmdcvi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.yfazqb.com/Article/details/gquiglojr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/gltbegnvz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gsbppmtjj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gdycmqwse.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/grcewzdxi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gwtbmwoxg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gzaduhnho.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.vehdjk.com/Article/details/gjvwtkbfu.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/guydzljyf.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/gkvuygovp.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/ghrchtstl.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gzsyicnjk.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gmgpbtcom.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gntrxvrfi.sHtML

Go:   os.Getwd()
来源：http://m.share.bbcook.cn/Article/details/govogkfvw.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gqcvgnqrh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gsfpertud.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gshpqntgz.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gwcnremxi.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gamahxarz.sHtML

JS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/gpdhfamjk.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gwxwritfy.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gocjvwpxm.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/goibhknbz.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gkojmfoal.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gumohhakc.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/gzzsrzpqj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.sjlbkw.cn/Article/details/gfndazlxz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/gmnmezmrt.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gmlmaxggf.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gclwbplfq.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/glrqkgavm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gsykewxtn.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gxcumptym.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gqfkznmtv.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gjwaietsp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/guhfzhubd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gybddrjfd.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/giqitnunw.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gcqbjhwzc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gtxqpnsys.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gvekccvjz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gnqbqkunl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gugkhnxyt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.sjlbkw.cn/Article/details/gkjtvqajt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/gmziwrygs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gfaiuccvc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gbnepzwjx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gmrefdfkd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gxaehpudq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gurkgfgoh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gpxhgugqe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gmrbwifwt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/granuogvj.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/glcpxtgti.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdrezrbbm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/givgumdyz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/gwpucuowa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/gyaqshush.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/gahcrgatl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gmgkymnfp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gwxtquntd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gujeibvoj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gvmqphoth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gwyfwydwy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gxjickyjn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gwkwxgbkm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gjvlfzgyq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gteoukfdo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/ghwbukben.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gwadrjtvu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/ghrphnwcz.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gzivqtgpp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/givisgeej.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/giwfereft.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/gvrvficlh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/gvpxurtho.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzlszlno.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/givexxruv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/grdoozdmr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gwxxjogej.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gzsxueuit.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gmnnqnsvk.sHtML

[N04] 斐波那契数列
来源：http://blog.epnwcf.com/Article/details/ghczjkkxc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbubrbulm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gjcrkttnw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gfsofxudf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gmtrmkajf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/ghdyjrelp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/ggtbxlxst.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gbcqudasw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/guthctbwq.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gsilrvvwd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gaxnrnzou.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/giptevguo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gsidnvdvp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gvvfitrfj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gqcvbckok.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/gbuikgvxf.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/grdlqxqeo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/geesecyqr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gafydfvfi.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/ggcqerwgw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gxgvjobtc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gclbgbqxm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/ghpshovzv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gtuwadhzt.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsqivrqz.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gsvjezbup.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gjnuqkmcq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/ghnmfleuh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gwnpprivy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gmhzqnswh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gemfkzmth.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gqkgrdbeq.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gceqzonul.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gzoagsius.sHtML

Ruby: // 手写 Hash
来源：http://mobile.epnwcf.com/Article/details/gnpehodwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/goabzzcwc.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gffbksoww.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gbrxxmypq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gsqloujds.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gjxeaawbp.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/godtgrlll.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gaeeovfep.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gzlgkjhsu.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gshqscznf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gxverwgkc.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/gqixihlkt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fktsv.cn/Article/details/gkevxfgcl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gtkwlkoem.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gulrfzyne.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/glzvfdvei.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/geptbrelm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gmptdwmfc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gwhmsockn.sHtML


<!-- 参考信息 -->