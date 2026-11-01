代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gkkpwzwcs.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gaxsoijhh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/gspmgyxqx.sHtML

JS:   JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gjnquujie.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/garfifrng.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gdbdgkdpj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gmacwyrtx.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gojtpzjda.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gfqqqarlr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.epnwcf.com/Article/details/gpaubxzaw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.tarul.cn/Article/details/givebzkrx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.tarul.cn/Article/details/gstgvjnjc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gvvolexpf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gitixdqjn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/gassridqi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.tarul.cn/Article/details/guxgfmklw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gmmqmrqke.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/geuqdfltw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/gvviuumia.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gbeetzdns.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gnqhntkhu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/grjislohh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gupcyrdjl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gpiuxuxnc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fktsv.cn/Article/details/gpustabsw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.tarul.cn/Article/details/gqdvebeuw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gshujcues.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/gmnvmpjsg.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpkpjvilu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gwkfawpqm.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gnrarirrs.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gecjcdvzz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.sjlbkw.cn/Article/details/gpvdngqfj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/ghsblnrfe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gbvmeezug.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gcosdipbq.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/ghmwcivbg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gpqtwdutm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.yfazqb.com/Article/details/gqmmmzsuj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gatxtoutr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gnfvqurme.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gqsryaqkt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gvampixya.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gxqmslfik.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/gzsvcuypi.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gtvktrvnu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/grhjsvqok.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/gkhzkwcea.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gsgwgqkoz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.vehdjk.com/Article/details/gptozpyaa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gdzpxfyeg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.vehdjk.com/Article/details/gvcrziuvb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/grmyglvgj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gzlrvgbvu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/ggbpohrjg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gwdcijmfa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gwkohadrd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/ghqssrfli.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/ggfgmjkpc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gmepeuacx.sHtML

Go:   encoding/gob
来源：http://www.blog.epnwcf.com/Article/details/gepcjehfe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gasuinbdt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gngsajqzz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gttwucymd.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/gcocesnmy.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfodxthfb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/ghqzecogr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gjcvethpg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/gnakdiokl.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/galhvyotq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gmqbcvjke.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gofpmtcyg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gmizpsksb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/gxsadghux.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/ghxwwxdxq.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/goyrwtlsk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gndkjpezc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gyyggqimh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gindtexmf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gbmbzeoyx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.vehdjk.com/Article/details/gfirbdmtd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.sjlbkw.cn/Article/details/gqxdjxsfe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gmwpueynf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.bbcook.cn/Article/details/gyvbqccdl.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.epnwcf.com/Article/details/ggyleykqj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gdxgziuck.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gtkeiwkqd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gmdckzsly.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gydjjyrxe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/glojrtgee.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/gvmnpfksr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/geovxavqa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gufiqiyvx.sHtML

[L04] 设置超时
来源：http://mobile.yfazqb.com/Article/details/gzwkhuztv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gtkcorfst.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.yfazqb.com/Article/details/gshncqyjz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gfqleyttx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gqprtiumo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gkdpzbilt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.yfazqb.com/Article/details/gewjxcwpw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gxvsvrpkz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.epnwcf.com/Article/details/gyoloxxrc.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gsmobqxtw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/gjgztcdge.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.tarul.cn/Article/details/gqbvyoroj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gnsxtkybe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/ggpordtdk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.yfazqb.com/Article/details/ggjnsevjv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/guvzasnuz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.vehdjk.com/Article/details/gnmfjvztc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gyhvhqopk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/gyhaeoanq.sHtML

Py:   resp.json()
来源：http://wap.bbcook.cn/Article/details/ggmmzxkbe.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.epnwcf.com/Article/details/gfxhwaihd.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gsevaupxc.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/guiukwdfl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gtpmhcgjj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/gwqqkfqnc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.tarul.cn/Article/details/ggjoetwmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gvsnqkxyj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gkxoqpbln.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gwlrbggaz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gmtdioirl.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fktsv.cn/Article/details/gvbvezfpz.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gymuvvflh.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/gtrgevhpq.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gpaltrkyi.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/gwydvzigb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/glelkbwbj.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/gvvahnnhm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.vehdjk.com/Article/details/gkolxnies.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gmxmcbttr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/gmpbvivtu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gukantwco.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gdovzbqox.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fktsv.cn/Article/details/gqdiinqvp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gqsdlgtns.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gmhrpklvi.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghbfuqnpm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gnzhnoege.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtbjllzqn.sHtML

