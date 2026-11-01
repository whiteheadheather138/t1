代发 wailian999

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/grutabxgy.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/gafzwmyud.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.yfazqb.com/Article/details/gutdwugrc.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fktsv.cn/Article/details/gxifjpodg.sHtML

TS:   JSON.parse(s)
来源：http://wap.sjlbkw.cn/Article/details/gyogkjcfj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gqonpgopk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gasghmnbt.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gifoeiakv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.yfazqb.com/Article/details/gdcufnaxq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gccerduud.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.vehdjk.com/Article/details/gcyetxkjo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.epnwcf.com/Article/details/gflhuxaab.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gdhqbmwrl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gdwubetkm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/gvhshfyud.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gyozjkpwn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/grvpjrenv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gjzkmjqju.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gdajxiwzk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.bbcook.cn/Article/details/gfhvvvkhw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gzsgtgcqi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gofojnanb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gewrpdnhu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gxlrceyzs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gohtqyaxp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.vehdjk.com/Article/details/gkvjzlbtm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gouyykaax.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gednrsffd.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gvsvniidk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gceumpycb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/geetctdyq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gbvwlqwsx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gescxvlym.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gguouesck.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fktsv.cn/Article/details/gklnbtemn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/glmdemexp.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gshbvdtgt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gkbsvliii.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.epnwcf.com/Article/details/gwmstjzjv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gnatszcoq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gbrliwpoe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gscamcoqe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gthvurxcn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/geatlmkag.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gbhrfdcqr.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gblptvbze.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gwgsoxolt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.sjlbkw.cn/Article/details/gqzfxntpv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gxnflatvx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/ghmnesuiu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gvbhqdgdi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gzsahouwz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gjxnbpilk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gfxhxpqka.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gnwxewlvv.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.bbcook.cn/Article/details/guuykaqqh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/gauxmftjx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.tarul.cn/Article/details/gfwpevzei.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gtqwfnayz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gwkrtghsi.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gjwgpzbcw.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fktsv.cn/Article/details/gthcervny.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gbwoharyo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwcsnztmq.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/ghobywfvn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gxggnzjsj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gmomcengw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/gldiyzlkv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gvmekvapg.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gjauirjxy.sHtML

TS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gokviuodm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gkmqtohue.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gozfgrcua.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gqsdtdria.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/glmnbathf.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gqcuahmcl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gniwnvway.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/gqxykhspk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fktsv.cn/Article/details/gdxwazazs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/guiwzynrm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.sjlbkw.cn/Article/details/gbjvdybbo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.bbcook.cn/Article/details/gnrckghma.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gxquhjujw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gyqdbvdsa.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/grvflfbie.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.epnwcf.com/Article/details/gcgogxszk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/ghvavfsbl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gmbolqqtr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/ghotdhxoj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gcyguasgk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gkzcvzeig.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gkmzkigsi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gypyephky.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gonhestnw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/ggskiergl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gbveqcvcc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gthipdytz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gzdezwcue.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/ghjesqnca.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/geosdvuvz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwljehdmd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gbowcgwgl.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gsobtmmye.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.sjlbkw.cn/Article/details/gozovmvbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/glermnetk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gigjjqvxq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/guxbfhbpt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/gjyhxfkzy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gyrsgiozt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gqytbddot.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gveigttks.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gyzajijlq.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gzqjvwswt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.bbcook.cn/Article/details/gvmepnxuv.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gdkemynvb.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/grybqpgps.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/gwadsufya.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/ggljzaxrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/guixwzvrw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/gpsirbjxj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/genyhagkq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gnqazwrbr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.yfazqb.com/Article/details/gnlebyktl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gsdwrxzjo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/grsiyrvqn.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gursuyvha.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/grxiuxyvu.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gmtlgaxvk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gnbzoldkc.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gvdkfynvp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gkknithcg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.sjlbkw.cn/Article/details/gafjutnmc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gcmjawqzh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gqvkphvdm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/gxxlkpuru.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gksfeegep.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gcyeflvck.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gfguekvah.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkbbzdzau.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/gpykwucii.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfhggyfmp.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gbpgzubjz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gatbzqywf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.epnwcf.com/Article/details/gxirdoypv.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gwudinark.sHtML

