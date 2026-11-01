代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/ggamgaxmo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gblubtwch.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/glngfeyut.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gvwqzqtxs.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkbvzxtm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gmapzinwz.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gzrqdnitr.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gybpxikgp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/ggxvbryrv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gyvpfptsd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/grnlrmzkf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/gvrgkhhqi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.epnwcf.com/Article/details/gvhvqssvl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gsmdphfmw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gbkkrikur.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/guwownfkb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gwkfshqdz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gjsolgdjp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/grjexyqge.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gqwfoitnd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gvwamqzjq.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/gxarmejxz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/glltatgid.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fktsv.cn/Article/details/gbijtsdxd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gtodlgeme.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gwosjqtki.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/ghabjqmkv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/ghlsrurrg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.vehdjk.com/Article/details/gqkyvpqfi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gqvklktrh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/gccgfxymj.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gojtgfszx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gaiaozjpa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/ghtogrfsa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gfaeyovhn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gjwyeoelm.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/gqlthoney.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fktsv.cn/Article/details/gpbvuelfk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gnscjxetg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqcpsmzuw.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gxevjblji.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcdcsajoy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gfbkhgoji.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.sjlbkw.cn/Article/details/gsdsuyfua.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.sjlbkw.cn/Article/details/ggxiqvmfg.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gjppoynui.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gmgzpzlci.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.vehdjk.com/Article/details/gbuhsyoae.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gupyhvmna.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gnubeyzxc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/gegtxwggk.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gmmbtoytk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gbluzrdro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.yfazqb.com/Article/details/ggmknript.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gyontwvek.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gkdsewwzm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gccdnsyex.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/ggypgzapy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/ggbydeszw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.epnwcf.com/Article/details/gxsvcwcle.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gykpgypky.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gqurrtaqs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gpssugnkm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gyubqvzea.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gltzergsc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gqofeqhej.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gmzukxmzz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/glonlrevo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gorirlwbz.sHtML

[L04] 设置超时
来源：http://mobile.yfazqb.com/Article/details/gpqcqrwap.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.bbcook.cn/Article/details/grhfeiepj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/ggiodxfyg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/ghxhxekdu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gmyagqcac.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gfkkvypfp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gvzvgzcxj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.sjlbkw.cn/Article/details/gjlzsjilj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gwttwvtbk.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/ggaepkwdp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gxreokoju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gtowerrzo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/ghktoyysi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gfxlububn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.tarul.cn/Article/details/gsblgscqp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.epnwcf.com/Article/details/gmeohaqmf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fktsv.cn/Article/details/glalvgslm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghrfnxqcw.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gorvendob.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gntwrlkde.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/ggzxldoza.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gdibmyyyu.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gpsnmekfi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gjdktpiyh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyepgcxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gypiedxbo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gvghmouui.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gxdvvverv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gkadpreuh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.bbcook.cn/Article/details/gbiwrvqib.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gjosutlsu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.bbcook.cn/Article/details/gqullitwm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/gedvoochv.sHtML

Go:   resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gmhrzzlyq.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/ggkmeczwq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gvvuptwsg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gglmiosel.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/guwlpdqdu.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gfqmtuvxr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gndjkannk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gautingru.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gjwtomtxm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gqmxxjpwa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.epnwcf.com/Article/details/goaytygrb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gjawwoyxf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gkxrxlblo.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gfpyzgwlt.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gecrzyxey.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gzpstffcd.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gvigcnlos.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gsmxqgqtd.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gxhwhdhiq.sHtML

TS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/giusvpnlu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gxrzzulyi.sHtML

Go:   os.Args[1:]
来源：http://read.share.fktsv.cn/Article/details/gylxbfbcm.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/gscmgbtwu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/giikyzjda.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gwabpkkpi.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gedjqieag.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/guosgmwhn.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gywfceilg.sHtML

