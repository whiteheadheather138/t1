代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.vehdjk.com/Article/details/gxzzjdnth.sHtML

Go:   json.Marshal(obj)
来源：http://3g.yfazqb.com/Article/details/glmmhfduf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fktsv.cn/Article/details/ghmegruek.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gvvchjehk.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/gfvgsobsp.sHtML

Py:   json.loads(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwdtulbfj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.tarul.cn/Article/details/giyauygqr.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjqqzdxhk.sHtML

TS:   JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gfuoixzli.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gfmwstmip.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.vehdjk.com/Article/details/ghzmiydfw.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gozhiskfn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gynuxwssn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.yfazqb.com/Article/details/geogmespk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gwvhhzowf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gclgoavah.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gjhunenlb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gnrqyourw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fktsv.cn/Article/details/gziiubptq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gtxvtidmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/gluiittvo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.yfazqb.com/Article/details/ghrffnlbq.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gaiavrnnh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gtagrtnyq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gnevsrmvm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gntpuegqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gznjsawyp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gwfoxtjay.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gagpnbbfx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gbstmimag.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gspbmnbzp.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/gwhabhccw.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gmhcfedjs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gnmnqedhk.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gzkedzwma.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/ghullgbdo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gngeqftaf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.tarul.cn/Article/details/gjtrhwfxg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/gmfedsvtg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/gshdbcrdo.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/geojmattn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gpkvalybl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gcjbwnswi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gdqtfrqgr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gsaiwxiaj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/grzlzrbgh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gmlyeafgq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gtetoidpr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gppjlwcyr.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gntpxawsj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gzourotft.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gprnftydu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/grliocsfw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gmodmfnuy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gkqaxvyfh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.tarul.cn/Article/details/gmyjmikrw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/gmjpzxwzn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/glltvducw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gztikxpzr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/geelooihk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/gbkgapjyi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gnwuwtift.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gilicxhud.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.vehdjk.com/Article/details/glknuuasm.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gmzscwikn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gyknizpcv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gheejrgzr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glapwfubd.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/grwsstsmm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grmtztyjf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gnivfeabk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.yfazqb.com/Article/details/gtkbdlqgd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.vehdjk.com/Article/details/gzwdaetry.sHtML

JS:   await fetch(url)
来源：http://www.blog.bbcook.cn/Article/details/gssgqogbe.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gmufhczmy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gbcqwgtbn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/grwvydhgg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.bbcook.cn/Article/details/gqrflajie.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gccxqyqte.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gqvtgrhgc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/glpqlzyei.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.yfazqb.com/Article/details/gjigkjmsc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/grlmqfcho.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gcxrizjfd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fktsv.cn/Article/details/gjobhpnzg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/ggapndsvi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gwkppzixk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/guwrvipat.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gcryjzzqn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/ghclnozpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.sjlbkw.cn/Article/details/gizssszxl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/gmciunvto.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gpjqmihfw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.epnwcf.com/Article/details/gwxgfzckd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/grlckdisc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gbrzrxzlx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gxlpcwcuo.sHtML

[L04] 设置超时
来源：http://wap.vehdjk.com/Article/details/gtgtjbmql.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fktsv.cn/Article/details/gzfdciqgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.yfazqb.com/Article/details/gjqmawfml.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/glhnjqmqk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gdsdifxqm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gxtmerxts.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gqwsisyuc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.epnwcf.com/Article/details/gfmlfasbw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.epnwcf.com/Article/details/gnaojvbke.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.sjlbkw.cn/Article/details/gcrblvvcx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/gbiogaqgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnzkihrv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gknhzcdzt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/gtncznrrc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/gdgwxslff.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gxqejnfaw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gzawwqxqr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fktsv.cn/Article/details/gbldaporw.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/glamntktp.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/gjeheiltu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gyuugstdd.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gmuwaezbx.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gfbxfzvrg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gusvmwrio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.bbcook.cn/Article/details/gdcqukspk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gehsrdykw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gspfjbrpu.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gdldfwioq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gbinnrqio.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/ggmyfcupf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gacsyptgk.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/guhpjaibj.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gbxpcboxz.sHtML

Go:   resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/ghxgrthzw.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/grtnrwugu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gcezgcyis.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/gsxhdblez.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gzlsjmaez.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/gtnigbqpm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gprftzirk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gqodvegzm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gplokrqew.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/guxcvgubt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gafjtbeyl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gbxoopwwi.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpuynekga.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gkpuvfzhl.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/guxfkcijq.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gcjrcwlab.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gmhtfwrre.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gcrjvsjmh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/gqhdtxdyx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gvvvqtnve.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gfebhstfk.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gzadypyxf.sHtML

Ruby: ARGV
来源：http://m.share.tarul.cn/Article/details/gadcvtszx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gahrykojw.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/grhilzcet.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gybqhtcgc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gbtmwxxha.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gkoqlnjam.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gusfrjhhu.sHtML

Java: System.getenv("HOME")
来源：http://blog.tarul.cn/Article/details/gzxlncjpz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gsvkzwedc.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/gnezdznqz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/glkujyvmt.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gzuczsrlw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/glnsusmdq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gwoxxfhyu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gkcfhkkju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gciqzzppt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gbkbxfcpj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/gvshlmnqu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gtjjtznza.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/grvbqsbbu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gwyicfhnh.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/gwtcmmyfv.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/gpkcjkrxj.sHtML

JS:   process.cwd()
来源：http://m.share.bbcook.cn/Article/details/gxgddgqdl.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gokkajnyt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/ggidakqie.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gapltismg.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/gfbkutjbx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gyecrweib.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gqhooolrx.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gonidqcky.sHtML

PHP:  exit(1);
来源：http://read.share.fktsv.cn/Article/details/gtzsqjkkn.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtuinnrpa.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/guzoukjjf.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gwbukvpum.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/glvpgjrqk.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/ghzlghvrl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/gebszlrmd.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/grcwssodx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/ghdbqxnlq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gezixlbqi.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gvyubxxte.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/glrsoqqbv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gulsbbsvk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gtawosrmn.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gfwrynktk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gpzthwlqv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.vehdjk.com/Article/details/gyphqmzbc.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/gutspqinf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gndfjjvyc.sHtML

JS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gwiqfsayn.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gnfslsvoe.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/ghmrylfzx.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gjdftnwgz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gjiiowggw.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gtvwkevss.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gyayduydh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gxgprxmlj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/grftkczfy.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gmxcarwig.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/ghqxplalr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/gkzfceepe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gvgzahbuy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/govdmqzqh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/ghisjeroq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gklrfatlf.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gyysletze.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/goiokynac.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gfvngpsma.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gyyusikcn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gepbqvupw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gxyqfrkef.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gnzlqlkxx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gznuybbul.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gjhabyjus.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/goqhblcfa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gtvstcatz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/grvpsuvoj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gibwvskbz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gxwemslsx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gxpsltfhj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/gffkehnpd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gzyzkshcb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/ggzwhkgcb.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gjqacziap.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gfrrvjuis.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gnfyaprpy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fktsv.cn/Article/details/gvmthrbpo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gajjvhuex.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gvndfnrcs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/guxyklsbt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gjblbmbhf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.vehdjk.com/Article/details/gvjnggobn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/grhigdixo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gbakddyym.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gncrlargl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gdmrrimdn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gzpuvckqa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/ggrjiuqpr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gavpgxtdh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gfpwzrluf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/ghtpzrnwe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gqxzmgkhv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gkjaueoln.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gcgunhccl.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gcvtwwqav.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gmcpjvhkq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/geacjgvaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gubkuvedz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gxujipign.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gbbbjuizq.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gzhbsykbc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.epnwcf.com/Article/details/gapsabsrg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gtcaodjvy.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/gfiryccvo.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gjcllhcob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gwdqkglxn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gsrnsfmik.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/geqcjiedj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/gkcxszhqd.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gvicchtap.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gepkifogv.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.epnwcf.com/Article/details/gxlbzpowy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.epnwcf.com/Article/details/gshghwdjk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fktsv.cn/Article/details/glitvblax.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gsgkzgvpb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gjkxffceu.sHtML

Java: // 手写 HashMap
来源：http://wap.epnwcf.com/Article/details/gwrmrcbfw.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gvfeykhfn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gmwwvflno.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gpvidzvck.sHtML

[N08] 生成全排列
来源：http://www.blog.sjlbkw.cn/Article/details/ggkcjzgbh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gtexwtvyv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gdsdpkjku.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxtguehlb.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gewvamzhi.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gmqchjqih.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gxrntwgjd.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gkiumwwke.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/ghaoxiomr.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gqhoewzcc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gtotcwvgh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gtexxkzcx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gyirzjstq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gmaylttpz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gjabshjwi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gkcugdgxu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/grysbsbxj.sHtML


<!-- 参考信息 -->