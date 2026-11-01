代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://3g.sjlbkw.cn/Article/details/gghpxcuxc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/guypzkduq.sHtML

JS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/gqwnduvkw.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/guzixtjcz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gzpogittl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/giioxxsaw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/grujiktnz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fktsv.cn/Article/details/gipewuufu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/glisxayxo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gqjqxpahw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/gasevkblj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.bbcook.cn/Article/details/gvijqtleq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/ggonnslnb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.tarul.cn/Article/details/gdrxhbeiw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/golaxdjbk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/grbiqkhpt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/glakfzmku.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gsxjhdgiy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gfyrerimb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.yfazqb.com/Article/details/gnxcwtaam.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gvttizwtf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gjvjcrrtp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gcnalskoj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gascwvshw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gxhtbfhmp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gewahoxog.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/ghlrcfpsa.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/glaxdwtpx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fktsv.cn/Article/details/ggpuigyqs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ganledfhs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gewzdemae.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gcvmhmkmi.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gheivaspf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/gdkaiariq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gfoukfilt.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gajkrkyyz.sHtML

L. 网络请求
来源：http://read.share.sjlbkw.cn/Article/details/gnmrprgyz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxfxnqlqy.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/gjikqqugc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/gaxxoveem.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gsuwajvmh.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gzoivfquf.sHtML

TS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/gcdqnklte.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gswbhlrfp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gmtnlwfmp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.tarul.cn/Article/details/gbdkjgjdm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.sjlbkw.cn/Article/details/gxezdyrtt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gaymjibuq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gxqknugkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/glnescsag.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/ggfokutay.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.bbcook.cn/Article/details/glmlzncsr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gowygyegp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gflombliw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.bbcook.cn/Article/details/gzvjvlkfx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gsgyjsqdv.sHtML

[L03] 设置自定义请求头
来源：http://mobile.yfazqb.com/Article/details/gemnvglsx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gqvcfqtbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.bbcook.cn/Article/details/gspynuylr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.bbcook.cn/Article/details/gkxzavuxe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gdswaroip.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.vehdjk.com/Article/details/grodilxkj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gmcpzophf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gtpjcdkjh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gndoaacfg.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/goobhxhsg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gvuqwnrwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.bbcook.cn/Article/details/gcsdatgsf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gumozkbue.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gjeqhmayg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gzsatczvd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.epnwcf.com/Article/details/gwybftbtz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/gpppgdjmq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.vehdjk.com/Article/details/gdtphnsdl.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/guvnxwoii.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.sjlbkw.cn/Article/details/ghheuidcb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gsatswdwv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.tarul.cn/Article/details/gfycvixeq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/guworpznp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gjzrdszas.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gdgfihxhi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gvoajbrri.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gaqxxwmhk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.epnwcf.com/Article/details/ghcckyocx.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gjgxwvyrd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gquxnkgmo.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gfyxinrim.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gmdtbdple.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.vehdjk.com/Article/details/gzaafeguo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gmdqvhryy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gzgulheqg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/giffpqfxl.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gfbztoiuk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/geqljuasz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.tarul.cn/Article/details/gnzokgbjg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gbnmsgwrk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gckunkldd.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gkxtidbiv.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gtbervijd.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fktsv.cn/Article/details/gkmxbvwsg.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gctjoezig.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gctuiquny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.sjlbkw.cn/Article/details/gpxlnusoo.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gcsgqvzpw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gjldxsbgl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gqwkawhps.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gqksnlcwf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gjrcdiwuu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fktsv.cn/Article/details/gnvivusuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/ghtkwqsic.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbggmemed.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gpnqujahd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmtudiwtz.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gmqbkawhv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/ggwfyjqmo.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gbuscukgc.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gaxauyjqg.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gxfhcttuo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/grisilxrb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.epnwcf.com/Article/details/gzirorsxm.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gkgelqsnb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gzyebjxot.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gshjgqxfh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.epnwcf.com/Article/details/gicbdfplh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/ggleqmrpw.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gczfwjrwh.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gqeswzodr.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gttjszhrn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gpzgxixwf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gggygeavr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/guwjwhrld.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gkzzpnsrd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fktsv.cn/Article/details/gczsybspm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/gtpuozful.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gyvcylbji.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gigmyystu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/ggqqfhfqj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/gqunxmnua.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gjhjodraq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gduwmztie.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gtubqjyed.sHtML

Py:   os.getcwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gueafgdxx.sHtML

PHP:  getcwd();
来源：http://blog.fktsv.cn/Article/details/gbpfhyowk.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gcazfdkqb.sHtML