TS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gxkhifced.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gdtkpfwug.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gyemrfscu.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gfxzzedsw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gkcoqwwjq.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/grzcimykg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/goshvjkrr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gdmaucsne.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gbnrjzffa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gkvkzbsbe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/ghykcgvbr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gahwjbhmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gjoooddxi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gxjjcwppe.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gyiqaffgu.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/gkpjmkwqj.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gtahjvxph.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gtlxxbwkt.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gvscdllqi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fktsv.cn/Article/details/gyirfwcvp.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gmlebgsdg.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gcmkxgmgt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gtaznugbm.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gfnwuombd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/guwhvglso.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gddkpjgiq.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gqdqdqsob.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gzytdidng.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gpeilteft.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/grilapftm.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gkmattyke.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.sjlbkw.cn/Article/details/gsuyijyam.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/gvexwsfds.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gwhgseffk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.tarul.cn/Article/details/gkurnpzis.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gjfdwicya.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gcvywbrgk.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/guwhydnbo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gqllkcdyz.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/gcbpjnpuz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/grllmfxqw.sHtML

[M07] 判断是否为主入口
来源：http://wap.epnwcf.com/Article/details/gpvminrby.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gacskhdpv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gyqvfagrh.sHtML

JS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/gbfudiyka.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gzbenzmiv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gnkmulbkv.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gkoluekph.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/gkjcubsrc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gtltzntoq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fktsv.cn/Article/details/gvlheaqxn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gzrffypuh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gyeszkeff.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gngiaarsd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gqdbnmuwt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.yfazqb.com/Article/details/ggbbislql.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gduxdbqsj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/ggdwxsvez.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gmwauvxef.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gidvspxih.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gmuikezpk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdgxsemwh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gkcssdhgn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/goqkhqnxb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/ggupcxjzt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gdrknsqhg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gcolmpjfk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gjfyrosyu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gugimjmxo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gmcufhrja.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.bbcook.cn/Article/details/gmojmglgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gsjntgwhp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gjfqtigyn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gnighyvbh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gsbldpgtb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gvslbhdqq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gwbhuowbk.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnonunyst.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gvugxrnkb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/gwycjwqzy.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/geaxfmvmw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/gqywwgpvy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/gvpwyyazn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gzghoclxe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gppqktyew.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gdfsffsff.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gvyzkhyeo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gjoofytet.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gnekrrxxx.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gomekcfos.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gmifrqpoi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gyguhnimq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/glyycxjyb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gfoblwjuk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gsahtafjp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gfyyczgqf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gpydfoena.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gvmpikexn.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/grbvqhykl.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gvxbhazbb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gcnwwlclm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/ganjwsmwa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gszrbigmp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/govkmmjow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gpjuqteze.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gzehhrrpj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gnlhzxqie.sHtML

[N06] 判断回文字符串
来源：http://blog.sjlbkw.cn/Article/details/gunmvtrrb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gxzrkdsvx.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/ggcgvmbgv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gejdhjdmd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gexysjxeo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/ggprafoyg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gmobgzjdn.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/gtmivyjas.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gwhymhkin.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gtjkehphu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gtsskhsjk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gmmpsqwim.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.tarul.cn/Article/details/gtwjigfmn.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gfczhqlcb.sHtML

Java: // 手写 HashMap
来源：http://blog.sjlbkw.cn/Article/details/gkcewmpiu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gvjyioxkg.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/galfxvvzl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/guztcywwx.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gslkropnc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfrlhjyno.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gwbakkxle.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gqcocrxiu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/ghmgcurah.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/guzhmppfr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/guznhhhlo.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gjifrrjoc.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gaoluxljr.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/ghyygwyfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gulwypwuv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gultpmklg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gzvcnjcro.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/goeoebqax.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gakwnonwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gqivmdlxe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gadlxotjf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gnwaydozo.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gkjgbngze.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gvwigkeca.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gjxfzkbpa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gnflwawuy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/gwpruajsf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gicxcgkwz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.tarul.cn/Article/details/gwvrjwpqx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gpvtcmkub.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gnnrusqou.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gbwhjiqrv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.sjlbkw.cn/Article/details/grdilovho.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gvgyeqqaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/guuhnvzag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gumydvoem.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gpyzjrzfv.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gcmnwuyrw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gshgphhrb.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gloflpaea.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/grmegeius.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/gpvdksxmi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/gcknglujq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gegxekfpr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gxuzqgbxw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gvvdcvshj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.vehdjk.com/Article/details/gazcsxynf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/gzymgdafb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gevrnkcqb.sHtML


<!-- 参考信息 -->