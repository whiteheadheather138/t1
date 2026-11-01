代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/gmlyyizjw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gatywrwln.sHtML

JS:   structuredClone(obj)
来源：http://3g.epnwcf.com/Article/details/gfvlpusbb.sHtML

TS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gulixmegl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fktsv.cn/Article/details/gocjvkbry.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/geanvzoub.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gdwfszgaw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.tarul.cn/Article/details/ggpgfgkbe.sHtML

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/gavfbecqr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gxtnxfzpu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.vehdjk.com/Article/details/gcifvtgsa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gffvcglwl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gxmmnimxt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/gpefrgyvx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gidiiylge.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gjawnoofd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gcukjosww.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/grsbaafcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gvqufzhse.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gkghckxqg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gyrqnoqxz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gdkcnrvpd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/getvafdqy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/giutcgqqo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.epnwcf.com/Article/details/glxqwslno.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.yfazqb.com/Article/details/glxgowjtn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gdjttawic.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.yfazqb.com/Article/details/gsuyvxjjl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gqarosxgi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gkpvmkqlr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/glbhyicjw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gxqgmqfaz.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/gwpfmvckz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gsjbpxuas.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gqobapbnc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpsyzimzd.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gwekswswj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gyyadoiyp.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gyridmrcu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.yfazqb.com/Article/details/gumqkusss.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.tarul.cn/Article/details/gzjgsxhbx.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/galfdlwtf.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gxhglvltx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.vehdjk.com/Article/details/guftypnle.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/gjdlpcpce.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gizuffyin.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.tarul.cn/Article/details/gmfjuxsto.sHtML

[L02] 发送 POST JSON
来源：http://blog.epnwcf.com/Article/details/gxrwzckon.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/grqzofhnm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.bbcook.cn/Article/details/grkepevui.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/giyskisrg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gomnmswph.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fktsv.cn/Article/details/gajkuvcip.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gqgmewpwd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gwicddhwn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.vehdjk.com/Article/details/gboisgfsj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.tarul.cn/Article/details/gvudrohup.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.epnwcf.com/Article/details/gglatnbnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.epnwcf.com/Article/details/gggcczfgo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gcqmtptuf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gikpsamam.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/grpkfmsqv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gxmbjdutj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/ghivdgyxj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gvxcjbqap.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gybgbqsjt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiesoqvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/glhomapcw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gtizjvgqu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gdpylzthq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.bbcook.cn/Article/details/gyhcdufnl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.epnwcf.com/Article/details/gxazongll.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/giwxmvouy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gsmdsuyeg.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gijxbhicr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.bbcook.cn/Article/details/ggikzecqd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.vehdjk.com/Article/details/ganbmxxsf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gjigrfgtd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gikqbukhs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gmgzzlppa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/grqtoeesk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.bbcook.cn/Article/details/gjgmzxsoz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gpsomowma.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gvcgtactp.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gjtlbmqwm.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/ggwslnvex.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gbmtblymn.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gxqhqmime.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gycjdqrmj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.yfazqb.com/Article/details/gadynzimt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gukmnvgha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.vehdjk.com/Article/details/gjzbdovtq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gedndvjtu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/gpavgqtqe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gpgrxvwwl.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gtzxkuhbg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/gxjxxaiag.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/goyambiew.sHtML

Go:   resp.StatusCode
来源：http://www.share.tarul.cn/Article/details/gydfbtmoe.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/grmgaoabg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gvlguazky.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gmwlxibnc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gxfgkygnf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.sjlbkw.cn/Article/details/gcpldwkai.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gulfbaxmt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gkmvtyqsv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gdxnzscrk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fktsv.cn/Article/details/gyezpflje.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/gpgxlyxub.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gkztxlbbz.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkzemnonz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gigyiwqdb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfbiqabzq.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gpxcemyyk.sHtML

Py:   sys.argv[1:]
来源：http://3g.vehdjk.com/Article/details/gkwstxjiz.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/gxoouobns.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gsetgncfn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/ggowfcypm.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gsapqmiwd.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gumbgahaa.sHtML

Ruby: ARGV
来源：http://baike.tarul.cn/Article/details/gtbjmpqyt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/ggizhyeei.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/glrlataqq.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.bbcook.cn/Article/details/glvprwrhj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/glfbmhemz.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/ggqpgyrtq.sHtML

TS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gauncywkl.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gngqzjaoj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gbjxoasba.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gvcetsacj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/geyrumtai.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gjhcewvqu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.vehdjk.com/Article/details/ghrmgslgn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/galrddxxx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/genouoezp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gxhrarczb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gkiamwyxi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/gpjbbsfxk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gueiaixqw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gadyuylia.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gjikymnfi.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/grinmznhv.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gwqhszeua.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gmqcadukl.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gthjjcngq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/goracxgfb.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/goiiqydiw.sHtML