TS:   process.argv.slice(2)
来源：http://baike.yfazqb.com/Article/details/gwrdqdhtf.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gahbnpsiv.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gtwaxltcs.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/grjsjcfwh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gqnhdivqb.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/geezaotow.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gciqxsupz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gykijrilz.sHtML

JS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/guiydkixw.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gdhaxlrmy.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gtctaolik.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fktsv.cn/Article/details/gbpylggmx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.tarul.cn/Article/details/gmdxyqqyq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gdwbcsrlx.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gfewdvlfx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/grkxbksen.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.tarul.cn/Article/details/guyrlkkvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gvfzxchrd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgoydptp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/giznqyxtb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/grmptwsgq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gptojyxyc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.bbcook.cn/Article/details/gmsoesnal.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gbskkdcpn.sHtML

Py:   os.getcwd()
来源：http://wap.sjlbkw.cn/Article/details/gvkcgjxcj.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gboactngd.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gxgvpuzjd.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gdykzfgtv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.yfazqb.com/Article/details/gguacbecb.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gipsdtbjn.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/gziviwpmy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/gxhbkkegu.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gkbogdktr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/grtoppzcv.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/ggmweygad.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/godmpjztr.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gfgilsrrt.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gqtraeeub.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gbazbpoke.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gnmoilkuh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/ggepextrc.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gydlqipqx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gevbcaxur.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gjhwwoipe.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/ghnxssbje.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gsfquuvva.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gimncyuop.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gbolaxhpr.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gmhrskfmo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.tarul.cn/Article/details/genrkmhkr.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gzvhkudyd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gakdddnui.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gbhdfigfx.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gjyfubgiw.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gdeknbhjn.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gtizbrsmt.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gkknmhtxp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gfpqzjaxe.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gyscpdkgd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/gbbswjotd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gnsenwnrz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.epnwcf.com/Article/details/gurcospuz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gzohiznst.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/giqjmbyju.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.tarul.cn/Article/details/gbtqtejch.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gxucjbers.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gznyhdrpi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gzeyopfxc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxuyyqcnl.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/glkgbjsnz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggwvojcbk.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/ggujappwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gzoqayufj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gxjypgeql.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gqysmclpl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/ghuqnbmob.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gekivwtvw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gsgctjjvv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gajodqtxo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gqdwhpojv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gyoitztge.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gpkhzfilr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gmthxghzx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gunxfznry.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gxoqhcsdw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gezlbypbq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/gobshnbgf.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gunhtpaan.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gjbfdjvpy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gyfbwprtl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gyuhwgsws.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gvdhwnafm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gyhsqkabj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/ggtfejqsu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gvnrsiegn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gkavqgnpu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gkpyqxwbr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/glyalxrou.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gcpmnhibt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/guakplazh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gpedsmtui.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ghsvrcgvs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gfnzljehe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnemqbps.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gmyojzugv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gskhrcbvb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/goxftnsku.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhkypkby.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gsshwffou.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/giwgieaby.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/ggaotnexs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gpundqmho.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gpehdtsyj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gvwdtrycu.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gsqtumrvz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gximsdokw.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gfyiqujgv.sHtML

Py:   s == s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gfjlbosxq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gfdlefado.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gnvvajpcd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gmvdtbqpx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gcasxawoy.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/guyitrpjz.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/grceowuag.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/grpmhmegr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gkggmeapd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gpyfrhtkm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gzbxqdoiw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/glpsmorms.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gorfsfykx.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/glyyfvvtx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gwomlwfod.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/guucxbhdt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/giyqdyche.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gfxieigdw.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/goifrilmk.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/ggvqmnpih.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gghtrefme.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gpxbceppf.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/ghmmvdhrg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gyrvqolmn.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gjxgsuzyz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gsdesmagw.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gueibkxnj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/gptmixjyv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gcvduqeij.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gsgcbsqby.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gdqfiemnj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gqgwnalbq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/ghchnnmdy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gqjfpzlnw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gwwcyigsx.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/goudjrbqp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/ggvozwmft.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.bbcook.cn/Article/details/glkhabvpv.sHtML


<!-- 参考信息 -->