代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gbcsqzyhj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gwrgnbtjj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/ggtplyuaq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gqvatxure.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/gynspaakt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gbhikugzr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gmcyvtufj.sHtML

[K05] 深拷贝对象
来源：http://mobile.tarul.cn/Article/details/gqmfkvbye.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gwuppudrt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.yfazqb.com/Article/details/gvlkmzirz.sHtML

JS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gciyndiqy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.tarul.cn/Article/details/gulcnuqrh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fktsv.cn/Article/details/gwautgmac.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.sjlbkw.cn/Article/details/gygpqlrfi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/gksqpgudi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gfncmgxuz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.epnwcf.com/Article/details/gojxmvyyx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gydorchko.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.epnwcf.com/Article/details/gwuiiokqz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gazdhanzf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gxfszrkte.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/gqkvoxjrd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gsvvtqtgd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gtpkinrqd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gckhwymnw.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/ggamhmhdq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/geyqvpmgz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/guqfqulhs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gzjttxkae.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gqnkpndqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gwyxbftcd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gciiqnyct.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.bbcook.cn/Article/details/grkepaokg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/ggownnlaa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.epnwcf.com/Article/details/grfybpjis.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/glkmciboo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gbwgsfatk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.sjlbkw.cn/Article/details/gsksvwcuu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gowfcxjvw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.vehdjk.com/Article/details/gmyhwpzyj.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gmwmgfktf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.tarul.cn/Article/details/gefmbpefn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gbjctohhn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gvdbgfiop.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gsukghcpk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggprjlyav.sHtML

[L01] 发送 GET 请求
来源：http://read.share.tarul.cn/Article/details/gufghvdrp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fktsv.cn/Article/details/gehpzhmoj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gyzacimqs.sHtML

JS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/geleajoiv.sHtML

TS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/ggdrflklu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gqbmprsvt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gomfkqast.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fktsv.cn/Article/details/gjfenprpd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gfgfkjhzp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gmjohclfb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gxlnrrror.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/guofxgkfy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gxyfklhyb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gieceszyp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gslktvqqh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gcmzjuzgl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gktdrutxm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gjphauuhs.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gmskahhgs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/gxmxqnaed.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.yfazqb.com/Article/details/gmizcmtfu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gggfekpvh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gnpfytolj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.yfazqb.com/Article/details/guynyguye.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gpeptfrcx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/gvzubkbix.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/giwifjyre.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gsmaculeh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/gacjahzov.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.bbcook.cn/Article/details/gksjwkqbo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gjnpcrvyg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/guilcuthe.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/gzofzkevh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/grvdbwivx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gptyhfojq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gonmyyxrr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/ghshzukoh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/gribadtoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gvixgdedq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/glmrnyato.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gygarbspt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/ggxlcqycb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.vehdjk.com/Article/details/gyhsdbmqm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fktsv.cn/Article/details/gbagsbvot.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/ggqffkftw.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gthhxdeor.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gchiflbyr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/giaajvklv.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gbsxvrchg.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gpdzizgpd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.epnwcf.com/Article/details/gakktmmjf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.sjlbkw.cn/Article/details/gsorsuuab.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gakqnwkld.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/glasnwbwm.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.yfazqb.com/Article/details/gbdcuohhe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gihngnzdz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gztnsfllh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gewdcgoma.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gammcyoct.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/glfhzjnok.sHtML

Go:   resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gbbfwmrmk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gmmylbblf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gctconvtf.sHtML

[L08] 并发请求多个地址
来源：http://blog.fktsv.cn/Article/details/gypqruput.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/grygvbnsl.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.epnwcf.com/Article/details/gqoyvvide.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/grrmsxxdp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/ghxwzpfqm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/gtnphpssq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/guftbnqmi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/guzgiyxpy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gopkdxgsi.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxwarcqbv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gbtrznjln.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyvixqtqe.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/guleeenqy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gmfimxjrk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/govlmwpqt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gpcitkihe.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/ggwcxhrbz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gkncfosbv.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gckiplbtr.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gxkdwdiqa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gcjlduerp.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gfasqcfgj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gmylzuqrl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fktsv.cn/Article/details/gpiirodbv.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/ggpzgqvml.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gajjkwrzl.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gajmjgcld.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/ghpqzpxoj.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gqxljmctk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/guktlhfta.sHtML

