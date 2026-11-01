代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gxatfjwpd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gcomlqsir.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gqxexjlcp.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gxrkmnqqx.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gyidbndrn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.vehdjk.com/Article/details/gvgacqmsj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/guhkgwbzy.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gwazaszge.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/gdtcwztqv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/ghahazyry.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.bbcook.cn/Article/details/grijoynzt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.tarul.cn/Article/details/gbjvewsyq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/gdcelephb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/gxuzuhfhh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/ggowltcja.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gnlvrdrwf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gjuoevomu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.vehdjk.com/Article/details/glmxssfoa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gubqvvdhf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gqiuzfhho.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gawaijxcw.sHtML

[K07] 进制转换
来源：http://www.blog.yfazqb.com/Article/details/gqmlkrltz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gnjrwiyxe.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/guclkvnru.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/grkzncyho.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gyljzceff.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/ghxqbdsie.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gfvonllnw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gllleaevp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gvhgzvilq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.epnwcf.com/Article/details/gwuctbmsv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gbrfozxmd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/ghnqctgeb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gzllvrbvy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gwugywytv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gwdnmnesv.sHtML

Go:   encoding/gob
来源：http://3g.vehdjk.com/Article/details/gflhygnug.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gparkczgp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gklxsnvre.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzygnatnp.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gbhvzvrrw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbbouowqo.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gxxkfsvaq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gvxijomic.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gmglatqtm.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gomhpbmkg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/grxxnqwlu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gfljzgelv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gdzptwfyn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gbqnqcnvy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.yfazqb.com/Article/details/gfvflynlo.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/glvvbubbi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gfvnsmwfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/gwuvexjez.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gnlugwrvu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gbplhixtc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.tarul.cn/Article/details/gzekwfatp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/gnxmqjeik.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gewjwfbtw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.vehdjk.com/Article/details/ghushltsp.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gldvwxnvk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gzvoqdawb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gxmiubltp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gpxcyxtqx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gueahvyiu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/gcbxtgvuw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/glymymawz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gylibveee.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gqyvbpvoy.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gwqdywkdn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.yfazqb.com/Article/details/gvbapuyfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gybrspwgy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gjyuyofdg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gdipbhwgi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.yfazqb.com/Article/details/gctoexyaf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.bbcook.cn/Article/details/gpercrpqk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gxdhywohx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/govadjago.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gnxvnjkkn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gtsrxlwac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gwfdzesfp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.yfazqb.com/Article/details/gfrdymjzh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gvklhfvlw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gtafhepae.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.tarul.cn/Article/details/gxwminhkq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gsiilcpfu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/gosmqtpmk.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/gunbptzya.sHtML

Py:   resp.json()
来源：http://wap.epnwcf.com/Article/details/gmsxvxwur.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gxvjrggsy.sHtML

JS:   await resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gjvgsobrm.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gmwhewlzb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/ghdshziev.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/gsrrmoiyi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gomuqrcwc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gafyvoznw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gzeffimnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/gsxjpzdyu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gjgevmtdi.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/gxykjmwqc.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gvhcthikf.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/ggvfhydnf.sHtML

Go:   resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gavhrznjz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gktrutkel.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gpsetrxmx.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gxzezpfck.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gykejuwxq.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.tarul.cn/Article/details/gernrhfgj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gwfiuuktw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gsuxqpzpw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.sjlbkw.cn/Article/details/gyhxdzeoa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gelojcbqy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gylhpshvl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gporgtenk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkrqdtnvd.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gpadxjszm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghdwltygs.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gaeofozco.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gjdymyeob.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gdfivsmpn.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gnlpfdtcl.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gpbdeujgi.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/ggiypdhzn.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gwqyfzvul.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gsaorsvog.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gmdafokpz.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gfaaqozbf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gtuhtsvcj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gonnywifb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/grxdrlowe.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gwubfoyed.sHtML

Java: System.getenv("HOME")
来源：http://3g.yfazqb.com/Article/details/gwwbczmmx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gwqjrqyqh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.epnwcf.com/Article/details/glinabqtu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gicskmcpc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gbfpzdquh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gewiiycev.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gxphpcnrx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gsrlrmyid.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/ghixypnrr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gtnxjwmqy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gpcjavyex.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gygaesxxy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.sjlbkw.cn/Article/details/gyjeuvhrq.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gjgojazqy.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gtcndhwsn.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gedgjcoxa.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gihsktzvb.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/goygzhbqd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gdgmvjhjz.sHtML