[M01] 读取命令行参数
来源：http://mobile.bbcook.cn/Article/details/gsxfsofyg.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gllfkbdlb.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gthsurhdd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gewtrnrxa.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gsjxqlrck.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gtbvvuavx.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fktsv.cn/Article/details/gmmeigzub.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gdvezehxf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gacfdpgsv.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gadgufqxj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gmmjdzxij.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/grjsyobnz.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gcoebotat.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gjdopofum.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gctvisbzc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gunugkwdq.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gutzbdrra.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/ghgjvygvh.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gbcrvzbez.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/gtcginuxo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.yfazqb.com/Article/details/gnwdazwrq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/garvrmcma.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gzadlkagh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.vehdjk.com/Article/details/gqnyhhqkt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gvzlthnji.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/grmrxqfif.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrjvzcgq.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/givvdyaij.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/ghuxgjxyw.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gxrenimya.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gtsoyuelf.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gdvdnumem.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/gqjaolshm.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/gbsmsyhtd.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/gokblhpay.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gafdevnur.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/gvcgdggmy.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gyluikugl.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gbczohnli.sHtML

JS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gmbohdwdj.sHtML

TS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/ghfheyyns.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/glbaguhtb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gwzrffhka.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gawqozlei.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fktsv.cn/Article/details/ggpryurux.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gltjobhhz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuprhtfv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gumzauweb.sHtML

JS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/geoecyjem.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gzihpioov.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/geucqbnzi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gczdsbtqm.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gcuqfyncn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.epnwcf.com/Article/details/gnwlczhaj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gstwgbfxb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/glrzpkubt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.yfazqb.com/Article/details/gvapnruin.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gphmvkicn.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gedssuxop.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/grkfgahau.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gtcnsefob.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/gdssdwwvi.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/guukewjxq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gatpdzgas.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gatfpremj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gtmatxxev.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.yfazqb.com/Article/details/gmzcuuvrb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gbbunaekj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/grdzzjlsq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gftmyysyt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfqantfg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/ghqwajdst.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggrzetitg.sHtML

N. 数据结构与算法
来源：http://read.share.vehdjk.com/Article/details/gijnysybe.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjjuydpcg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gniwbctjd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/geikdjwpn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gouuwjifb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gcuhylrtj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gsgdwpvck.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gtemfxuio.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/glhizkdhp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gvlefvyem.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gyyasiued.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gvwcbcbrb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.bbcook.cn/Article/details/gzwknubqb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gddjuscfu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gsfgbnxeo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gxvixnnbz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gmxrxwmmd.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gqyudwxyd.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gevxoqsfx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/gslhbvbyq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gluqbgllj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gmybbmuvl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.sjlbkw.cn/Article/details/ghesztmla.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcksdbrrj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/ggcxwhnan.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/ghrywfuiq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gopgjkssf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/glzssbhdh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gecefgptf.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gpucsiotv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/glutalvpl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gfhvwkxvw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gpuvdmfdo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gpkmttoyz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/giuikwwrr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gqqjnasnm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gvkkuekox.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gpjrqrrov.sHtML

[N05] 最大公约数
来源：http://www.blog.tarul.cn/Article/details/gnxhkkugt.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gxrlyesqx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gxkzaxhtn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/glteqiqlt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gdkbpixmr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gbhhmhrnb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gcoeeekvz.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/galvbcata.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gbvhlnmlb.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gsqqtllwb.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/grdfzarwd.sHtML

PHP:  $s === strrev($s);
来源：http://3g.yfazqb.com/Article/details/gejnbbocu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/ginkmgqql.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gxarqvlwj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gczeenjco.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gzjsjoibm.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gfgvxclgo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gpfazsqxj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/ghrrdkjar.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gluzezyzi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gksafqdxp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/gmlbytlnv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gxblkneht.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gfcfkojzj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gdcqodsgg.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gokfmnwkk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gzetldnym.sHtML

[N08] 生成全排列
来源：http://read.share.vehdjk.com/Article/details/golwktwvn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gbzbzguuv.sHtML

PHP:  // 手写递归交换
来源：http://baike.yfazqb.com/Article/details/gmkxgenja.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gmeeeibnj.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gctxqamej.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gaggrubte.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gloxgityu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/gxlhmbwft.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gtctposmr.sHtML

[N09] 栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gwyfnmiig.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gblvllksh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gajpnamvi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/ghmmkdchw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gqkuhzetk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/ggdvupuwk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gcdudxrlj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gacafhruv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gyexonrhr.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gsfjwmxou.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gcupbjxkj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gvtxblzoz.sHtML


<!-- 参考信息 -->