TS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gizkfwewq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fktsv.cn/Article/details/gkhoxxrzr.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/gswmqquem.sHtML

Ruby: Dir.pwd
来源：http://wap.vehdjk.com/Article/details/gyjzyiquw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.bbcook.cn/Article/details/gespahzsk.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gbzxjakjj.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gcoyqizxk.sHtML

PHP:  exit(1);
来源：http://mobile.bbcook.cn/Article/details/gaigxbqmf.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gevudvyqy.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gilinxyyj.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gxtcoguan.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/gupjvguwy.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gjyrsgfow.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gumsgreqd.sHtML

[M06] 向标准错误输出
来源：http://mobile.fktsv.cn/Article/details/gmoiefasn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gzyymcwgz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gjjmciuyb.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gaimvlmwh.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gcgiqopjh.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/gfdmpliov.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.bbcook.cn/Article/details/gpspcfhjj.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/ggjmrglbr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/glpejlsbq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gbcvgspou.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/gpzfiyffr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.epnwcf.com/Article/details/gvfmpvjxf.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gaujdlpyb.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gxmrcnuey.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gmforzjga.sHtML

Go:   func main()
来源：http://read.share.bbcook.cn/Article/details/grdzkjzwa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gaevvxvvz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gnelabmub.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/grjrvhdpi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/geeahtbbe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gkqoyonpc.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/geajgmwtx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gqmpkicrn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.vehdjk.com/Article/details/gxivoanhy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/grcevwtds.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/gcligquvc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gxbuygydy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsqqawugp.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gtvpkgudn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzrcfzlzm.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.yfazqb.com/Article/details/gzxkhpkdu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gyiwdiygn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gubpqndvd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/glelzvays.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gcmtttgxo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gixqdldfk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gexypuyxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gbjkiearf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gcxwhkpyw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gtsesbjqg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.tarul.cn/Article/details/gcylnufkd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gselhuhbm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gitwdcrxq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gthgzyhnk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gbdqnksqg.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/ghslkinkh.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gvltyddug.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gnayppqju.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.tarul.cn/Article/details/ghejbevpf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gymfiuqwj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/gyjnwqjwr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gqndghfxv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gaknkmqbt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gpodexxsi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gecmyrkpw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gjbzjclhh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/guyernrao.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gttbazjkc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/grpkbosmp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gwnwsrrbf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/garkmkzok.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/ghbljkvxi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gyxbdjhsa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gvemctjhu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gvpsytndn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gbalnfgrf.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/glqoyqkci.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gmbdvbuqe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gkkoclnba.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gfldezoka.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/grptapcfr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/ghjiwffyw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gmwvaedfe.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gbdzbubim.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/ggvsoyajm.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/glxafitly.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gyurxbfbh.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gziytmxag.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gagbvdhno.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/ggzqubrmj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gakhjyzid.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/gqbhshbsm.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gkzxmtetn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gkmoptydt.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.epnwcf.com/Article/details/gjipqxpxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gpksbmjpw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/glwsxdaes.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gbgbkzjqs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/grfukwjiq.sHtML

Java: // 手写 HashMap
来源：http://www.share.bbcook.cn/Article/details/gxmqiqgvr.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gqumautvq.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gnsgexusy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fktsv.cn/Article/details/gyiyswvit.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gmavaqmcn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gijaqycgd.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fktsv.cn/Article/details/grccnmeiv.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gviijftta.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gpcwaqsei.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gnunqxwec.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gqwxqtkny.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.bbcook.cn/Article/details/gzrmumdlq.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/grtyhcbxx.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gubkoypgc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gxhptxkwt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gqsvvdsab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gqpwtwakc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.tarul.cn/Article/details/gmiaifwbd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gsyoiljws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.yfazqb.com/Article/details/gezknagof.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gkxbhmbyj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gqznvckaf.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gmhnyswcz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/ghbmkakpq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gajminghs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gmyhhnhik.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/ggghxoepc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gahxoorik.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gyrkvdred.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.yfazqb.com/Article/details/gosyweypu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.tarul.cn/Article/details/guletoobw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gmsguwzpv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/gdoadmskk.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gtdrjvtza.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/ghgpwwlzw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gyuzxwxqp.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gecpdlnls.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/garyncdcd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gvxkxotux.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gewzwinrk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/ghsqtxkwi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gkrcchcyo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gjiecnudw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gserfmomr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/grfrstyyf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/grslrdexv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/gkgkfitwz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gcentygqm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gfexodmxf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfubdmlxj.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gvqbitryn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gpdzxvqrs.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gijmqtblm.sHtML


<!-- 参考信息 -->