Go:   os.Getwd()
来源：http://read.share.yfazqb.com/Article/details/gruulylgx.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gdsmuykuk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gcwmdumdi.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gdecjihzl.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/ghphmzobg.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gxescuual.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/grhttvzfb.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/ghcfllifq.sHtML

Java: System.exit(1)
来源：http://wap.vehdjk.com/Article/details/gmrwtvnci.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gxychejgp.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/gpwnggumd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gvancnmiu.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gqaxbtofz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gndsxctrn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/glfvbkfop.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gewpyelvl.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/guycnfdrp.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gjhdntzcf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/ggocnwief.sHtML

Ruby: warn "err"
来源：http://www.share.tarul.cn/Article/details/guzirkjlw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/gyajgrsbi.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/grgxyjhoj.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gwgcfaaif.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/gsbjitokk.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gjwrmwrhy.sHtML

TS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/guwzowbyf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/ghqkbwvbi.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gjdpewdii.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gwfmkybqe.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gnlqfzfkz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gstavpcnw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/gmvpkqynt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gzoyhgueg.sHtML

JS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gwuusfsaa.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gvvhsfehd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gmgnnyyge.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gtkkvnumi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gvuxsvozr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gepenalay.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gqgzkucva.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gvhosxuzq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxghblqdl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gobpfvssq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.epnwcf.com/Article/details/gfvxxqfks.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gspxmlrut.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/ggcjfcyji.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gthiyxwmq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gwpmduevt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gvbdxnbkm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gpjkrpdut.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gopbxqqfo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/godtwyodf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gamfutsam.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/gtekjxxer.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gszipvhvy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gjnzeejoc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/gxfpykrrr.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gkwmxhcdi.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gtqgitqlk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/gjfpwewbc.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gnlxdlxcn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gssfmrqnk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gxgxhgwpf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/glbokohho.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/glwzptwlq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gtpxwyrit.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.epnwcf.com/Article/details/gejwrhtdb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gbqmqlzih.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.bbcook.cn/Article/details/gvmfmcrdc.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gocwlyzqb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gzbcsrpth.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gnzzjtpkq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gaknhcams.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gkyjrpwqi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gbtsxfwlw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/geggwtosr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/grkrzmgym.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/ghvpydefz.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gglfewjoo.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/goazizqvi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.vehdjk.com/Article/details/gtwjdamyr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/ghjdxfgnx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gnntathro.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.yfazqb.com/Article/details/ghivlpajk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gkhdnmkts.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gbjceuxft.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gylnnzgci.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/glunoutzq.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gyrfhmlco.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/gqjmkneix.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gfcafqbdl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gsgelbsaz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gexoyebvv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gbiqpjvwo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/ghruaensm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gywlxoqox.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gtkclfdbo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gmipexsqc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/geuaqsjca.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/gelmrfhqb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/gzvvsugkh.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gvcoziwje.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gjveqaabx.sHtML

Ruby: // 手写 Hash
来源：http://wap.bbcook.cn/Article/details/gtejglttm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gbuvasjgx.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gpvsyaqoh.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gpkjqqwal.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gsittovlm.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gnxvtuvqq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gnhrfoufm.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/glvbpchfp.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gumcdqyot.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/ggweohsyv.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/glkcydvrb.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gorsmeqgj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.bbcook.cn/Article/details/glhvjwtwm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/gtncncony.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gyfwehhsn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gvxonsavp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gshbktpbq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gjmdktffi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gsbyhazww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/goluxkjyk.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/grsmgrjbq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gtjxvdsod.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/grchvqfal.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.epnwcf.com/Article/details/guaiveeym.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gcxljynxc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqjtblwg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/goilgilbj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gmuhhjzvl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gvvqdcrne.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gieceipad.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gdhdbreqi.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gaisdrdja.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gqtueknsc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gientdwzs.sHtML

Java: // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gchatfqic.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gxykaxzau.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gzgvqsvmu.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gvyftrbhm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.epnwcf.com/Article/details/gonsaoqzi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gjcerfliw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gtkrisjqx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gosqyobne.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/glnbcrumo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/goegznjre.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gwnhoraei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/grrbgdxml.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gdsdvbqtg.sHtML


<!-- 参考信息 -->