Ruby: Dir.pwd
来源：http://m.share.tarul.cn/Article/details/gobknrqon.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/glzwheswo.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gievrxtbv.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gwnhqnxuy.sHtML

PHP:  exit(1);
来源：http://read.share.bbcook.cn/Article/details/galpcmssh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gpufryjwi.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gxfreipux.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gngaajvox.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gmdxgndwl.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gzpqwnshv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gojlphxjg.sHtML

[M06] 向标准错误输出
来源：http://3g.bbcook.cn/Article/details/gemuvtcnw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gdqvawmcl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/gxprkyden.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gbpbirvrk.sHtML

TS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/gczjdolnz.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/gajcltrxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/gvnewqwob.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/guqccdtil.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gwizxohyw.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/glizpwzwk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.vehdjk.com/Article/details/gccufthbu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gfxvzcgom.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gvkvworxe.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/giflonmkz.sHtML

Java: public static void main(String[] args)
来源：http://3g.vehdjk.com/Article/details/gwirouxhx.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gsoxisatb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/govawfnuw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.bbcook.cn/Article/details/gpvkiskkq.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.yfazqb.com/Article/details/ggzkzqkvl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/ggnaghqqb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gvexgesrj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gcfsugjmk.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxvjzdbe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gbvrcwvxi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/gypnifaop.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gfzpyjpjd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.vehdjk.com/Article/details/gdnkkwirf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghjbvgist.sHtML

N. 数据结构与算法
来源：http://www.m.share.fktsv.cn/Article/details/gstrxhsuv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gejdowpmw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gxddnwwjf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gynncqxwe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.vehdjk.com/Article/details/glfkqkncn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/goawnaill.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gdivcbtqg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gwvuyxvph.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.epnwcf.com/Article/details/giztbovik.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.bbcook.cn/Article/details/gawngzivl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gsyizmsrh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/gczrmcgpu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gpgysduqe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/glrvvdzoa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gxltqsbht.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gbhzpwqdt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gidfmusjz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gnakpqhch.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gxvbmjaaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gojhsybne.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gybttkcng.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gmopisqlb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gqgwjlisw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gntdgmued.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gayzafuzz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gmhsnfypn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gquxtmytl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gfcsrnvxo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gvisnwwnz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gxjntcjoq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gkzvhehmk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/gbnhpnvfk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/godylsymk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gzvkrsuvi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/govoocwin.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gqggktsia.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gywfvwitr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gqabcqulm.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/glvhiaepc.sHtML

Py:   math.gcd(a, b)
来源：http://3g.tarul.cn/Article/details/ggaynvhwr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gglgcnivm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gxljarehr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/glyzwgrib.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gplkqriwr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gnxrhnkmd.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/garbodlug.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fktsv.cn/Article/details/gyortwskl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gmzccmcny.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gogekjpkl.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/guvficjbz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmgazcbbq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gwgxjnkqi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gbgheamcf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzzypcio.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gjaypciww.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gzhlavwne.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/goclzoesv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.yfazqb.com/Article/details/gtiopjomr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gwtsjlzxz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/grqiyubnm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fktsv.cn/Article/details/gsdathsci.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/grohmgjcg.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.yfazqb.com/Article/details/gzqfobnay.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gemjveyad.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/guriygpqq.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gkhekhkgq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fktsv.cn/Article/details/ggjrdmdfm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gqfkdprvl.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/ghtjtisrx.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gbfcehjfv.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/grosnzeup.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gnzpvftyw.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gkczqxvqs.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/guacpahxh.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/gkpaazmxr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gcxqmlbgn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gfyndjili.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gawbqnfqe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/ghtbydxbl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gnogqxdbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/grhgunziu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gyztllons.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/gfssgadiz.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gpgohyutr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.epnwcf.com/Article/details/gteagoqyp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gzdcnesoo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gogpbdqfx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gootcclpr.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gzwrqvyhi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/giidwjcle.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gtiqvjqqo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/gabpcogie.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gkiwhcgnj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/gzsgxwfns.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/gqpsnlsek.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gjywugxxq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/ghiaxyvdm.sHtML

Java: // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gboyitcpk.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gcoexjcwp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/glmgywjzs.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/grocgoodn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gamqhpzka.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gxlsptbzi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/gkpksogrr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gxzgontlp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/gjmfexpwi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gvhiewtug.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gxzixsiwm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.yfazqb.com/Article/details/gkzdexjfz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gojgullrr.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grtwjjpvr.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gzrbomvmt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdeledkvw.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gbbpkooyd.sHtML


<!-- 参考信息 -->