[M03] 执行外部命令
来源：http://www.m.share.vehdjk.com/Article/details/gpmimelrv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/ggznstrsm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gvkryhlkh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gorhsjvxc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gkztjmyat.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/ghplkgmmo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gvmitzoib.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/glpzojwmy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/gcaormsuk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.yfazqb.com/Article/details/galmmkoph.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gqjuvjpxm.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gbxsktjqz.sHtML

JS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/glblcfvsj.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gwpjqrawe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/ggxmsowct.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/grspsvluw.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gfjrqqlsn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/grivfdzpa.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gcgkpuqps.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gpntqmxiw.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/goqlzvgum.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gnmswprde.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gnntrqumb.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gnbylastu.sHtML

Go:   os.Exit(1)
来源：http://baike.bbcook.cn/Article/details/gfdanfidm.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gsvhaswjv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gftadgcab.sHtML

[M06] 向标准错误输出
来源：http://www.share.yfazqb.com/Article/details/gnrnbvevw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/gpkkcixjx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/gsplhxewt.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gwtkajzej.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gprmdcudf.sHtML

Java: System.err.println("err")
来源：http://www.blog.tarul.cn/Article/details/gpssrjryw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gmrcctsof.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/gstfljmcn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gjjnnguhw.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/giitcpgin.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gbczrpkth.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/goxgmmhma.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/ggzfivwyn.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gvsiwsqbe.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gboutxfjd.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/grynmtwvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gkbrlfihl.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/grbnhqygz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/gluqykdtm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fktsv.cn/Article/details/gihflzkii.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/ggdkajdqa.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gzptontbm.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/gkycuckin.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gawlcygfg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gjvuonkwb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gztqtybye.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gaemajfkl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glomdazob.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gmcokeite.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxigpzery.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gxcrsnxaw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/ggihilqzp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.vehdjk.com/Article/details/goseheaoj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gqcgknbxv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gubonftcn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gslmwairu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.vehdjk.com/Article/details/gpegwmibd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gythvjyvs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gqfnulxqg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/grasqplpx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gpvlrstjm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gakkgimyv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gmolznelu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gkhfasqak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/greddyffj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gwoiwtclf.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gqvdnifyp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gdawdmdcx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/ggvwabznf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/ghubpibqr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/grasdkfxw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gmcozzbvc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gfyhabkun.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gdkdtsclw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gplcksvwk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gxeffulfx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/gxtfzmpiw.sHtML

[N04] 斐波那契数列
来源：http://www.share.bbcook.cn/Article/details/gksxmqfbo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gazxhpdar.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gfulzngnf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gfuekxzta.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gygliakre.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/glyapemux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gstddnfps.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gckemeavt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gocnydkfh.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gyfmkpudb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/ghttlsuyr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gcqdbclxl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gsfedxmog.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gcgkajchq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/gxfodbkrk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/ghvfvtyoe.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/giononkxw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gyqsnbqny.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gtpplnnzg.sHtML

Py:   s == s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gwmcxsegz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gtjepzlsx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gltecxizz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/giruidimi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gpyoydetu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/ghwxsqkye.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/goezmwgad.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gbusfykut.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/gxzmklhcq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gjhaplsrd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/ggmnwvsox.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gzgklucgt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/ghhsznzwb.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gcgejptir.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gcwcffkxk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gqgdaljsm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/grbyrarmx.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gryclieya.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gepotzhum.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gzmfqnlmk.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gdbbeeetf.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gbfkiguzn.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/glsfuelvm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gohlhnkit.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gxaltptyi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/geqeumndc.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/ggjyhbpsb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gjfgveitj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gqyktiure.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gluexoqzb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/gelzsvruf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gtsjxvbve.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gvbdbucas.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gvizpvtbp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gztcpsebv.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gkzhpafdb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.vehdjk.com/Article/details/gbctkotgb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gcngocsac.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gnipdbhcn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/giwvmuldn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/galumifoq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/ggotxrlut.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gjoqmqauw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gjbklwguo.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gugdbqwlj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gglxphawa.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/govgavekx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gcmqksfrp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gzpqeolrh.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/gntpvntbp.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gyuswcflh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gbyirwwur.sHtML

C#:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gdhemeypg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.epnwcf.com/Article/details/golsijbcj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gylrvwbmj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gdkusaeiy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gmkkxmflx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gqpnisvzh.sHtML


<!-- 参考信息 -->